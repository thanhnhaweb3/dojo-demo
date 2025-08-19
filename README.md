# dojo-demo on ubuntu 25.04 (campmamo.olym3.xyz)

# 20 slot VPS Google Cloud for testing DOJO. 

Submit here: https://forms.gle/ThQ45U2SUNaNDJfp8

# Prepairing:

https://dojoengine.org/tutorials/dojo-starter

https://github.com/celestiaorg/campmamo-demos

ssh-keygen -t rsa -b 2048 -C "your@gmail.com"


sudo apt update

sudo apt install -y build-essential pkg-config libssl-dev clang llvm-dev libclang-dev

sudo apt install -y libc6-dev gcc-multilib g++-multilib

# nvm

https://github.com/nvm-sh/nvm#install--update-script

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash



# Rust & Cargo:
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

source $HOME/.cargo/env

# SOZO

https://dojoengine.org/toolchain/sozo


## Install Rust 1.79.0
rustup install 1.79.0
rustup default 1.79.0


# Clone asdf and Install Scarb (Cairo)

git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.18.0

asdf install dojo 1.5.0

source ~/.bashrc

scarb --version

# Sozo (Dojo CLI)

sudo rm -rf /tmp/*

sudo rm -rf ~/.cargo/registry

sudo rm -rf ~/.cargo/git

## Another target

mkdir -p ~/cargo-target

export CARGO_TARGET_DIR=~/cargo-target

## sozo build

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




