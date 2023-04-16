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

## Jest Unit Testing

Run Unit test:
``` 
npm run test-unit
```

### Tests
1. The login function fetches and stores a token in browser storage
2. The logout function clears the token from browser storage

## Cypress E2E Testing
Create a `cypress.env.json` in your root folder and copy the example from `cypress.env.example.json`. Change out to your own credentials.
Remeber to add `cypress.env.json` to your `.gitignore`!

Run E2E test:
``` 
npm run test
```
### Tests
1. Invalid user credentials for login.
2. Valid user credentials for login.
3. Logout user.

## Github Actions
1. `Deploy and Build`a static page on push.
2. `Unit testing` on pull_request and workflow_dispatch
3. `E2E testing` on pull_request and workflow_dispatch

Remember to add your `cypress.env.json` credentials to `secrets` in the `action` tab to run the `E2E testing`.