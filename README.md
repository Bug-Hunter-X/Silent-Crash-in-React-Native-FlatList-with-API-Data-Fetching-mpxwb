# Silent Crash in React Native FlatList with API Data Fetching

This repository demonstrates a subtle bug in a React Native application that uses `FlatList` to display data fetched from a remote API.  The app crashes silently, without providing helpful error messages in the console, making debugging a challenge.  The issue arises from an unhandled promise rejection within the data fetching process. 

## Reproduction

1. Clone the repository.
2. Run `npm install` or `yarn install`.
3. Run the app using a React Native simulator or device.
4. Observe that the app crashes silently (without console errors) upon loading.

## Solution

The solution involves properly handling potential errors during the API fetch and providing appropriate feedback to the user.  The solution is shown in `bugSolution.js`