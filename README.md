# boilerplate-lambda-api

A boilerplate for creating AWS API with Claudia & babel.

## Prerequisite
 - an AWS profile with sufficient permissions, see [claudia's lazy quick start](https://claudiajs.com/tutorials/installing.html#lazy-quick-start)

## Editor
Ensure your editor supports:
- [EditorConfig](http://editorconfig.org/#download).
- Live linting
  - [ESLint](http://eslint.org/docs/user-guide/integrations#editors) plugin installed and enabled for linting JS

## Scripts
| Command                 | Purpose                                                                                     |
|-------------------------|---------------------------------------------------------------------------------------------|
| `npm start`             | interactive cli menu to list and run npm tasks                                              |
| `npm run transpile`     | transpile (using `babel`) `src` folder to `build` folder                                    |
| `npm run lint:js`       | run `eslint` through `src` folder, display errors/warnings to stdout                        |
| `npm run lint:js:fix`   | run `eslint` through `src` folder, fix all auto-fixable problems                            |
| `npm run deploy:create` | transpile, then deploy the very first version of the api module, also create `claudia.json` |
| `npm run deploy`        | transpile, then update the api module                                                       |
| `npm run deploy:dev`    | transpile, then deploy to `dev` version of the api module                                   |
| `npm run destroy`       | **DANGEROUS** destroy the lambda module, also remove `claudia.json`                    |
