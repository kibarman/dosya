source $HOME/.cargo/env
curl https://sh.rustup.rs -sSf | sh
source $HOME/.cargo/env
rustup update nightly
rustup target add wasm32-unknown-unknown --toolchain nightly
git clone https://github.com/availproject/avail.git
screen -S avail
cd avail
