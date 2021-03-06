# UpLeveled VS Code ESLint Shared Config

UpLeveled ESLint defaults for programming in JavaScript, React and Node.js.

<img src="screenshot.png" alt="Screenshot of errors and warnings generated by this configuration" />

## Setup

Regardless of which environment you have for your project, the first steps are to install the dependencies and add the file:

```sh
yarn add --dev eslint-plugin-cypress
```

Then create a file in the root of your project called `.eslintrc.js` and add the content of [the `.eslintrc.js` file](https://github.com/upleveled/upleveled-vscode-eslint-base-config/blob/main/.eslintrc.js).

If you are using `create-react-app`, this is enough! You're ready to go.

If your app is not using `create-react-app`, read on:

### Without `create-react-app`

If your application does not use `create-react-app` (eg. Node.js or Next.js), then you will need to also run the following command:

```sh
npx install-peerdeps --dev --yarn eslint-config-react-app
```

### Verify Setup

To verify that the configuration is working properly, you can try pasting the contents of [`__tests__/index.js`](./__tests__index.js) into a new file and seeing whether you get the same warning messages as in the screenshot at the beginning of the readme (you may need to hover over the words underlined with orange / red squiggly lines).
