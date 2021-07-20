# CONFIGURANDO ESLINT y PRETTIER
- Acceso a vídeo  [configurando ESLINT y PRETTIER](https://www.youtube.com/watch?v=EEDRcolSHms).
## ESLINT

- Instalar dependencia de esLint (7.00)
  - Sitio oficial eslint  [eslint](https://eslint.org/).
  - Ejecutar: npm i -D eslint
- Configurar esLint (7.15)
  - Ejecutar: npx eslint --init
	  - How would you like to use ESLint?
	    - To check syntax, find problems, and enforce code style
    - What type of mudules does your project use?
	    - JavaScript modules (import/export)
    - Which framework does your project use?
	    - React
    - Does your project use TypeScript?
	    - No
    - Where does your code run?
	    - Presionar a para TODOS.
    - How would you like to define a style for your project?
	    - Use a popular style guide
	      - Standard: https://github.com/standard/standard
    - What format do you want your config file to be in?
	    - JavaScript
    - Would you like to install them now with npm?
	    - Yes
  - Instalar extension de ESLINT (14.15)
	  - ESLint de Dirk Baeumer (dbaeumer.vscode-eslint)
  - Buscar problemas (14.58)
	  - Ejecutar: npx eslint .
	  - O ejecutar: ./node_modules/.bin/eslint .
  - Reparar problemas (15.30)
	  - Ejecutar: npx eslint . --fix
	  - O ejecutar: ./node_modules/.bin/eslint . --fix

## PRETTIER

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
