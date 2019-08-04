### **MINING IN A NUTSHELL**

0xBitcoin is a Smart Contract on the Ethereum network, and the concept of Token Mining is patterned after Bitcoin's distribution. Rather than solving 'blocks', work is issued by the contract, which also maintains a Difficulty which goes up or down depending on how often a Reward is issued. Miners can put their hardware to work to claim these rewards, in concert with specialized software, working either by themselves or together as a Pool. The total lifetime supply of 0xBitcoin is `21,000,000` tokens and rewards will repeatedly halve over time.

The 0xBitcoin contract was deployed by Infernal_Toast at Ethereum address: [0xb6ed7644c69416d67b522e20bc294a9a9b405b31](https://etherscan.io/address/0xb6ed7644c69416d67b522e20bc294a9a9b405b31)

*  **MINING IN MORE DETAIL (Gee-Whiz Info)**

0xBitcoin's smart contract, running on the Ethereum network, maintains a changing "Challenge" (that is generated from the previous Ethereum block hash) and an adjusting Difficulty Target. Like traditional mining, the miners use the SoliditySHA3 algorithm to solve for a Nonce value that, when hashed alongside the current Challenge and their Minting Ethereum Address, is less-than-or-equal-to the current Difficulty Target. Once a miner finds a solution that satisfies the requirements, they can submit it into the contract (calling the Mint() function). This is most often done through a mining pool. The Ethereum address that submits a valid solution first is sent the 50 0xBTC Reward.

(In the case of Pools, valid solutions that do not satisfy the full difficulty specified by the 0xBitcoin contract, but that DO satisfy the Pool's specified Minimum Share Difficulty, get a 'share'. When one of the Miners on that Pool finds a "Full" solution, the number of shares each miner's address has submitted is used to calculate how much of the 50 0xBTC reward they will get. After a Reward is issued, the Challenge changes.

*  **HOW DIFFICULTY ADJUSTMENT WORKS**

A Retarget happens every `1024` rewards. In short, the Contract tries to target an Average Reward Time of about 60 times the Ethereum block time. So (at the time of this writing):

 `~13.9 seconds \* 60 = 13.9 minutes`

If the average Reward Time is longer than that, the difficulty will decrease. If it's shorter, it will increase. How much longer or shorter it was affects the magnitude with which the difficulty will rise/drop, to a maximum of 50%.
* *[Click Here](https://0x1d00ffff.github.io/0xBTC-Stats/) to visit the stats page~ (https://0x1d00ffff.github.io/0xBTC-Stats) to see recent stats and block times, feel free to ask questions about it if you need help understanding it.*
