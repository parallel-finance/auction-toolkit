# Auction toolkit

This repo is store the static sources for auction.

## Usage

Use [jsDeliver](https://github.com/jsdelivr/jsdelivr#github) to get the resource from github.

e.g.

- https://cdn.jsdelivr.net/gh/parallel-finance/auction-toolkit@v1.0.0/crowdloans/project/polkadot.json
- https://cdn.jsdelivr.net/gh/parallel-finance/auction-toolkit@latest/crowdloans/project/polkadot.json
- https://cdn.jsdelivr.net/gh/parallel-finance/auction-toolkit@main/crowdloans/project/polkadot.json

### Before release new version

- After merge the changes, please use auction dapp dev environment or staging environment to check if everything goes well.
  - dev: https://crowdloan-dev.parallel.fi
  - staging: https://crowdloan-staging.parallel.fi

### How to release a new version

Since jsDeliver has their own [caching logic](https://github.com/jsdelivr/jsdelivr#caching), so we cannot use the url directly when you merge the new changes into main branch.

What we need to do after merging the new changes.

- Create a tag for main branch with the new changes
- Release the tag
- There is a github action to purge cache automatically, please using [latest url](https://cdn.jsdelivr.net/gh/parallel-finance/auction-toolkit@latest/crowdloans/project/polkadot.json) to check the changes after action is completed.

#### Notes

We created a github action for purge the caching of cdn. But if it doesn't work after release in few minutes. You can try to manually purge the caching.
Call `https://purge.jsdelivr.net/gh/parallel-finance/auction-toolkit@latest/crowdloans/rewards/polkadot.json` in browser, you can change the file name that you want to clear the cache.

## Resource

### Crowdloan projects

We should update the `/crowdloans` information based on [fearless-utils](https://github.com/soramitsu/fearless-utils) update, please note update the images url to our own images url. You can download the images into our repo, and update the url.

### Icons

For the icons of parachain or token, you can find it from [polkadot.js app](https://github.com/polkadot-js/apps/tree/master/packages/apps-config/src/ui/logos)
