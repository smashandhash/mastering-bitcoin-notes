# Chapter 1: Introduction

## Bitcoin users communicate with each other using the Bitcoin protocol primarily via the internet, although other transport networks can also be used.

<p>What it means Bitcoin users communicate with each other from Bitcoin protocol is how user's transaction is broadcasted to other users via the Bitcoin node, that follows the rules from the Bitcoin protocol. The way users broadcast it has a various way to do it, mostly using internet, and some doesn't, like how Blockstream uses a satellite to run a Bitcoin node at the moon.</p>

## The Bitcoin protocol stack, available as open source software, can be run on a wide range of computing devices, including laptops and smartphones, making the technology easily accessible.

<p>At first, I thought he's only talk about the Bitcoin node. Turns out he talks about the whole ecosystem on the Bitcoin network, like running a hot wallet on a computer like Sparrow, or at a smartphone like Aqua Wallet, or running a cold wallet with a Raspberry Pi like how SeedSigner do.</p>

## Units of bitcoin are created through a process called "mining," which involves repeatedly performing a computational task that references a list of recent Bitcoin transactions.

<p>The bitcoin's total supply is fixed to 21 million coins, but it gradually released by the miners, especially when one of them successfully solved the Proof-of-Work puzzle. So, miners not only creating a new block of transaction, but it also runs a Bitcoin node too, so they can check whether the given transaction is valid or not, based on the consensus rules from the Bitcoin protocol.</p>

<p>Here's what I need to remember. A node runner running a Bitcoin node, so each transaction using their node is valid, while the miners do the same thing as the node runner, but also adds a new transaction block and given a reward for it.</p>

## Previously, the double-spend problem was a weakness of digital currency and was addressed by clearing all transactions through a central clearinghouse.

<p>Clearinghouse is traditionally controlled by a single source, either it's a bank, or a digital service like PayPal. The downside of the centralized and doesn't show how they do with our money is hideous, where they have a right to do with our money, either they manipulate it, or lend it to someone else, meaning they're not actually holding our money.</p>

<p>In Bitcoin network, people who runs the node are the one who hold the ledger from the first transaction until the latest one. So, by doing this, there's no double-spending, decentralized, and scammers aren't able to manipulate the data, unless there's 51% people doing the same thing.</p>

## Running on general-use operating systems such as Windows and macOS has certain security disadvantages, however, as these platforms are often insecure and poorly configured.

<p>It's called insecure due to the desktop we use isn't mainly used as a bitcoin wallet only, but rather doing something else. This can attracts unwanted things, like virus from downloading files from source that you can't verify whether it's safe or not, or you may had other apps that has an access through your file.</p>

<p>The author states poorly configured desktop wallet is generally sees user store their seed phrase on the same hard drive, this may encounter worst scenario like failing hard drive that causes stored coin lost forever. If your wallet is unencrypted, it can get exploited remotely, where hackers can access your computer and accessing your wallet.</p>

<p>If you're using Sparrow desktop wallet, it's best to set the wallet's password, so your seedphrase isn't exposed and encrypted. If you do it, try to check the file on this directory if you're on MacOS `~/{ username }/.sparrow/wallets`.</p>

<p>If you're seeing a file named with the assigned wallet's name when you're setting up the wallet, you can see the file is formatted with extension named `.mv.db`. If you open it with a TextEdit application, the text starts with saying `H2encrypt`, and the rest until the end of the line is unreadable.</p>

<p>But, do note if someone else knows your password, they're able to see your seedphrase. So, to harden up your defense, you should set a passphrase, to make someone else unable to access your wallet.</p>