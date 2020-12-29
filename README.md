# Challenge 1:
*Launch a local Substrate development chain and use the Front-End Template to make a balance transfer and make an
on-chain remark with your GitHub username.*


Submission requirements
Provide a screenshot that shows the finalized transaction.



https://github.com/aadorian/HackPolkadot.git

Solution: 

0. Clone https://github.com/substrate-developer-hub/substrate-node-template
1. Build 
2. Run `./target/release/node-template purge-chain --dev `(purging the existing chain)


4. Run the node `./target/release/node-template -l runtime=debug --dev`
 ![](https://i.imgur.com/18VTcSx.png)
5. Clone, build , Run the Substrate node frontend
https://github.com/substrate-developer-hub/substrate-front-end-template
![](https://i.imgur.com/FIUJ2tj.png)
(Note: Verify than node_modules packages are installed (via npm install or npm update))

References: https://substrate.dev/docs/en/tutorials/create-your-first-substrate-chain/interact


7. Run npm `run start `
8. ![](https://i.imgur.com/t6cSEG8.png)
9. Select in the Pallet Interactor, Extrinsic, system , remark and add the twitter account
10. Verify the block hash transaction 
![](https://i.imgur.com/Rk5iisM.png)


# Challenge 2:

Use Polkadot-JS or the Front-End Template to write a web page (hosted on GitHub pages or similar) that displays information about the latest block on Kusama, Polkadot or any other Substrate-based chain. Include a component to search for a block by number (height) and/or hash.

Submission requirements:

Provide links to your source code and deployed web page.
Resources
• Polkadot-JS API
• Substrate Front-End Template


https://github.com/aadorian/MyLastBlockCard.git
![](https://i.imgur.com/zPnwbEg.png)

# Challenge 3:

Run A Polkadot Node And Add It To Telemetry
Download the latest binary release or build Polkadot or Kusama from source, and run your node. Add it to telemetry as per the README
instructions, and let us know when your node appears in the telemetry.polkadot.io list!
Submission requirements
The node has to be on telemetry, fully synced, for at least 24 hours. The
syncing will take a while, so be patient. Pro tip: run it with the
--wasm-execution=compiled flag to quadruple sync speed!
Resources
• https://github.com/paritytech/polkadot/releases
• https://github.com/paritytech/polkadot/#connect-to-polkadot-mainnet

TODO 



# Challenge 4: FRAME Identity
Substrate-based chains which implement the Identities pallet let users of the chain set some on-chain metadata through which to identify their accounts. Kusama and Polkadot come with identities built in, but on
node-template you have to manually extend the chain. Do it. Add the identity pallet to the node template, then register an identity of an account on your local development chain.
**Submission requirements**
Register an account’s identity on your local node-template chain. Add as many fields as you want, but at least one. See resources for a full guide on how to do this on a chain which supports setting identities. Once
you’ve done this, send us a screenshot of that identity visible in Polkadot
JS Apps connected to your local chain. Important: Make sure the fields
clearly show a value through which we can contact you. E.g. the twitter
field should have a valid twitter username, or the email field should have
a valid email. We’ll use this to get in touch with you, so if you don’t have
this info in your account’s identity, we can’t verify the completion of the
task!

Resources
• Polkadot Wiki: Identity
• https://github.com/paritytech/polkadot/releases
• PolkadotJS Apps
• FRAME Identity Module
• Rust docs: Identity Module
• Substrate Node Template
• How to add a FRAME pallet to a Substrate Node
Set  on chain identity 

Ref: https://substrate.dev/docs/en/tutorials/add-a-pallet/import-a-pallet


![](https://i.imgur.com/pto20vb.png)

# Challenge 5: FRAME Multisig

Add the Multisig pallet to the Node Template and create a Polkadot-JS script to make a multisig transaction. Use the Front-End Template to create a multisig UI component.
Submission requirements
Provide a link to your GitHub repository and a screenshot of your multisig UI component.
**Resources**
• FRAME Multisig pallet
• Substrate Node Template
• Polkadot-JS API
• How to add a FRAME pallet to a Substrate node


1. Cargo.toml 
`[dependencies] ...pallet-multisig = { default-features = false, version = '2.0.0' }..`

`  std = [...'pallet-multisig/std',..]`
2