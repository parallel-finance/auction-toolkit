# Auction toolkit

This repo is store the static sources for auction.

## Usage

Use [jsDeliver](https://github.com/jsdelivr/jsdelivr#github) to get the resource from github.

e.g.

* https://cdn.jsdelivr.net/gh/parallel-finance/auction-toolkit@v1.0.0/crowdloans/polkadot.json

### How to use a new version

Since jsDeliver has their own [caching logic](https://github.com/jsdelivr/jsdelivr#caching), so we cannot use the url directly when you push a new changes into branch.

What we need to do after pushing the new changes.

* Create a tag for the new changes
* Release the tag
* Update the usage with new version. e.g. https://cdn.jsdelivr.net/gh/parallel-finance/auction-toolkit@{new-version}/crowdloans/polkadot.json

## Resource
### Crowdloan projects

We should update the `/crowdloans` information based on [fearless-utils](https://github.com/soramitsu/fearless-utils) update, please note update the images url to our own images url. You can download the images into our repo, and update the url.

### Icons

For the icons of parachain or token, you can find it from [polkadot.js app](https://github.com/polkadot-js/apps/tree/master/packages/apps-config/src/ui/logos)
