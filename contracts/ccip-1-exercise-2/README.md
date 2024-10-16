# CCIP 1 - MASTERCLASS

## EXERCISE 2A: SEND DATA FROM AVALANCHE FUJI TO ETHEREUM SEPOLIA

### SENDER CONTRACT (AVALANCHE FUJI): 0x88eF1a9c14046e4f9DA2B9b95C741FdD23B56C63

https://testnet.snowtrace.io/address/0x88eF1a9c14046e4f9DA2B9b95C741FdD23B56C63

#### Router address:	0xF694E193200268f9a4868e4Aa017A0118C9a8177

#### LINK: 0x0b9d5D9136855f6FEc3c0993feE6E9CE8a297846

1/ Send 10 LINK to: 0x88eF1a9c14046e4f9DA2B9b95C741FdD23B56C63

2/ whitelistChain (Ethereum Sepolia): 16015286601757825753


### RECEIVER CONTRACT (ETHEREUM SEPOLIA): 0xa63d6b21cb7f53da32cb11eea643d07de783194f

https://sepolia.etherscan.io/address/0xa63d6b21cb7f53da32cb11eea643d07de783194f#code

#### Router address: 0x0BF3dE8c5D3e8A2B34D2BEeB17ABfCeBaf363A59

#### Price: 100

3/ whitelistSender (sender contract): 0x88eF1a9c14046e4f9DA2B9b95C741FdD23B56C63

4/ whitelistSourceChain (avalanche fuji): 14767482510784806043

5/ TransferToken:

destinationChainSelector (ethereum sepolia): 16015286601757825753

receiver (contract): 0xA63D6B21Cb7F53Da32cB11EEa643d07De783194f

token (CCIP_BnM): 0xD21341536c5cF5EB1bcb58f6723cE26e8D8E90e4

amount: 100

6/ Transaction:  Fail (Gaslimit)

======================================================

## EXERCISE 2B: SEND DATA FROM ETHEREUM SEPOLIA TO AVALANCHE FUJI

### SENDER CONTRACT (ETHEREUM SEPOLIA): 0x3763AAe80d9709c3af58115ACD8Bbc6fCcb83892

https://sepolia.etherscan.io/address/0x3763aae80d9709c3af58115acd8bbc6fccb83892

#### Router address:	0x0BF3dE8c5D3e8A2B34D2BEeB17ABfCeBaf363A59

#### LINK: 0x779877A7B0D9E8603169DdbD7836e478b4624789

1/ Send 10 LINK to: 0x3763AAe80d9709c3af58115ACD8Bbc6fCcb83892

1a/ Send 0.1 CCIP_BnM to: 0x3763AAe80d9709c3af58115ACD8Bbc6fCcb83892

2/ whitelistChain (FUJI): 


### RECEIVER CONTRACT (AVALANCHE FUJI): 0xf23a0ff715256f71255c419162FfAb3646f771Fe

https://testnet.snowtrace.io/address/0xf23a0ff715256f71255c419162FfAb3646f771Fe

#### Router address: 

#### Price: 100

3/ whitelistSender (sender contract): 

4/ whitelistSourceChain (avalanche fuji): 

5/ TransferToken:

destinationChainSelector (ethereum sepolia): 

receiver (contract): 

token (CCIP_BnM): 

amount: 100

6/ Transaction:
