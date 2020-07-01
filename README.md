# Minimal popup login Auth0.js sample

## Prerequisites

Node.js, was tested in v12.7.0

## Setup

1. Create an SPA application in Auth0
   - Add `http://localhost:3000/callback` to "Allowed Callback URLs"
   - Under "Advanced Settings -> Grant Types", make sure "Implicit" is enabled - this is needed only for testing purposes.
2. Install all dependencies in the sample folder `npm install`
3. Prepare the configuration:
   - Make a copy of the `auth_config.json.example` file and name it `auth_config.json`
   - Write there the Client ID and Auth0 Domain for the newly created app in step 1

## Running

`npm run dev` (or `npm run start`)

## Expected behaviour

1. On page load, a button is displayed "login".
2. Click the button - a popup should open with the Auth0 Universal Login.
3. After successful login, the popup should close and page's console should display the login result which includes an ID Token.

Errors should be displayed in an alert box.

## Troubleshooting

- Check Auth0 tenant logs
- Check the page console in browser dev tools
- Check the popup console in browser dev tools
