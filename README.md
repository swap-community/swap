# Swap

Copyright (c) 2014-2019 The Monero Project.   
Swap (previously known as Freehaven) is based on [Monero](README_original.md)

![Build-Linux](https://github.com/swap-dev/swap/workflows/Build-Linux/badge.svg)

## Production & Development

Active Branches:
- Stable: master(latest/release)
- Unstable: swap-v3.2dev(latest)
- Testing: N/A

To contribute to the Swap Project, please make all pull requests to the _swap-v3.2dev_ branch.<br/>
For production, please use the _latest or tagged release_ of the _master_ branch.

## Resources
- Webpage: [swap.foundation](https://swap.foundation)
- Explorer: [explorer.swap.foundation](https://explorer.swap.foundation)
- Pool List: [miningpoolstats.stream/swap](https://miningpoolstats.stream/swap)
- GitHub: [https://github.com/swap-community](https://github.com/swap-community)

## Social/Contact

- Discord: [https://discord.gg/VdbtGJNtzc](https://discord.gg/VdbtGJNtzc)

## Specifications & Emission

- Coin ticker: XWP
- Total supply: 18,400,000 coins before tail emission
- Tail emission: ~158,000 coins each year (starting at year 8)
- Decimal places: 12
- PoW hash algorithm: Cuckaroo29s (GPU only)
- Block time: 15 seconds
- Difficulty Adjustment Algorithm: Monero DAA
- Genesis block: 2018-11-16 (November 16, 2018) at 09:06:03 (UTC)
- Premine: No
- Developer fee: No
- Founders reward: No
- Mainnet default P2P port: 19949
- Mainnet default RPC port: 19950


## Build on linux

install deps:

`sudo apt-get install build-essential cmake pkg-config libboost-all-dev libssl-dev libzmq3-dev libunbound-dev libsodium-dev libreadline6-dev libpgm-dev libnorm-dev`

clone repo:

`git clone --recursive https://github.com/swap-dev/swap`

build daemon and wallet:

`cd swap && mkdir build && cd build && cmake .. && make daemon simplewallet`

or build everything:

`cd swap && mkdir build && cd build && cmake .. && make`

## Build on Windows (using MinGW)

install deps:

`pacman -S mingw-w64-x86_64-toolchain make mingw-w64-x86_64-cmake mingw-w64-x86_64-boost mingw-w64-x86_64-openssl mingw-w64-x86_64-zeromq mingw-w64-x86_64-libsodium mingw-w64-x86_64-hidapi`

clone repo:

`git clone --recursive https://github.com/swap-dev/swap`

build daemon and wallet:

`cd swap && make release-static-win64`

