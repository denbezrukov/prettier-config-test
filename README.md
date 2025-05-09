# prettier-config-test

## Description

This project is a simple monorepo setup with Prettier for code formatting. It contains two packages: `format` and `app`. The `format` package includes Prettier as a dependency, while the `app` package contains a simple JavaScript file.

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/denbezrukov/prettier-config-test.git
   cd prettier-config-test
   ```

2. Install dependencies for both packages:
   ```
   cd packages/format
   npm install
   cd ../app
   npm install
   ```

## Usage

1. To format the code in the `app` package, run the following command from the root of the monorepo:
   ```
   npx prettier --write packages/app/index.js
   ```

2. You can also add a script to the `app` package's `package.json` to format the code:
   ```json
   "scripts": {
     "format": "prettier --write index.js"
   }
   ```

   Then, you can run the script from the `app` package directory:
   ```
   npm run format
   ```
