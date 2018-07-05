### How to prevent forgery? And how to establish intent (e.g. of payment)?

Digital currency is string of bits, which is copyable, hence (1) usable many times (2) forgeable.

**Solution:** sign message “Alice is giving Bob one coin” with her private key (digital signature). Anyone with her 
public key can confirm that she (and nobody else) signed it, so 

1. She can’t deny it (establishing intent); 
2. Nobody could’ve forged it from scratch (they can still duplicate it, after Alice makes the message public). 

_(Remark: the message is the money. Later improvements upon this proto-bitcoin will just comprise more elaborate messages.)_

### How to prevent double-spending?

It’s still a string of bits, so Alice can keep sending the message over and over, to Bob or many different 
people. Is this many different coins, or accidental duplication, or malicious duplication (i.e. Alice wants Bob to think 
she sent him many coins, when she only sent one)?

**Solution:** uniquely label coins, using a trusted source of labels (serial numbers), e.g. banks. Banks would

1.	Provide serial numbers for each coin
2.	Keep track of who has which coins (in a ledger of coin transactions)
3.	Validate transactions to users

Example: 

```markdown
Alice withdraws money (one coin) from bank: bank 
(1) reduces account balance by one coin, 
(2) assigns Alice a never-before-used serial number, e.g. 314159. 
Alice wants to pay Bob: she signs “Alice is giving Bob one coin labeled 314159” with private key. Bob 
(1) checks with Alice’s public key to establish intent of payment, 
(2) checks with bank that this exact coin currently belongs to Alice to 
  (2a) establish ownership, 
  (2b) prevent double-spending; 
(3) tells bank he accepts Alice’s payment. 
Bank updates both users’ accounts to show that coin 314159 now belongs to Bob, not Alice.
```

### How to get rid of the bank? 

_(This is also called "decentralizing the money supply".)_

Alice can send the message “pay Bob coin 314159” to Bob, and “pay Charlie coin 314159” to Charlie simultaneously. 
If they verify the transaction before hearing from one another, their own copies of the blockchain will say that 
the coin is Alice’s to spend, so they’ll accept and broadcast both transactions. Which transaction should other users 
accept? How to prevent Bob or Charlie being cheated? There’s a time window between Bob’s acceptance of payment and 
everyone else (including Charlie) being notified of Bob’s acceptance, and updating their blockchain copies with 
Alice-Bob’s transaction, thereby rejecting Alice-Charlie: Alice can (1) do network traffic analysis to identify times 
when Bob and Charlie have lots of latency in communication, (2) disrupt Bob-Charlie’s comms. How?

**Solution:** don’t validate transactions themselves, ask everyone else to help validate. This “maintains blockchain 
integrity”. Since “everyone” is ill-defined (network always grows), substitute “enough users”.

Example using a legitimate transaction: 

```markdown
Alice sends signed message “314159” to Bob. Bob verifies Alice’s sign (intent to pay), checks with enough users 
that transaction is legitimate, enough users agree and broadcast agreement, Bob accepts payment and tells everyone, 
everyone updates blockchain copies.
```

Example using an _illegitimate_ transaction: 

```markdown
Alice sends signed message “314159” to Bob, and “314159” to Charlie. Bob verifies Alice’s sign (intent to pay), 
checks with everyone that transaction is legitimate. Charlie does same. Enough users notice conflicting transactions, 
and reject legitimacy. Both Bob and Charlie reject payment, and broadcast rejection. No one’s blockchain is updated: 
all recorded transactions are guaranteed legitimate.
```
