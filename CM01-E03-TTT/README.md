# CONTRACT TIC TAC TOE WITH DF85

# CCIP TIC TAC TOE

## CONTRACT ON FUJI: 

Command: npx hardhat run ./scripts/deployTicTacToe.ts --network avalancheFuji



Router FUJI: 0xF694E193200268f9a4868e4Aa017A0118C9a8177

Chain selector Fuji: 14767482510784806043

## CONTRACT ON AMOY: 

Command: npx hardhat run ./scripts/deployTicTacToe.ts --network polygonAmoy

Router Amoy: 0x9C32fCB86BF0f4a1A8921a9Fe46de3198bb884B2

Chain selector Amoy: 16281711391670634445

## CONTRACT ON SEPOLIA: 

Command: npx hardhat run ./scripts/deployTicTacToe.ts --network ethereumSepolia





Router Sepolia: 0x0BF3dE8c5D3e8A2B34D2BEeB17ABfCeBaf363A59

Chain selector Sepolia: 16015286601757825753

### ROUTER UPDATE:

npx hardhat ttt-update-router --blockchain ethereumSepolia --contract 0x30641DfE54052CA56cdfb5D1638299798d0897AB --router 0x0BF3dE8c5D3e8A2B34D2BEeB17ABfCeBaf363A59



npx hardhat ttt-update-router --blockchain avalancheFuji --contract 0x48fBa5197563022709284AAA7d8eb9CcE751C042 --router 0xF694E193200268f9a4868e4Aa017A0118C9a8177



npx hardhat ttt-update-router --blockchain polygonAmoy --contract 0xAd9A7755D6149A3431C972A9e078a47cb9B27A49 --router 0x9C32fCB86BF0f4a1A8921a9Fe46de3198bb884B2


### START GAME BETWEEN SEPOLIA AND FUJI:

npx hardhat ttt-start --source-blockchain ethereumSepolia --sender 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2 --destination-blockchain avalancheFuji --receiver 0x48fBa5197563022709284AAA7d8eb9CcE751C042

### START GAME BETWEEN FUJI AND SEPOLIA:

npx hardhat ttt-start --source-blockchain avalancheFuji --sender 0x48fBa5197563022709284AAA7d8eb9CcE751C042 --destination-blockchain ethereumSepolia --receiver 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2





### Get session ID:

sessionId at index 0 is:

npx hardhat ttt-get-sessionId --blockchain ethereumSepolia --contract 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2 --index 0

npx hardhat ttt-get-sessionId --blockchain avalancheFuji --contract 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF --index 0

### Player 2 makes a move in Blockchain 2

#### Move 2: 
npx hardhat ttt-move --x 0 --y 1 --player 2 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain avalancheFuji --sender 0x48fBa5197563022709284AAA7d8eb9CcE751C042 --destination-blockchain ethereumSepolia --receiver 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2

#### Move 4:
npx hardhat ttt-move --x 1 --y 2 --player 2 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain avalancheFuji --sender 0x48fBa5197563022709284AAA7d8eb9CcE751C042 --destination-blockchain ethereumSepolia --receiver 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2

#### Move 6:
npx hardhat ttt-move --x 2 --y 1 --player 2 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain avalancheFuji --sender 0x48fBa5197563022709284AAA7d8eb9CcE751C042 --destination-blockchain ethereumSepolia --receiver 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2

#### Move 8:
npx hardhat ttt-move --x 0 --y 2 --player 2 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain avalancheFuji --sender 0x48fBa5197563022709284AAA7d8eb9CcE751C042 --destination-blockchain ethereumSepolia --receiver 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2

### Player 1 makes a move in Blockchain 1

#### Move 1: 
npx hardhat ttt-move --x 0 --y 0 --player 1 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain ethereumSepolia --sender 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2 --destination-blockchain avalancheFuji --receiver 0x48fBa5197563022709284AAA7d8eb9CcE751C042

#### Move 3: 
npx hardhat ttt-move --x 1 --y 1 --player 1 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain ethereumSepolia --sender 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2 --destination-blockchain avalancheFuji --receiver 0x48fBa5197563022709284AAA7d8eb9CcE751C042

#### Move 5: 
npx hardhat ttt-move --x 2 --y 2 --player 1 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain ethereumSepolia --sender 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2 --destination-blockchain avalancheFuji --receiver 0x48fBa5197563022709284AAA7d8eb9CcE751C042

#### Move 7: 
npx hardhat ttt-move --x 1 --y 0 --player 1 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain ethereumSepolia --sender 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2 --destination-blockchain avalancheFuji --receiver 0x48fBa5197563022709284AAA7d8eb9CcE751C042

#### Move 9: 
npx hardhat ttt-move --x 2 --y 0 --player 1 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain ethereumSepolia --sender 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2 --destination-blockchain avalancheFuji --receiver 0x48fBa5197563022709284AAA7d8eb9CcE751C042

### Check the winner

npx hardhat ttt-check-winner --blockchain ethereumSepolia --contract 0xd61E14AE090e89773e8274869F7b2F75FeC3Aad2 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc 

#### winner of sessionId 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c is: 0x0000000000000000000000000000000000000000

npx hardhat ttt-check-winner --blockchain avalancheFuji --contract 0x63EE1a476b19676800aC8130B4b8ddd54799EdeF --session-id 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c

#### winner of sessionId 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c is: 0x0000000000000000000000000000000000000000
