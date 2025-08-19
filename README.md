# dojo-demo on ubuntu 25.04

sudo apt install git-lfs # or use your package manager
git lfs install        # run once

# install toolchain
curl -L https://install.dojoengine.org | bash          # installs dojoup

source /home/<path-to-your-app>

dojoup install

dojoup use 1.5.0                                       # cairo, scarb, sozo, katana, torii

git clone <repo>
cd whack-a-mole-dojo/backend

# fetch deps & compile
scarb fetch
sozo build

# one-shot dev node + deploy + indexer
sozo dev   # ⏳ keep terminal open




