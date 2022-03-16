# Auction toolkit

This repo is store the static sources for auction.

## Usage

Use S3 bucket to store all the resource for crowdloan.

e.g.

- https://auction-us-east-2.s3.us-east-2.amazonaws.com/crowdloans/projects/polkadot.json

### Before release new version

- After merge the changes, please use auction dapp dev environment or staging environment to check if everything goes well.
  - dev: https://crowdloan-dev.parallel.fi
  - staging: https://crowdloan-staging.parallel.fi

### How to release a new version

What we need to do after merging the new changes.

- Go to [production deployment action](https://github.com/parallel-finance/auction-toolkit/actions/workflows/production-deploy.yml), click `Run workflow` dropdown, make sure the branch selection is `main`, then click confirmed button. 
- After the action finished, please using the following urls to check the changes after action is completed. 
  - https://auction-us-east-2.s3.us-east-2.amazonaws.com/crowdloans/projects/polkadot.json
  - https://auction-us-east-2.s3.us-east-2.amazonaws.com/crowdloans/projects/kusama.json
  - https://auction-us-east-2.s3.us-east-2.amazonaws.com/crowdloans/rewards/polkadot.json
  - https://auction-us-east-2.s3.us-east-2.amazonaws.com/crowdloans/rewards/kusama.json

## Resource

### Crowdloan projects

We should update the `/crowdloans` information based on [fearless-utils](https://github.com/soramitsu/fearless-utils) update, please note update the images url to our own images url. You can download the images into our repo, and update the url.

### Icons

For the icons of parachain or token, you can find it from [polkadot.js app](https://github.com/polkadot-js/apps/tree/master/packages/apps-config/src/ui/logos)
