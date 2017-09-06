# BurnableToken

Purpose: to share some part of the company profit with token holders.

Sheme:
Token creator sends a part of his income to the token contract.
Token owners are able to "burn" (sell to the contract and withdraw from circulation) part of their tokens, and receive some reward. This reward is calculated as <amount_of_burned_tokens> * <amount_of_ETH_on the_contract> / <total_amount_of_tokens>.

This reward actually works as a minimal sell price on exchange. (Nobody'll sell cheaper on exchange while they can sell to the contract.)
And this reward can only be increased (by sending more ETH to the contract) and'll never decrease. Peopeles wainting for the next profit from token creator will usually sell on exchange for the price greater than this minimal price.

Also, Ether is holded on the contract and is whitdrawn from circulation, which is good for Ethereum price.

Example:
There is toataly 1500000 tokens, and you've sent 500 ETH to the contract.
Bob burns his 100 tokens. His reward is 100 * 500 / 1500000 ≃ 0.033333333 ETH.
Then Alice also burns 100 tokens. She receives 100 * 499.966666667 / 1499900 ≃ 0.033333333 ETH (the same as Bob).
After this operations there are total 1499800 tokens and 499.966666667 ETH on the contract.
After next profit distribution 100 ETH were sended to the contract. And now there is 599.93333333367 ETH.
Then Jack burns his 100 tokens. His reward: 100 * 599.93333333367 / 1499900 ≃ 0.039998222 (greater then Alice's and Bob's because he waited for the profit distribution)
