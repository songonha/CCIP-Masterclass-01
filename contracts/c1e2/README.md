## EXERCISE 2: SEND DATA FROM ETHEREUM SEPOLIA TO AMOY

### SENDER CONTRACT (ETHEREUM SEPOLIA): 0x22f21830EEfCE7242cef260418C3276DBC86Bf9E

https://sepolia.etherscan.io/address/0x22f21830eefce7242cef260418c3276dbc86bf9e

#### Router address:	0x0BF3dE8c5D3e8A2B34D2BEeB17ABfCeBaf363A59

#### LINK: 0x779877A7B0D9E8603169DdbD7836e478b4624789

1/ Send 10 LINK to: 0x22f21830EEfCE7242cef260418C3276DBC86Bf9E

1a/ Send 0.1 CCIP_BnM to: 0x22f21830EEfCE7242cef260418C3276DBC86Bf9E

2a/ whitelistChain (FUJI): 14767482510784806043

2b/ whitelistChain (AMOY): 16281711391670634445

2c/ whitelistChain (BSC): 13264668187771770619


###  2B1 RECEIVER CONTRACT (AVALANCHE FUJI): 0xee560d18109bcBd0a88cEC1784Cb1B68b4e334c8

https://testnet.snowtrace.io/address/0xee560d18109bcBd0a88cEC1784Cb1B68b4e334c8

#### Router address: 

#### Price: 100

3/ whitelistSender (sender contract): 0x3763AAe80d9709c3af58115ACD8Bbc6fCcb83892

4/ whitelistSourceChain (SEPOLIA): 14767482510784806043

##### 5/ TransferToken:

5a/ TransferToken to FUJI: 

destinationChainSelector (FUJI): 14767482510784806043

receiver (contract): 0xee560d18109bcBd0a88cEC1784Cb1B68b4e334c8

token (CCIP_BnM): 0xFd57b4ddBf88a4e07fF4e34C487b99af2Fe82a05

amount: 100

Transaction:

https://ccip.chain.link/#/side-drawer/msg/0xd95c73327c21a499bd890867aa781d25746ecb59b5685497a3b566832be794dc

https://ccip.chain.link/#/side-drawer/msg/0x1622f5083504d03bb6f6b931fe17d3d58d8d364f03e289d207dff07df33b3ac2

=============================================

###  2B2 RECEIVER CONTRACT (AMOY): 0xb6843ba34c706fa1687a5b7ee99e25d19d3910df

https://www.oklink.com/vi/amoy/address/0xb6843ba34c706fa1687a5b7ee99e25d19d3910df

#### Router address: 0x9C32fCB86BF0f4a1A8921a9Fe46de3198bb884B2

#### Price: 100

3/ whitelistSender (sender contract): 0x3763AAe80d9709c3af58115ACD8Bbc6fCcb83892

4/ whitelistSourceChain (SEPOLIA): 14767482510784806043

##### 5/ TransferToken:

5a/ TransferToken to AMOY: (NFT: 0x62C2268290619743D3017ba082a193d5CbDD5bEc)

destinationChainSelector (AMOY): 16281711391670634445

receiver (contract): 0xB6843bA34c706Fa1687a5b7EE99E25D19d3910Df

token (CCIP_BnM adress on Amoy): 0xFd57b4ddBf88a4e07fF4e34C487b99af2Fe82a05

amount: 100

Transaction:
