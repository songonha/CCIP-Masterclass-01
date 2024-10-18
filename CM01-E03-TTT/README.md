# CONTRACT TIC TAC TOE WITH DF85

# CCIP TIC TAC TOE

## CONTRACT ON FUJI: 

Command: npx hardhat run ./scripts/deployTicTacToe.ts --network avalancheFuji

✅ Tic Tac Toe Demo deployed at address 0x1a8110B7252d65E2C367e0B2285BE88DAe502486 on avalancheFuji blockchain

https://testnet.snowtrace.io/address/0x1a8110B7252d65E2C367e0B2285BE88DAe502486

Router FUJI: 0xF694E193200268f9a4868e4Aa017A0118C9a8177

Chain selector Fuji: 14767482510784806043

## CONTRACT ON AMOY: 

Command: npx hardhat run ./scripts/deployTicTacToe.ts --network polygonAmoy

Router Amoy: 0x9C32fCB86BF0f4a1A8921a9Fe46de3198bb884B2

Chain selector Amoy: 16281711391670634445

## CONTRACT ON SEPOLIA: 

Command: npx hardhat run ./scripts/deployTicTacToe.ts --network ethereumSepolia

✅ Tic Tac Toe Demo deployed at address 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE on ethereumSepolia blockchain

https://sepolia.etherscan.io/address/0x4726e37410e20c86a4da66fdf53f419bbf4e64fe

Router Sepolia: 0x0BF3dE8c5D3e8A2B34D2BEeB17ABfCeBaf363A59

Chain selector Sepolia: 16015286601757825753

### ROUTER UPDATE:

npx hardhat ttt-update-router --blockchain ethereumSepolia --contract 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE --router 0x0BF3dE8c5D3e8A2B34D2BEeB17ABfCeBaf363A59

✅ Update successful, transaction hash: 0x861176973b0813bbc83e74976d4f4f1915de2a59e2e07d0d913fed5f1652a7ed

npx hardhat ttt-update-router --blockchain avalancheFuji --contract 0x1a8110B7252d65E2C367e0B2285BE88DAe502486 --router 0xF694E193200268f9a4868e4Aa017A0118C9a8177

✅ Update successful, transaction hash: 0x400b0d4f0bcdb95133369aa3175e2bf326d943fd30f77062a4c485bc9a8a9a54

npx hardhat ttt-update-router --blockchain polygonAmoy --contract 0xAd9A7755D6149A3431C972A9e078a47cb9B27A49 --router 0x9C32fCB86BF0f4a1A8921a9Fe46de3198bb884B2


### DEPOSITE NATIVE TOKEN TO SMART CONTRACT

ON SEPOLIA: 0.1 ETH

ON FUJI: 2 AVAX

### START GAME BETWEEN SEPOLIA AND FUJI:

npx hardhat ttt-start --source-blockchain ethereumSepolia --sender 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE --destination-blockchain avalancheFuji --receiver 0x1a8110B7252d65E2C367e0B2285BE88DAe502486



### START GAME BETWEEN FUJI AND SEPOLIA:

npx hardhat ttt-start --source-blockchain avalancheFuji --sender 0x1a8110B7252d65E2C367e0B2285BE88DAe502486 --destination-blockchain ethereumSepolia --receiver 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE

**✅ Message sent, game session created! transaction hash: 0x850ba256f32e2c203d9d3879c7e1d2911dc5d64bf1da114ec180609ebc342eac**
✅ Message sent, game session created! transaction hash: 0x850ba256f32e2c203d9d3879c7e1d2911dc5d64bf1da114ec180609ebc342eac


### Get session ID:

sessionId at index 0 is:

npx hardhat ttt-get-sessionId --blockchain ethereumSepolia --contract 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE --index 0

npx hardhat ttt-get-sessionId --blockchain avalancheFuji --contract 0x1a8110B7252d65E2C367e0B2285BE88DAe502486 --index 0

