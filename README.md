# tobalaba-nonauthority-node for local development

I usually connect to different blockchains from my development machine and prefer to modify the default member.toml to place the particular blockchain data into specific directories. Please modify member.toml to your preferred directories.

## Steps to install parity from source
-  Install rust on your machine
```
brew install rust
```
-  Make sure you have the latest rust compiler by running 
```
rustup update stable
```
-  Clone the parity code on your local machine
```
git clone https://github.com/paritytech/parity.git
```
- cd into the parity codebase and compile the code with the command below. This should create your parity binary in the target/release directory
```
cargo build --release
```

## Setup member.toml
-  Modify chain, base_path, db_path, keys_path, path, log_file in member.toml according to your preference. My preference is to create a directory called ewf in my home directory and place everything there.

## Starting the node
Start the node with the command below. Please modify the path to the member.toml file based on where you placed it.
```
./target/release/parity --config ~/ewf/member.toml
```
## Connecting to the UI
Once the node is started connect to the UI with the generated URL from the command below. Please modify the path to the member.toml file based on where you placed it.
```
./target/release/parity --config ~/ewf/member.toml signer new-token
```
