# Web Monetization Torrent App

## Install and build

```
$ npm install
$ npm run build
```

## Configuration

Bittorrent tracker endpoint, to change in `static/js/config.js`
```js
module.exports = {
  tracker: 'ws://localhost:8000'
}
```

## Run

Requirements:
* running ILP bittorrent tracker
* running SPSP server that supports STREAM receipts
* running receipt verifier

Run:
* user a server of your choice to start the app, e.g. python server
```
$ cd build/
$ python3 -m http.server 3003
```
Then navigate to `http://localhost:3003`. 