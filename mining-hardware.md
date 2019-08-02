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
