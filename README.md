# Merchant Onboarding UI

Implementation of the application and onboarding flow for a merchant.
Data is stored and porwered by the FoxCommerce backend API.

## Local Development

### Prerequisites

* `node` > v5.1.0

  To install this or another versions of node you can use [n](https://github.com/tj/n) or [nvm](https://github.com/creationix/nvm)

* [Flow](http://flowtype.org)

  We're using [Flow](http://flowtype.org) to perform type checks and `babel-plugin-typecheck` for same thing at runtime. Install Flow per the instructions on the website. Checkout required version in `.flowconfig` file.

* `public_key.pem` in the root of the project, as described in the [engineering wiki](https://github.com/FoxComm/engineering-wiki/blob/master/development/setup.md#developing-frontend-applications)

### Run the dev server

1. Run `npm i` to install dependencies.

1. Select your backend. There are convenience tasks to run the common backend development methods, hitting backend at either local or remote stage:

  `npm run dev` — backend at `http://localhost:4042`

1. Develop it at http://localhost:4042/

You can set the marketplace backend API and Ashes URLs as a shell variables `API_URL` and `ASHES_URL`.

For example, to hit staging:

```
export API_URL=http://tgt.foxcommerce.com
export ASHES_URL=https://tgt.foxcommerce.com/admin
```
then run

```
npm run dev
```

For **static type checking** [flowtype](http://flowtype.org/) is used. You can run check manually by `npm run flow` command.

## License

Copyright (C) 2016. FoxCommerce, Inc.
