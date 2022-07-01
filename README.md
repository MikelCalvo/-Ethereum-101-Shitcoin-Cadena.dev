# 💸 GorotzCoin Shitcoin Project -> [https://gorotzcoin.vercel.app/](https://gorotzcoin.vercel.app/) 💸

Rinkeby Shitcoin that duplicates the ammount sent in every transaction. [(Example)](https://rinkeby.etherscan.io/tx/0xd2d12b03e264a311673f58c6560c11b5839813f16b105bed109a91a158d05e66)

How many coins can we make?

This website is part of the course Ethereum 101 from [cadena.dev](https://cadena.dev)

## Screenshots

- Coin Management Layout

![Deployer Layout](https://raw.githubusercontent.com/MikelCalvo/Ethereum-101-GorotzCoin-Cadena.dev/master/screenshots/coin_deployer_lowres.png)

- User Layout

![Deployer Layout](https://raw.githubusercontent.com/MikelCalvo/Ethereum-101-GorotzCoin-Cadena.dev/master/screenshots/user_lowres.png)

## Installation

Install dependencies with npm

```bash
  npm install
```

Create a .env file in the root directory with the following variables:

```
POKT_RINKEBY_URL=https://....
RINKEBY_PRIVATE_KEY=000000....
```

POKT_RINKEBY_URL is your [POKT Rinkeby app endpoint](https://mainnet.portal.pokt.network/#/).

RINKEBY_PRIVATE_KEY is your ETH private key to deploy the coin contract into rinkeby.

## Contract Compilation & Deployment

You can compile the coin contract using the following command:

```
npx hardhat compile
```

And then you have to deploy it to the Rinkeby network using:

```
npx hardhat run scripts/deploy.js --network rinkeby
```

You should see the following message as a result:

```
GorotzCoin deployed to: 0x86cc78EfA4C11325dB5D89483b86250d08c3AaDA
GorotzCoin owner address: 0x7Ed4D8f4195da9993b66600F0f2DeA420FB42978
```

Copy the contract address and paste it into webapp/src/App.js:21

## Frontend Local Deployment

To create a local instance of the frontend, cd into webapp and use the following command

```
cd webapp
npm start
```

## go to [http://localhost:3000/](http://localhost:3000/) & you should see your webapp.

by mikelcalvo.eth
