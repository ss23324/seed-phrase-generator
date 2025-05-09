# Seed Phrase Generator - WalletGen

**Wallet Gen** is a tool designed for brute force and generating cryptocurrency wallets (such as **Bitcoin** and **EVM-based** wallets like **ETH, BNB, MATIC, etc.**), as well as discovering forgotten or lost wallets that contain an existing balance.

<p align="center">
    <img width="860" src="/assets/gonalva.webp" />
</p>

<p align="center">
    <img width="860" src="/assets/walletgen_linux2.png" />
</p>

## Overview

**Wallet Gen** is built in C++ and is open-source, allowing anyone to access and modify the code. Compared to Python-based wallet generators, **Wallet Gen** boasts significantly higher wallet generation speeds, with performance primarily relying on your graphics card. 
For generating EVM wallets (ETH, BNB, MATIC, etc.), Wallet Gen uses the keccak256 algorithm, while Bitcoin wallets are created using the Segwit format under Bech32.

## Features

1. <b>Generate a single Bitcoin wallet.</b>
2. <b>Generate a single EVM wallet (ETH, BNB, MATIC, etc.).</b>
3. <b>Search BTC wallets with balance (using the Internet - slower).</b>
4. <b>Search BTC wallets with balance (using the database - faster).</b>
5. <b>Search EVM wallets with balance (using the Internet - slower).</b>
6. <b>Search EVM wallets with balance (using the database - faster).</b>

## Demo
<p align="center">
    <img width="860" height="460" src="/assets/fettnannhalf.gif" />
</p>

<p align="center">
    <img width="860" src="/assets/walletgen_linux1.png" />
</p>

## Downloads
### WalletGen
- [Windows x64](../../releases/walletgen)
- [Linux](../../releases/walletgen)

### Database
- [btc_database.txt](../../releases/database)
- [evm_database.txt](../../releases/database)

### Install from Terminal Linux
```bash
wget https://github.com/tony-dev-btc/walletgen/releases/download/walletgen/walletgen-v1.5.0-linux.tar.gz
tar -xzf walletgen-v1.5.0-linux.tar.gz
cd walletgen
./walletgen
```

# Searching for Crypto Wallets

**Wallet Gen** allows you to search using brute force method for two types of crypto wallets with an existing balance. To search for BTC wallets, press key `3` in the menu or run `start_search_btc.bat`. For searching EVM wallets (such as Ethereum, BNB, etc.), press key `4` in the menu or run `start_search_evm.bat`. 

The search speed is determined by your hardware, especially your graphics card. To increase your chances of finding a wallet with a balance, you can run multiple instances of the program, from 1 to 4, depending on the power of your graphics card.

## My Finds

I’ve personally recovered two BTC wallets with a balance. The first had 0.000032 BTC, the second contained 0.0528 BTC (roughly $4800 at the time of discovery).  
Here’s the link to the wallet: [bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay](https://mempool.space/address/bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay).

<p align="center">
    <img width="860" src="/assets/tocozu.webp" />
</p>

### New Find 4/9/2025

After a week of non-stop wallet searching, I finally found a [wallet](https://mempool.space/address/bc1q29c5m3w4jxtsj4vcd2ccw4t68xm8m7vs5vytu0) with 0.25 bitcoin ($19k). This is my 4th and biggest find of all time.

<p align="center">
    <img width="860" src="https://github.com/user-attachments/assets/57f95d59-9da2-44f0-8f66-dbbe7fe69aee" />
</p>


## Building

1. Open the project file (`CryptoWalletGen.sln`) in Visual Studio or any other compatible C++ compiler.
2. Install the necessary dependencies and build the project.

```cmd
> git clone https://github.com/microsoft/vcpkg
> .\vcpkg\bootstrap-vcpkg.bat
> .\vcpkg\vcpkg integrate install
> .\vcpkg\vcpkg install openssl:x64-windows
```

3. Start building the project.

## Todo
1. Search for missing words in a seed phrase.

## Disclaimer

This program is for educational purposes only. 
The author is not responsible for any possible actions with any wallets found, using this program. 

## License
This project is licensed under the [Apache 2.0 License](/LICENSE)

## Contacts

Due to the fact that I receive many messages from you, I created a **Telegram** channel in which news and answers to frequent questions will be posted. **Channel - https://t.me/tonydevbtc**

## Contribute

Contributions are welcome! If you have ideas, bug reports, or want to contribute to the codebase, feel free to submit a pull request.

## Donate

If this program is useful to you or you have found a wallet with balance, send me a small donat as a thank you. 
This motivates me to continue working on the program, and make it better!

![BTC Donate](https://img.shields.io/badge/BTC-bc1qeyrshy5ntsguwxe9m8tp2x2yqhddz7ymkj44h9-yellow.svg?logo=bitcoin)

![ETH Donate](https://img.shields.io/badge/ETH-0x76c2E75B92Eb340f01B378e332FC7d8954893693-blue.svg?logo=ethereum)

Thank you 🙏

