## Project Description

This is a cronjob written in Node.js to get data for a crypto dashboard I wrote. The purpose of this cron is to get the exchange rates for Euro/Zar and USD/Zar every hour to calculate bitcoin and ethereum prices at certain times. This cron was written for the following project repos:<br/>
[crypto-dashboard](https://github.com/EstianD/crypto-dashboard)<br/>
[crypto-api](https://github.com/EstianD/crypto-api)<br/> [cryptoCron](https://github.com/EstianD/crypto-cron-no-express)<br/>
This cron uses PM2 process manager to run every hour.

## Running the App

### `npm install`

Installs dependancies for app.

### `Add .env file`

MONGODB_URI=mongodb://localhost:27017/crypto-db<br/>
USDZARLINK=https://www.alphavantage.co/query?function=CURRENCY_EXCHANGE_RATE&from_currency=USD&to_currency=ZAR&apikey=PUE3PZ1B5KZATT8E<br/>
EURZARLINK=https://www.alphavantage.co/query?function=CURRENCY_EXCHANGE_RATE&from_currency=EUR&to_currency=ZAR&apikey=PUE3PZ1B5KZATT8E<br/>
PORT=3000

## Scripts

In the project directory:

### `npm run start`

Runs the app in the production mode.
