# Merchant Onboarding UI

Implementation of the application and onboarding flow for a merchant.
Data is stored and porwered by the FoxCommerce backend API.

## Local Development

### Prerequisites

* `node` > v5.1.0

  To install this or another versions of node you can use [n](https://github.com/tj/n) or [nvm](https://github.com/creationix/nvm)

* [Flow](http://flowtype.org)

  We're using [Flow](http://flowtype.org) to perform type checks and `babel-plugin-typecheck` for same thing at runtime. Install Flow per the instructions on the website. Checkout required version in `.flowconfig` file.

* `public_key.pem` in the root of the project. This is the public key used to verify the authenticity of the JWT. See Max or Jeff for access to the key.

### Environment Variables

- `API_URL`: Location of the API to hit. Example: `https://tgt.foxcommerce.com`
- `ASHES_URL`: Admin experience to redirect to once onboarding is complete. Example: `https://tgt.foxcommerce.com/admin`

### Run the dev server

1. Run `npm i` to install dependencies.

1. Select your backend. There are convenience tasks to run the common backend development methods, hitting backend at either local or remote stage:

  `npm run dev` — backend at `http://localhost:4042`

1. Develop it at http://localhost:4042/

For **static type checking** [flowtype](http://flowtype.org/) is used. You can run check manually by `npm run flow` command.

## License

Copyright (C) 2016. FoxCommerce, Inc.
