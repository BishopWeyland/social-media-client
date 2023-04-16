[![Deploy static content to Pages](https://github.com/BishopWeyland/social-media-client/actions/workflows/pages.yml/badge.svg)](https://github.com/BishopWeyland/social-media-client/actions/workflows/pages.yml)
[![Unit Testing](https://github.com/BishopWeyland/social-media-client/actions/workflows/unit-test.yml/badge.svg)](https://github.com/BishopWeyland/social-media-client/actions/workflows/unit-test.yml)
[![Run E2E Testing](https://github.com/BishopWeyland/social-media-client/actions/workflows/e2e-test.yml/badge.svg)](https://github.com/BishopWeyland/social-media-client/actions/workflows/e2e-test.yml)

# Social Media Client - Noroff Workflow CA


## Getting Started

1. Clone the repo
   ```sh
   git clone https://github.com/BishopWeyland/social-media-client.git
   ```
2. Install NPM packages
   ```sh
   npm install
   ```

## Prettier and ESlint

Prettier and ESlint is configured to run on pre-commits in the .git/hooks folder.

## Branch Protection rules

1. Require a pull request before merging 
2. Require approvals 
3. Require status checks to pass before merging 
4. Require conversation resolution before merging
5. Do not allow bypassing the above settings

## Cypress E2E Testing
Create a `cypress.env.json` in your root folder and copy the example from `cypress.env.example.json`. Change out to your own credentials.
Remeber to add `cypress.env.json` to your `.gitignore`!

Run E2E test:
``` 
npm run test
```