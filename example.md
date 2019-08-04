# **Mining ERC-918 Tokens (0xBitcoin)**
<br>
### **GENERAL INFORMATION**

**[0xBitcoin (0xBTC)](https://0xbitcoin.org)** is the first mineable ERC20 token on Ethereum. It uses mining for distribution, unlike all previous ERC20 tokens which were assigned to the contract deployer upon creation. 0xBTC is the first implementation of the EIP918 mineable token standard ([https://eips.ethereum.org/EIPS/eip-918](https://eips.ethereum.org/EIPS/eip-918)), which opened up the possibility of a whole new class of mineable assets on Ethereum. Without any ICO, airdrop, pre-mine, or founder’s reward, 0xBitcoin is arguably the most decentralized asset in the Ethereum ecosystem, including even Ether (ETH), which had a large ICO.

The goal of [0xBitcoin](https://0xbitcoin.org) is to be looked at as a currency and store of value asset on Ethereum. Its 21 million token hard cap and predictable issuance give it scarcity and transparency in terms of monetary policy, both things that Ether lacks. 0xBitcoin has certain advantages over PoW based currencies, such as compatibility with smart contracts and decentralized exchanges. In addition, 0xBTC cannot be 51% attacked (without attacking Ethereum), is immune from the “death spiral”, and will receive the benefits of scaling and other improvements to the Ethereum network.

<br>
### **GETTING 0xBITCOIN TOKENS**

[0xBitcoin](https://0xbitcoin.org) can be mined using typical PC hardware, traded on exchanges (either decentralized or centralized) or purchased from specific sites/contracts.

##### -Mined using PC hardware

##### -Traded on exchanges such as

* *Enclaves ([https://enclaves.io/trade/0xBTC](https://enclaves.io/trade/0xBTC)) 0xBTC/ETH*

* *Fork Delta ([https://forkdelta.app/#!/trade/0xBTC-ETH](https://forkdelta.app/#!/trade/0xBTC-ETH)) 0xBTC/ETH*

* *Mercatox ([https://mercatox.com/](https://mercatox.com/)) 0xBTC/ETH and 0xBTC/BTC*

* *IDEX ([https://idex.market/eth/0xbtc](https://idex.market/eth/0xbtc)) 0xBTC/ETH*

* *or Traded OTC on the 0xBitcoin Discord or wherever traders see fit.*

  *~more listings are in the works. Feel free to suggest 0xBTC to your favorite exchanges!*

<br>
### **MINING IN A NUTSHELL**

0xBitcoin is a Smart Contract on the Ethereum network, and the concept of Token Mining is patterned after Bitcoin's distribution. Rather than solving 'blocks', work is issued by the contract, which also maintains a Difficulty which goes up or down depending on how often a Reward is issued. Miners can put their hardware to work to claim these rewards, in concert with specialized software, working either by themselves or together as a Pool. The total lifetime supply of 0xBitcoin is `21,000,000` tokens and rewards will repeatedly halve over time.

The 0xBitcoin contract was deployed by Infernal_Toast at Ethereum address: [0xb6ed7644c69416d67b522e20bc294a9a9b405b31](https://etherscan.io/address/0x8fea1cf4845417f0525f5effca0f312a8c419a4e)

* ##### **MINING IN MORE DETAIL (Gee-Whiz Info)**

0xBitcoin's smart contract, running on the Ethereum network, maintains a changing "Challenge" (that is generated from the previous Ethereum block hash) and an adjusting Difficulty Target. Like traditional mining, the miners solve for a Nonce value that, when hashed alongside the current Challenge and their Minting Ethereum Address, is less-than-or-equal-to the current Difficulty Target. Once a miner finds a solution that satisfies the requirements, they can submit it into the contract (calling the Mint() function). This is most often done through a mining pool. The Ethereum address that submits a valid solution first is sent the 50 0xBTC Reward.

(In the case of Pools, valid solutions that do not satisfy the full difficulty specified by the 0xBitcoin contract, but that DO satisfy the Pool's specified Minimum Share Difficulty, get a 'share'. When one of the Miners on that Pool finds a "Full" solution, the number of shares each miner's address has submitted is used to calculate how much of the 50 0xBTC reward they will get. After a Reward is issued, the Challenge changes.

* ##### **HOW DIFFICULTY ADJUSTMENT WORKS**

A Retarget happens every `1024` rewards. In short, the Contract tries to target an Average Reward Time of about 60 times the Ethereum block time. So (at the time of this writing):

 `~13.9 seconds \* 60 = 13.9 minutes`

If the average Reward Time is longer than that, the difficulty will decrease. If it's shorter, it will increase. How much longer or shorter it was affects the magnitude with which the difficulty will rise/drop, to a maximum of 50%.  
* *[Click Here](https://0x1d00ffff.github.io/0xBTC-Stats/) to visit the stats page~ (https://0x1d00ffff.github.io/0xBTC-Stats) to see recent stats and block times, feel free to ask questions about it if you need help understanding it.*

<br>
### **MINING HARDWARE**

*Presently, 0xBitcoin and "Alt Tokens" can be mined on GPUs, CPUs, IGPs (on-CPU graphics) and certain FPGAs. The most recommended hardware is nVidia graphics cards for their efficiency, ubiquity and relatively low cost. As general rules, the more cores and the higher core frequency (clock) you can get, the more Tokens you will earn!*

##### **Mining on nVidia cards:**
* Pascal (GTX 10x0) cards are usually the best choice due to their power efficiency. Maxwell-Generation 2 (GTX 9xx) cards are also a good choice and are often great overclockers, but they use more power/generate more heat. Any fairly-recent nVidia card supporting CUDA should be capable of mining Tokens. It's possible to mine in OpenCL mode on nVidia devices, but It is preferable to use a CUDA for substantially better performance. (See Mining Software section.)

##### **Mining on AMD cards:**
* AMD GPUs are quite capable of Token mining, though they can't achieve quite the same performance that nV/CUDA GPUs can at this time. Because of their typically-high memory bandwidth (especially cards with HBM/HBM2), it is possible to mine 0xBitcoin/ERC918 Tokens alongside a Video Memory-intensive algorithm like Ethash or Cryptonight!  (See Mining Software section.)

##### **Mining on IGPs (e.g. AMD Radeon and Intel HD Graphics):**
* This type of GPU is considerably less powerful than a discrete GPU, but is still capable of mining. They can supplement hashpower from other devices. The best performance should come from a chip with a larger number of Shader cores (like a Zen-based APU), but even typical Intel IGPs can submit shares and earn Tokens. (See Mining Software section.)

##### **Clocks and Power Levels:**
* The algorithm used for 0xBitcoin and Alt-Token mining uses the faster memories in a GPU core instead of Video Memory. As a result, it is advisable to underclock the Memory, which will save a little power, reduce memory temperature and sometimes enable the GPU core to hit higher clock speeds with stability. A card's Power Limit and Core Voltage can be tweaked to attain the best efficiency for individual cards.

    *~Pascal cards (like GTX 10x0) are generally more temperature-sensitive when overclocked. Reducing Core temperature can often stabilize higher overclocks better than adding voltage can. Maxwell-Gen2 cards (like GTX 9xx) can usually be overclocked further at higher temperatures.*

<br>
### **MINING SOFTWARE AND DESCRIPTIONS**

*For the most up-to-date version info, download links, thread links and author contact information, please see this thread: [https://www.reddit.com/r/0xbitcoin/comments/8o06dk/links\_to\_the\_newestbest\_miners\_for\_nvidia\_amd/](https://www.reddit.com/r/0xbitcoin/comments/8o06dk/links_to_the_newestbest_miners_for_nvidia_amd/)  Keep up to date for the latest speed, stability and feature enhancements!*

##### **-COSMiC Miner by LtTofu:**
 * V4.x versions are a near-total 'Modern' C++ rewrite/redesign for 64-bit Windows, built for speed, ease-of-use and stability. It supports nVidia/CUDA devices and Pool Mining. Solo/CPU mining both planned. Features a fully-integrated GUI, numerous optimizations assembly functions for speed (nicknamed 'Hashburner'), and supports multiple GPUs running in a single instance since v4.1. Auto-Donation/devfee of 1.5% (default of 1.5%.) Under active development!

	###### --COSMiC Miner 3.4t by LtTofu:
	A fork of 0xBitcoin-Miner designed for enhanced speed and less invalid shares at the Pool level. It is somewhat older and is built using a combination of NodeJS/C++/CUDA. It has versions available for 64-bit Windows and Linux and runs from a command-line interface. Comes in multiple versions with 1, 1.5 or 2% "Auto-Donation"/devfee. Not under development at this time, but still relevant.

##### **-SoliditySha3Miner by Amano7:**

* A Command-Line Interface miner that aims to provide functionality similar to that of "CCMiner" for other algorithms for 0xBitcoin and other ERC-918s. As such, it offers an API for integrating with Mining management software and integration with EthOS is in the works. It uses the CUDA core from COSMiC Miner and also supports OpenCL devices (such as AMD cards and Intel IGPs.) Has a minimum Auto-Donation/devfee of 1.5% (with a default of 2.0%.) Under active development!

##### **-AIOMiner All-In-One GPU Miner:**
* AIOMiner is an All-In-One GPU Mining software for Windows that boasts support for over 55 different algorithms, is free to use, and eliminates the need to configure batch files through its easy to use interface.

##### **-TokenMiner by MVis (Mining-Visualizer):**

* TokenMiner is based upon Genoil Ethminer and was the first to add support for OpenCL devices (AMD GPUs/APUs.) It supports CPU and Pool/Solo mining from its command-line interface (in -C or -G, -S or -P modes.) It can also mine on nVidia/CUDA cards (in OpenCL mode, albeit with lesser performance.) Has a 1% "devfee" running in Pool Mode. This miner has since been forked for compatibility with some FPGAs!

##### **-"Nabiki"/2.10.4 by Azlehria:**

* v2.10.4 is an enhancement of the original 0xBitcoin-Miner with CUDA support added by Mikers and enhanced by Azlehria. "Nabiki" is a C++-only version, with no NodeJS code, which supports Pool Mining (just not Solo) and works on Windows 64-bit and Linux. Source code is available with pre-packaged binaries and a GUI in the works. Has a 2.5% "devfee". Under active development!

~*Older Miners: Older and possibly-unsupported miner versions can be found at the above link for historical purposes and specific applications- including the original NodeJS CPU miner by Infernal Toast/Zegordo, the '1000x' NodeJS/C++ hybrid version of 0xBitcoin-Miner and Mikers' enhanced CUDA builds.*

&#x200B;

### **FOR MORE INFORMATION...**

If you have any trouble, the friendly and helpful 0xBitcoin community will be happy to help you out. Discord has kind of become 0xBTC's community hub, you can get answers the fastest from devs and helpful community members. Or message one of the community members on reddit listed below.
##### *Links*
* Discord: [https://discordapp.com/invite/xAPwaDC](https://discordapp.com/invite/xAPwaDC)

* 0xBitcoin Subreddit: [https://www.reddit.com/r/0xbitcoin/](https://www.reddit.com/r/0xbitcoin/)

* 0xBitcoin Forum: [http://forum.0xbtc.io/](http://forum.0xbtc.io/)

* Token Mining Subreddit: [https://www.reddit.com/r/tokenmining/](https://www.reddit.com/r/tokenmining/)