sessionId at index 0 is: 0xbb9ae76f71906dbfbdddc3f3ad5fd0f456def88953723700d04ab4d19bc7f718

### Player 2 makes a move in Blockchain 2

#### Move 2: 
npx hardhat ttt-move --x 0 --y 1 --player 2 --session-id 0xbb9ae76f71906dbfbdddc3f3ad5fd0f456def88953723700d04ab4d19bc7f718 --source-blockchain avalancheFuji --sender 0x1a8110B7252d65E2C367e0B2285BE88DAe502486 --destination-blockchain ethereumSepolia --receiver 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE

✅ Message sent, you make a move! transaction hash: 0x6bd68052f564e27a248d1ae0e58fe14d42aadc12563cdd1e227def53a225ef97

#### Move 4:
npx hardhat ttt-move --x 1 --y 2 --player 2 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain avalancheFuji --sender 0x1a8110B7252d65E2C367e0B2285BE88DAe502486 --destination-blockchain ethereumSepolia --receiver 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE

#### Move 6:
npx hardhat ttt-move --x 2 --y 1 --player 2 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain avalancheFuji --sender 0x1a8110B7252d65E2C367e0B2285BE88DAe502486 --destination-blockchain ethereumSepolia --receiver 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE

#### Move 8:
npx hardhat ttt-move --x 0 --y 2 --player 2 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain avalancheFuji --sender 0x1a8110B7252d65E2C367e0B2285BE88DAe502486 --destination-blockchain ethereumSepolia --receiver 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE

### Player 1 makes a move in Blockchain 1

#### Move 1: 
npx hardhat ttt-move --x 0 --y 0 --player 1 --session-id 0xbb9ae76f71906dbfbdddc3f3ad5fd0f456def88953723700d04ab4d19bc7f718 --source-blockchain ethereumSepolia --sender 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE --destination-blockchain avalancheFuji --receiver 0x1a8110B7252d65E2C367e0B2285BE88DAe502486

✅ Message sent, you make a move! transaction hash: 0x6d281f061564e783e7f7c690eb78789051485f28e6e564e02b0c4dc36e6f6567

#### Move 3: 
npx hardhat ttt-move --x 1 --y 1 --player 1 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain ethereumSepolia --sender 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE --destination-blockchain avalancheFuji --receiver 0x1a8110B7252d65E2C367e0B2285BE88DAe502486

#### Move 5: 
npx hardhat ttt-move --x 2 --y 2 --player 1 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain ethereumSepolia --sender 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE --destination-blockchain avalancheFuji --receiver 0x1a8110B7252d65E2C367e0B2285BE88DAe502486

#### Move 7: 
npx hardhat ttt-move --x 1 --y 0 --player 1 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain ethereumSepolia --sender 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE --destination-blockchain avalancheFuji --receiver 0x1a8110B7252d65E2C367e0B2285BE88DAe502486

#### Move 9: 
npx hardhat ttt-move --x 2 --y 0 --player 1 --session-id 0x8f976a1aa42199234b93ea83ac13114e15a8d5218532fbcc2a401f540a5ddffc --source-blockchain ethereumSepolia --sender 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE --destination-blockchain avalancheFuji --receiver 0x1a8110B7252d65E2C367e0B2285BE88DAe502486

### Check the winner

npx hardhat ttt-check-winner --blockchain ethereumSepolia --contract 0x4726E37410e20C86a4DA66FdF53f419BBF4E64fE --session-id 0xbb9ae76f71906dbfbdddc3f3ad5fd0f456def88953723700d04ab4d19bc7f718 

#### winner of sessionId 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c is: 0x0000000000000000000000000000000000000000

npx hardhat ttt-check-winner --blockchain avalancheFuji --contract 0x1a8110B7252d65E2C367e0B2285BE88DAe502486 --session-id 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c

#### winner of sessionId 0xec0af7f38dbc4a1de6708f0f6b92193b17710a7f30b4a0e3d83a938f5290925c is: 0x0000000000000000000000000000000000000000
