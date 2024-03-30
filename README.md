#Arcx

ArcX is the first product to integrate physical arcade games using blockchain technology, aiming to create the next generation of arcade culture and provide players in the Web3 metaverse with real-world experiences.

#### Resources

- [Android APK Download] - in submission
- [Sync HomePage](http://arcx.world/)
- [Sync Twitter](https://twitter.com/ArcX_games)

#### Summary of Submission Features

- Game DEMO
- Conceptional Implementation API endpoints
- Feeless peer-to-peer Listing
- Parsed Solana Metadata Store for Games
- Live on Solana Devnet
- Live on Android

#### Tech Stack

- Anchor: [Collection NFT](./programs/sync-nft) Customise NFT program for easy integration for any game
  - TypeScript: [Main API](./app/src/app/api/) Centerpiece for games interacting with the Solana blockchain
- Web3 Auth SDK: Single sign-in with Google and non-custodial signing wallet
- Solana Unity SDK: Integration Solana Wallet Connect with Unity games
- Unity: [Mobile Game]()
- NextJs: [Marketplace / API Dashboard Interface](./backend/src/circle/)
- Postgresql/Prisma: [Database](./app/prisma/) for storing indexed data, listing, and game data, also act as a cache for Solana blockchain data and metadata provider

### Present Limitations/Known Issues

- Some features currently disabled on devnet:
  - Friend Investing System
  - Fiat payment for listing purchases
  - API endpoint are more strightforward approach compare to live version

---

# Sync API Local Development

To deploy Sync API locally, you will need to set up the following:

- Anchor (isntallation instructions [here](https://www.anchor-lang.com/docs/installation))

## API / Frontend setup

- Install Node.js LTS [here](https://nodejs.org/en/download/)

### Install Dependencies

- run `npm install` in the `app` directory

### Set up Environment

- run `npm run dev` in the `app` directory


In a terminal in the project directory run `npm install`

run `npm run dev` 

### Test the programs

You must have run the setup steps already.

- To Start Solana Validator with Metaplex and Anchor programs: you will need [@metaplex/js](https://github.com/metaplex-foundation/js), clone the repo and run `yarn` && `yarn amman:start` in the repo root directory.

- Set the url to the local validator in the `.env` file.
- run `anchor test` in the sync app `root` directory

### Program Info


