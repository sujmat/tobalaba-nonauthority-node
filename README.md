# tobalaba-nonauthority-node

I usually connect to different blockchains from my development machine and prefer to modify the default member.toml to place the particular blockchain data into specific directories. Please modify member.toml to your preferred directories.

## Steps to install
-  Install the latest parity client on your mac/linux machine
-  Modify chain, base_path, db_path, keys_path, path, log_file according to your preference. My preference is to create a directory called ewf in my home directory and place everything there.

## Starting the node
Start the node with the command below. Please modify the path to the member.toml file based on where you placed it.
```
parity --config ~/ewf/member.toml
```
## Connecting to the UI
Once the node is started connect to the UI with the generated URL from the command below. Please modify the path to the member.toml file based on where you placed it.
```
parity --config ~/ewf/member.toml signer new-token
```
