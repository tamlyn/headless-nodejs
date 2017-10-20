# Docker image with Chrome, Firefox and Node 8

    docker run --it -v $PWD:/tests tamlyn/headless-nodejs

This will open a bash prompt where you can `npm test` or whatever.

Start Firefox with `firefox --headless`.

Start Chrome with `google-chrome-stable --headless --disable-gpu --no-sandbox`.

Image includes `yarn`, `git` and `build-essential` required for building native NPM modules.