# CONFIGURANDO ESLINT y PRETTIER

- Acceso a vídeo [configurando ESLINT y PRETTIER](https://www.youtube.com/watch?v=EEDRcolSHms).

## ESLINT

- Instalar dependencia de esLint (7.00)
  - Sitio oficial [eslint](https://eslint.org/).
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
  - Crear script en package.json (16.45)
    - "lint": "eslint . --fix",
  - Configurar settings.json (17.50)

    - Abrir con UI: Crtl ,
      - Eslint: Enable
      - Controls whether eslint is enabled for JavaScript files or not.
    - Abrir como archivo: Crtl + shift + p seleccionar Open Setting (json) (19.40)

      - C:\Users\xxxx\AppData\Roaming\Code\User\settings.json

        ```json
        {
          "[javascript]": {
            // Utilizando CON prettier
            // "editor.defaultFormatter": "esbenp.prettier-vscode",
            // "editor.formatOnSave": true,
            // Original
            "editor.codeActionsOnSave": {
              "source.fixAll.eslint": true
            }
          }
        }
        ```

  - Desactivar reglas de ESLint y StandardJS (21.35)

    - 'React' must be in scope when using JSX y Error de las propTypes

      - En archivo ".eslintrc.js" sección "Rules"

        ```
        const RULES = {
          OFF: 'off',
          WARN: 'warn',
          ERROR: 'error'
        }
        module.exports = {
          rules: {
            'react/prop-types': RULES.OFF,
            'react/react-in-jsx-scope': RULES.OFF
          },
        }
        ```

## PRETTIER (29.10)

- Mismo estilo de código en todo nuestro proyecto.
  - Sitio oficial [Prettier](https://prettier.io/).
- Evitar conflictos con eslint. (40.30)

  - Ejecutar: npm i -D eslint-config-prettier
  - Ejecutar: npm i -D prettier
  - En archivo ".eslintrc.js" desactivar todas las reglas de linter q pelean con prettier.
  - Agregar com ÚLTIMA extensión la de prettier.

    ```
    extends: [
      'plugin:react/recommended',
      'standard',
      'prettier'
    ],

    ```

- Configuración prettier. (43.30)
  - crear archivo .prettierignore (45.00)
    - .next
  - crear archivo .prettierrc.json
    - Que exista aunque sea vacío.
- ver errores. (45.30)
  - npx prettier . --check
- corregir errores. (45.30)
  - npx prettier . --write
- Instalar extension de PRETTIER (46.15)

  - Prettier de Code formatter using prettier (esbenp.prettier-vscode)

  ```json
  {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "[javascript]": {
      "editor.defaultFormatter": "esbenp.prettier-vscode"
      // Fijarse en la parte de eslint que ya se especifica.
    }
  }
  ```

- Decirle a PRETTIER no usar ; (49.55)

  - En ".prettierrc.json" Prettier de Code

    ```json
    {
      "semi": false
    }
    ```

## VERIFICAR ESLINT Y PRETTIER SE CUMPLEN (54.30)

- Sitio oficial [lint-staged](https://github.com/okonet/lint-staged).

- Ejecutar: npx mrm@2 lint-staged
