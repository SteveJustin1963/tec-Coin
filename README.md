# tec-Coin
A tec-1 bitcoin system. You know what they say "if it can be computed  by hand then the z80 can do it too". 

## sudo code
- record current financial record in ledger (new purchase history etc.)
- concatanate a hash of previous block in the chain                       `:H code h!;`
  - https://en.wikipedia.org/wiki/MD5#Algorithm 
- add a integer (Lets call it :A), First time round,                      `:0a!; \\counter`
- [D] Concatante :A at the end, Hash through an alorigthm (MD5, SHA1 etc) `a h +`
- check if output meets a certain condition (Like having 3 0's at the end)
- If does not meet condition, Imcrement                                   `:A 0 at enth()();` and goto [D]
- When the condition is met, organise the block, this is done by:
- Combine the financial record with the integer and this with the hash
- Add this block onto the chain
- Update this copy of the block chain to all users of the network
- Your done! be sure to repeat this operation as fast as possible to prevent counterfeit of your currency
- every now and then, verify the blockchain, by hashing the part containing the financal record and number (:A) to make sure it has not been tampered with and review the financial history to make sure everyones balances is correct
 



## Ref 
- https://lifehacker.com/how-to-create-your-own-cryptocurrency-1825337462
- http://www.righto.com/2014/09/mining-bitcoin-with-pencil-and-paper.html
