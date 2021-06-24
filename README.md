# ESLint & Babel Quick Setup Guide

## Testing

If your app uses a testing library, such as [React Testing Library](https://github.com/testing-library/react-testing-library), there is just a bit of extra setup.

First, you need to install the ESLint plugin for Testing Library and Jest-DOM:

`npm i eslint-plugin-testing-library eslint-plugin-jest-dom`

Once installation is complete, open your `package.json` file. Find the `eslintConfig` code block and remove it entirely.

Once that is done, continue with the steps listed below.

## Setup

The easiest way to get started is by using a React boilerplate, such as [Create React App](https://github.com/facebook/create-react-app), because ESLint is included with Create React App.

Once Create React App is finished downloading, you can easily create an ESLint config by running:

`npx eslint --init`

Go through and answer the questions accordingly. It's recommended picking `JSON` for the file format.

You may also be asked to download additional packages, to which you should answer `Yes`.

It may also be suggested to you to run `npm audit fix` to fix any package vulnerabilities, which you should also do.

## Usage

To save yourself sometime, I've included 2 starter ESLint config files you can use or reference.

If your project includes tests using React Testing Library, check out the config file in the `tests` folder.

If your project does not include tests, check out the config file in the `base` directory.

Of course, feel free to modify the rules to your liking!
