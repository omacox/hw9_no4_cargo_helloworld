# hw9_No4_Cargo_Anchor_Helloworld

# New cargp project step by step:
# to run a Hello World 
# You have to have the validator from the boot camp running
# and the solana log in respective terminals 
# to see the transaction in this example
# The solana log will show the transaction 
# and the console terminal (third terminal or terminal 
# within codium) will show the Hellow World message

mkdir anchor
cd anchor
anchor init anchor_app 

cd anchor_app/programs/anchor_app/src
nano lib.rs
# on line 9 add '_' to the ctxt
ctl-x y
cd ..
cd ..
cd ..
cd anchor_app/tests 
nano anchor_app.ts
# on line 14 replace " Your transaction signature" with "Helloworld"
ctl-x y
cd ..
nano package.json
# add this to file after first "{"
"license": "MIT",
ctl-x y

# add to anchor.toml
nano anchor.toml
 [test]
startup_wait = 10000
clt-x y

# sale all changes
anchor clean
anchor build
# chech if validator is running
anchor test --skip-local-validator
# this command at the end of checking validator
# will display your anchor hellworld
sudo lsof -i :8899
sudo kill -9 <PID>

# or just run
anchor test

# Install Cargo and Hellow hellow world
mkdir cargo_app
cd cargo_app
cargo new --bin cargo_app
cd app
cargo run  

# now done with home - be safe# hw9_no4_cargo_anchor_helloworld
# hw9_no4_cargo_anchor_helloworld
# hw9_no4_cargo_anchor_helloworld
# hw9_no4_cargo_anchor_helloworld
# hw9_no4_cargo_anchor_helloworld
# hw9_no4_cargo_helloworld
# hw9_no4_cargo_helloworld
# hw9_no4_cargo_helloworld
# hw9_no4_cargo_helloworld
