# Lesson 1: Cryptography 101
If you are following along offline, check out the slides [here](https://docs.google.com/presentation/d/19xTJLwixjGnZM6NWDvdmAwhHUxCfE6p9hs40srcYKY8/edit#slide=id.g31f6a41322a_0_0).

In this lesson, the workshop has three parts.

### Part I: Install the Node
Install the Koii Node, which also doubles as a Key Management Device, visit [the Koii Website](https://koii.network/node).

To get free $KOII, you'll need to visit the Koii Faucet during the installation process. Faucets are websites that distribute tokens for testing purposes, and for onboarding new users. You'll need to authenticate with Gmail or another method. 

Make sure you get at least 10 $KOII, or ask one of the Koii Global Reps for more tokens if it doesn't work.

If you are participating online, you can always ask for tokens for development by joining the [Koii discord channel](https://discord.gg/koii-network).

### Part II: Find your Key File
Once you have the node, you can navigate to the settings tab to get access to your Key File.

It should be located at <OS-specific path>/KOII-Desktop-Node/wallets/<name>_mainSystemWallet.json.

The OS-specific paths are as follows:

Windows: /Users/<username>/AppData/Roaming

Mac: /Users/<username>/Library/Application Support

Linux: /home/<username>/.config (This path contains a dot folder that may be hidden by default. You can show hidden folders by pressing Ctrl-H)

On unix, the wallet is located at home/< your username >/.config/KOII-Desktop-Node/wallets/Laura_mainSystemWallet.json

Now, finally, open `.env` and set 
```
STAKING_WALLET_PATH="< your path >"
```

### Part III: Test Cryptography Fundamentals
Open crypto-101.js and inspect the codebase to see how it uses cryptographic primitives. 

Before you can run the sample code, you'll need to install dependancies.

```sh
yarn #installs system dependancies 
```
If this step fails, be sure to check the installation instructions in the master readme at the root of this repo.

Once the yarn install completes, you can try running the sample code with `yarn start`. 

### Part IV: Create a Token