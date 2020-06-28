# `cors-yt` 

Cloudflare workers CORS proxy for youtube-dl requests from front end.


## Deploying
Install [wrangler](https://github.com/cloudflare/wrangler)
```console
# wrangler.toml with your Cloudflare Account ID
$ wrangler config
$ wrangler publish
```
## Usage from front end
```js
fetch('<workers-url>/<youtube.com-cors-url>')
    .then(response => response.json())
    .then(data => console.log(data));
```