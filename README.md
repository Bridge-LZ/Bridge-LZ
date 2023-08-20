# 🌉 $BRIDGE

The first shitcoin omnichain with multiple functionality thanks to [@LayerZero_Labs](https://twitter.com/LayerZero_Labs). 
1:1 with gas chain, 5% fee max like on this jpeg. [$BRIDGE]() is the best way to move fund from one chain to another. [$BRIDGE]() is simply a P2P way to move fund from one chain to another.
<br>
<br>
This project use OpenZeppelin contract + LayerZero OFT contract.
<br>



## 🤓 How it works ?

1. First you neeed to mint new [$BRIDGE](). For this go to the contract link bellow and call the function `createToken()`, number [F6 (link to Base)](https://basescan.org/token/0x233dc79f924c35acb4524bac4a883c8ce11a75b2#writeContract#F6), and enter the amount of token to create. Remember, you  will receive 1:1 [$BRIDGE]() with gas chain spend, less fee. 


2. To move your fund from one chain to another, you need to call the function `sendFrom()` number [F15 (link to Base)](https://basescan.org/token/0x233dc79f924c35acb4524bac4a883c8ce11a75b2#writeContract#F15). And complete the data as follows :
   - `sendFrom` : Some Ether to pay the fee of LayerZero tx, 0.01 ETH is enough. If you put more than required you will be refunded.
   - `address _from` : Your address
   - `uint16 _dstChainId` : The chainId of the recipient chain, you can find this info on LayerZero documenation [link](https://layerzero.gitbook.io/docs/technical-reference/mainnet/supported-chain-ids). For example for Linea it's 183.
   - `bytes32 _toAddress` : The address of the recipient in bytes32. To have the address in bytes32 you can use [https://playground.ethers.org](https://playground.ethers.org) and write `utils.defaultAbiCoder.encode(["address"], ["YOUR _ADDRESS"])`
   - `uint256 _amount` : The amount of token you want to send in 10^18.
   - `tupe _callParams` : `["YOUR_ADDRESS","0x000000000000000000000000000000000000dEaD","0x"]`
 

3. Wait for the transaction to be mined, then wait for LayerZero to send [$BRIDGE]() to the chain you request. You can follow the progress by going to [https://layerzeroscan.com/](https://layerzeroscan.com/) and enter your hash transaction.


4. Once you receive your [$BRIDGE]() on the other chain call `burnToken` number [F2 (here example for Base)](https://lineascan.build/address/0x233dc79F924c35AcB4524BaC4A883c8CE11A75B2#writeContract#F2)  with the number of [$BRIDGE]() to burn `uint256 _amount`. Once transaction minted you will receive 1:1 gas chain with the token burn.

## 🗳️ Last proposal
- Change the fee, now it's 2% : [https://twitter.com/Bridge_LZ/status/1693265690772345185](https://twitter.com/Bridge_LZ/status/1693265690772345185)

## ℹ️ Useful link

- Twitter : [https://www.twitter.com/bridge_lz](https://www.twitter.com/bridge_lz)
- Telegram Group : [https://t.me/bridge_lz](https://t.me/bridge_lz)
- DefiLlama : [https://www.defillama.com/protocol/bridge_lz](https://www.defillama.com/protocol/bridge_lz)
- Ethereum Contract Address : [https://etherscan.io/address/0x233dc79F924c35AcB4524BaC4A883c8CE11A75B2](https://etherscan.io/address/0x233dc79F924c35AcB4524BaC4A883c8CE11A75B2)
- Base Contract Address :  [https://basescan.org/address/0x233dc79F924c35AcB4524BaC4A883c8CE11A75B2](https://basescan.org/address/0x233dc79F924c35AcB4524BaC4A883c8CE11A75B2)
- Linea Contract Address :  [https://lineascan.build/address/0x233dc79F924c35AcB4524BaC4A883c8CE11A75B2](https://lineascan.build/address/0x233dc79F924c35AcB4524BaC4A883c8CE11A75B2)
- Optimism Contract Address :  [https://optimistic.etherscan.io/address/0x233dc79F924c35AcB4524BaC4A883c8CE11A75B2](https://optimistic.etherscan.io/address/0x233dc79F924c35AcB4524BaC4A883c8CE11A75B2)
- Twitter link on how to mint [$BRIDGE]() : [https://twitter.com/Bridge_LZ/status/1688941241654747136](https://twitter.com/Bridge_LZ/status/1688941241654747136)

## 📣 Important Announcement 

- 2023-08-14 : [$BRIDGE]() is looking for someone to create a front-end. Fee will share with the dev. Contact us on Telegram or Twitter if you are interested [https://twitter.com/Bridge_LZ/status/1690889507187417089](https://twitter.com/Bridge_LZ/status/1690889507187417089)
- 2023-08-15 : [$BRIDGE]() as open a [Friend.tech](https://www.friend.tech/) account and some synergy will be create with [Friend.tech](https://www.friend.tech/) collector and [$BRIDGE]() fee. [link 1](https://twitter.com/Bridge_LZ/status/1692324217025347944), [link 2 with reference code](https://twitter.com/Bridge_LZ/status/1692865556272078869) 
