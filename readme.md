# Lottery Contract
## How it works
- Players put their eth into the smart contract
- Manager then will tell the contract to pick a winner
- Contract will pick one of the player, and will send all the money out of the prize pool to the winner
- Contract will then reset

Lottery contract structure
variables
- manager: address of person who created the contract
- players: store array of addresses who have entered ETH

function
- enter: players enter into the lottery
- pickWinner: randomly picks a winner and send them all the eth

## Miscellaneous
- pseudo random code in solidity because Solidity doesn't have random. `return uint(keccak256(block.difficulty, now, players));`
- The modulo operator works by dividing a number with a divisor then returns with a remainder. The remainder will always be less than the divisor.