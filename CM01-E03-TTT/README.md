# CONTRACT TIC TAC TOE WITH DF85

# CCIP TIC TAC TOE

## CONTRACT ON FUJI: 

Command: npx hardhat run ./scripts/deployTicTacToe.ts --network avalancheFuji

✅ Tic Tac Toe Demo deployed at address 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF on avalancheFuji blockchain

Router FUJI: 0xF694E193200268f9a4868e4Aa017A0118C9a8177

Chain selector Fuji: 14767482510784806043

## CONTRACT ON AMOY: 

Command: npx hardhat run ./scripts/deployTicTacToe.ts --network polygonAmoy

✅ Tic Tac Toe Demo deployed at address 0xAd9A7755D6149A3431C972A9e078a47cb9B27A49 on polygonAmoy blockchain

https://amoy.polygonscan.com/address/0xAd9A7755D6149A3431C972A9e078a47cb9B27A49

Router Amoy: 0x9C32fCB86BF0f4a1A8921a9Fe46de3198bb884B2

Chain selector Amoy: 16281711391670634445

## CONTRACT ON SEPOLIA: 

Command: npx hardhat run ./scripts/deployTicTacToe.ts --network ethereumSepolia

✅ Tic Tac Toe Demo deployed at address 0x30641DfE54052CA56cdfb5D1638299798d0897AB on ethereumSepolia blockchain

https://sepolia.etherscan.io/address/0x30641DfE54052CA56cdfb5D1638299798d0897AB

Router Sepolia: 0x0BF3dE8c5D3e8A2B34D2BEeB17ABfCeBaf363A59

Chain selector Sepolia: 16015286601757825753

### ROUTER UPDATE:

npx hardhat ttt-update-router --blockchain ethereumSepolia --contract 0x30641DfE54052CA56cdfb5D1638299798d0897AB --router 0x0BF3dE8c5D3e8A2B34D2BEeB17ABfCeBaf363A59

✅ Update successful, transaction hash: 0x5ea5186d98e7c22c913c3110039574c2d0c2ae399ae2f1711690a411462e1a8c

npx hardhat ttt-update-router --blockchain avalancheFuji --contract 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF --router 0xF694E193200268f9a4868e4Aa017A0118C9a8177

✅ Update successful, transaction hash: 0xd0df7e237ffb8b15acc3b2c19639d58942ba88ca170c13158839c25bc68c47cb

npx hardhat ttt-update-router --blockchain polygonAmoy --contract 0xAd9A7755D6149A3431C972A9e078a47cb9B27A49 --router 0x9C32fCB86BF0f4a1A8921a9Fe46de3198bb884B2


### START GAME BETWEEN SEPOLIA AND FUJI:

npx hardhat ttt-start --source-blockchain ethereumSepolia --sender 0x30641DfE54052CA56cdfb5D1638299798d0897AB --destination-blockchain avalancheFuji --receiver 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF

### START GAME BETWEEN FUJI AND SEPOLIA:

npx hardhat ttt-start --source-blockchain avalancheFuji --sender 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF --destination-blockchain ethereumSepolia --receiver 0x30641DfE54052CA56cdfb5D1638299798d0897AB

✅ Message sent, game session created! transaction hash: 0x8c8559154c258509f77552bde87f11f42fb0472255b287fd6a7945f597c9073c

https://ccip.chain.link/#/side-drawer/msg/0x4faa634e03a075ff4c3b8578d462e06d7ee3e13d4a0c71edbaee728e9b1987c0

### Get session ID:

sessionId at index 0 is: 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c

npx hardhat ttt-get-sessionId --blockchain ethereumSepolia --contract 0x30641DfE54052CA56cdfb5D1638299798d0897AB --index 0

npx hardhat ttt-get-sessionId --blockchain avalancheFuji --contract 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF --index 0

### Player 2 makes a move in Blockchain 2

npx hardhat ttt-move --x 0 --y 0 --player 2 --session-id 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c --source-blockchain avalancheFuji --sender 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF --destination-blockchain ethereumSepolia --receiver 0x30641DfE54052CA56cdfb5D1638299798d0897AB

#### ✅ Message sent, you make a move! transaction hash: 0xec68fa022fb7ecfbace97a2ccecbc5a8c3aabae644688e5a44c1c1667c377018

npx hardhat ttt-move --x 0 --y 2 --player 2 --session-id 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c --source-blockchain avalancheFuji --sender 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF --destination-blockchain ethereumSepolia --receiver 0x30641DfE54052CA56cdfb5D1638299798d0897AB

#### ✅ Message sent, you make a move! transaction hash: 0x4b90e6c4cbae39223c00f8058e29f1bdae15569966bf27418c5802ce83a99d0e



### Player 1 makes a move in Blockchain 1

npx hardhat ttt-move --x 0 --y 1 --player 1 --session-id 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c --source-blockchain ethereumSepolia --sender 0x30641DfE54052CA56cdfb5D1638299798d0897AB --destination-blockchain avalancheFuji --receiver 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF

#### ✅ Message sent, you make a move! transaction hash: 0xe29e054f80ec184db29e277fb8bdeb8df84becb0e4bbc932c8bd84a28c8b0d59

npx hardhat ttt-move --x 1 --y 0 --player 1 --session-id 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c --source-blockchain ethereumSepolia --sender 0x30641DfE54052CA56cdfb5D1638299798d0897AB --destination-blockchain avalancheFuji --receiver 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF

✅ Message sent, you make a move! transaction hash: 0xf4886820f1e87c8cde1bfdca6b1a6b8c8eaa7dbfc313404fe31a606ae353ef11

npx hardhat ttt-move --x 1 --y 1 --player 1 --session-id 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c --source-blockchain ethereumSepolia --sender 0x30641DfE54052CA56cdfb5D1638299798d0897AB --destination-blockchain avalancheFuji --receiver 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF

✅ Message sent, you make a move! transaction hash: 0xdcac907ce9a0cfa54bb2d64dd8344bf749753ff62f14042503fd11c60d165086

npx hardhat ttt-move --x 2 --y 1 --player 1 --session-id 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c --source-blockchain ethereumSepolia --sender 0x30641DfE54052CA56cdfb5D1638299798d0897AB --destination-blockchain avalancheFuji --receiver 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF

✅ Message sent, you make a move! transaction hash: 0x29479474721b5a559b0691aa833899e973f04a8085e7b2fef35a4b3092aee2b1

### Check the winner

npx hardhat ttt-check-winner --blockchain ethereumSepolia --contract 0x30641DfE54052CA56cdfb5D1638299798d0897AB --session-id 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f3 

#### winner of sessionId 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c is: 0x0000000000000000000000000000000000000000

npx hardhat ttt-check-winner --blockchain avalancheFuji --contract 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF --session-id 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c

#### winner of sessionId 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c is: 0x0000000000000000000000000000000000000000
