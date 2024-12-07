# FractalBitcoinAuction  
Date of publication 7/12/2024 22:26

A Telegram bot for participating in The LonelyBit (TLB) NFT Auctions.

# The LonelyBit NFT Auction Bot

<p align="center"> 
  <img src="https://thelonelybit.org/images/TLB-Icon-TransBG.png" alt="The LonelyBit Logo" width="200"/>
</p>

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [User Interaction](#user-interaction)
  - [Getting Started](#getting-started)
  - [Main Menu](#main-menu)
  - [Registering Bids](#registering-bids)
  - [Viewing Current Auction Status](#viewing-current-auction-status)
  - [Placing Bids](#placing-bids)
  - [Leaderboard](#leaderboard)
  - [Checking Your Bids](#checking-your-bids)
- [Administrative Functions](#administrative-functions)
  - [Starting and Stopping Auctions](#starting-and-stopping-auctions)
  - [Notifying Users](#notifying-users)
  - [Selecting Winners](#selecting-winners)
- [Data Storage and Management](#data-storage-and-management)
- [Security Measures](#security-measures)
  - [Validating Addresses](#validating-addresses)
  - [Transaction Tracking](#transaction-tracking)
  - [Data Privacy](#data-privacy)
- [Limitations and Policies](#limitations-and-policies)
- [How to Use the Bot](#how-to-use-the-bot)
- [Conclusion](#conclusion)

---

## Introduction

**The LonelyBit NFT Auction Bot** is a Telegram-based solution that allows users to participate in NFT auctions using The LonelyBit (TLB) on BRC20 protocol as currency. Users can register their FB/TLB addresses, place bids by sending TLB tokens to a designated pool address, and track the leaderboard to see the highest bidders. Once the auction ends, the highest bidder wins the NFT, and all participants are notified of the results.

---

## Features

- **NFT Auctions**: Participate in time-limited auctions for unique NFTs.
- **TLB-Based Bidding**: Place bids using The LonelyBit (TLB) tokens.
- **Automatic Tracking**: The bot monitors TLB transactions to update user bids automatically.
- **Leaderboard**: View the top bidders at any point during the auction.
- **Notifications**: Users receive updates on their bid status, outbids, and auction outcomes.
- **Admin Controls**: Administrators can start/stop auctions, announce winners, and manage participants.

---

## User Interaction

### Getting Started

- **Start Command**: Send `/start` to register with the bot and access the main menu.
- **Help Command**: Use `/help` to view available commands and instructions.

### Main Menu

The interactive menu provides quick access to functionalities:
- **/register_bid**: Register your TLB address to start bidding.
- **/my_bids**: Check your current bid amount.
- **/leaderboard**: View the top bidders.
- **/current_bid**: See the highest bid, auction details, and how to place a bid.
- **/help**: Get help and usage instructions.

### Registering Bids

1. **Register Your Address**:  
   Use `/register_bid` and provide your valid TLB address. Once registered, you can start placing bids.

2. **Address Validation**:  
   The bot ensures the address format is correct before registering it.

### Viewing Current Auction Status

- **/current_bid**: View the current highest bid, the number of participants, and the NFT details.
- The bot also displays the auction end time, ensuring transparency and clarity.

### Placing Bids

1. **Obtain Pool Address**:  
   After registration, the bot provides a staking pool address.
   
2. **Send TLB Tokens**:  
   Transfer your desired TLB amount to the provided pool address.
   
3. **Automatic Update**:  
   The bot monitors transactions and updates your total bid automatically.  
   
4. **Outbid Alerts**:  
   If you get outbid, the bot sends you a notification, prompting you to send more TLB if you wish to remain the highest bidder.

### Leaderboard

- **/leaderboard**: Displays the top bidders along with their bid amounts.  
- Useful for monitoring your competition and strategizing your bids.

### Checking Your Bids

- **/my_bids**: Check how much TLB you’ve currently bid in the active auction.

---

## Administrative Functions

### Starting and Stopping Auctions

- **/start_auction**: Administrators can start a new auction by setting the NFT details and duration.
- **/stop_auction**: Stop an ongoing auction early if needed.

### Notifying Users

- When a new auction starts, all registered users receive a notification.
- When the auction ends, all participants are notified and the winner is declared.

### Selecting Winners

- Once the auction ends, the bot identifies the highest bidder as the winner and notifies them as well as the admin.

---

## Data Storage and Management

- **SQLite Database**:  
  Stores auction details, registered users, bids, and processed transactions.
- **Processed Transactions Table**:  
  Ensures each TLB transaction is counted only once, preventing double counting.

---

## Security Measures

### Validating Addresses

- The bot enforces strict address format checks to ensure only valid addresses are registered.

### Transaction Tracking

- **Unique Transaction IDs**: The bot uses unique transaction IDs to track which transactions have been counted, preventing bid inflation.
  
### Data Privacy

- User data (addresses, bids, and Telegram IDs) is stored securely and is not shared with unauthorized parties.

---

## Limitations and Policies

- **Auction Duration**: Auctions run for a set number of days. No late bids are accepted after the closing time.
- **No Refunds**: Bids are final. Participants should ensure they want to commit their TLB tokens.
- **Admin Discretion**: The administrator can stop auctions or enforce policies to ensure fair play.

---

## How to Use the Bot

1. **Register**: Start the bot with `/start`.
2. **Get Help**: Use `/help` to understand the features.
3. **Register Your Address**: Use `/register_bid` to register your TLB address.
4. **Place Bids**: Send TLB tokens to the pool address. Your bid updates automatically.
5. **Check Status**: Use `/my_bids` to track your personal bids, and `/leaderboard` to see where you stand.
6. **View Current Auction**: `/current_bid` provides details about the highest bid and how to increase yours.

---

## Conclusion

The LonelyBit NFT Auction Bot offers a seamless and secure way to participate in NFT auctions using BRC20 tokens. With automatic bid updates, a transparent leaderboard, and essential administrative controls, the bot provides an engaging, fair, and rewarding auction experience for all participants. Join the auction and may the highest bid win! 🚀
