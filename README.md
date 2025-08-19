# dojo-demo on ubuntu 25.04

sudo apt update

sudo apt install -y pkg-config libssl-dev build-essential curl git

# Rust & Cargo:
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

source $HOME/.cargo/env


# Scarb
curl -L https://github.com/software-mansion/scarb/releases/latest/download/scarb-installer.sh | bash

scarb --version

# Sozo (Dojo CLI)

cargo install --locked sozo --git https://github.com/dojoengine/dojo.git --tag v0.7.0

sozo --version

# LFS

sudo apt install git-lfs # or use your package manager

git lfs install        # run once

# install toolchain

curl -L https://install.dojoengine.org | bash          # installs dojoup


source /home/<=path-to-your-app=>


dojoup install


dojoup use 1.6.2                                       # cairo, scarb, sozo, katana, torii


git clone https://github.com/gbarros/dojo-demo


cd dojo-demo/dojo-backend


# fetch deps & compile

scarb fetch

sozo build

# one-shot dev node + deploy + indexer
sozo dev   # ⏳ keep terminal open




