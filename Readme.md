# Docker image with headless Chrome, Firefox and Node 8

Ideal for running end-to-end integration tests in CI.

    docker run --itv $PWD:/tests tamlyn/headless-nodejs

This will open a bash prompt where you can `npm install && npm test` or whatever.

## Browsers

Start Firefox with `firefox --headless`.

Start Chrome with `google-chrome --headless --disable-gpu --no-sandbox`.

### Warning

Headless Chrome currently requires the `--no-sandbox` flag in order to run in a container. 
This is potentially unsafe so you should not use it on untrusted sites. 

## Other software

Image includes `yarn`, `git` and `build-essential` required for building native NPM modules.
