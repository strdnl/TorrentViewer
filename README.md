<h1 align="center">

  <a href="https://webtorrent.io"><img src="https://www.thoughtco.com/thmb/7_rJkBY2uh3ConQe4Ks9_QYlaNY=/768x0/filters:no_upscale():max_bytes(150000):strip_icc()/george_orwell-1943-56af81233df78cf772c542f1.jpg" alt="Instant.io" width="400"></a>
  <br>
</h1>

<h4 align="center">Internet over WebTorrent (torrents on the web)</h4>

<p align="center">
  
  <a href="https://standardjs.com"><img 

Powered by [WebTorrent](http://webtorrent.io), the first torrent client that works in the
browser without plugins. WebTorrent is powered by JavaScript and WebRTC. Supports Chrome,
Firefox, Opera (desktop and Android). Run <code>localStorage.debug = '*'</code> in the
console and refresh to get detailed log output.

## Install

If you just want to do file transfer on your site, or fetch/seed files over WebTorrent, then there's no need to run a copy of instant.io on your own server. Just use the WebTorrent script directly. You can learn more at https://webtorrent.io.

The client-side code that instant.io uses is [here](https://github.com/webtorrent/instant.io/blob/master/client/index.js).

### Run a copy of this site on your own server

To get a clone of https://instant.io running on your own server, follow these instructions.

Get the code:

```
git clone https://github.com/webtorrent/instant.io
cd instant.io
npm install
```

Modify the configuration options in [`config.js`](https://github.com/webtorrent/instant.io/blob/master/config.js) to set the IP/port you want the server to listen on.

Copy [`secret/index-sample.js`](https://github.com/webtorrent/instant.io/blob/master/secret/index-sample.js) to `secret/index.js` and set the Twilio API key if you want a [NAT traversal service](https://www.twilio.com/stun-turn) (to help peers connect when behind a firewall).

To start the server, run `npm start`. That should be it!

## Mirrors

- https://torrent.partidopirata.org/
- https://instant-io.glitch.me/

## Tips

1. Create a shareable link by adding a torrent infohash or magnet link to the end
of the URL. For example: `https://instant.io#INFO_HASH` or `https://instant.io/#MAGNET_LINK`.

2. You can add multiple torrents in the same browser window.

## License

MIT. Copyright (c) [WebTorrent, LLC](https://webtorrent.io).

