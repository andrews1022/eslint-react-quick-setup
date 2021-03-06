# ESLint & Babel Quick Setup Guide

## Testing

If your app uses a testing library, such as [React Testing Library](https://github.com/testing-library/react-testing-library), there is just a bit of extra setup.

First, you need to install the ESLint plugin for Testing Library and Jest-DOM:

`npm i eslint-plugin-testing-library eslint-plugin-jest-dom`

Once installation is complete, open your `package.json` file. Find the `eslintConfig` code block and remove it entirely.

Once that is done, continue with the steps listed below.

## Setup

Create an ESLint config by running:

`npx eslint --init`

Go through and answer the questions accordingly. It's recommended picking `JSON` for the file format.

You may also be asked to download additional packages, to which you should answer `Yes`.

It may also be suggested to you to run `npm audit fix` to fix any package vulnerabilities, which you should also do.

## Usage

To save yourself sometime, I've included some ESLint rules that I like to use. Of course, feel free to modify the rules to your liking!

The rules are assuming you are using TypeScript as well, so rules like `react/prop-types` are turned off. Update to your use case.
