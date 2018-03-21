# Pleak SQL Derivative Sensitivity Editor

This project is the front-end part of the [SQL derivative sensitivity analysis tool for pleak.io](https://github.com/pleak-tools/pleak-sql-analysis/tree/master/banach) that is a part of the [SQL analysis tool for pleak.io](https://github.com/pleak-tools/pleak-sql-analysis).

## Prerequisites

You need to locate [pleak-backend](https://github.com/pleak-tools/pleak-backend), [pleak-frontend](https://github.com/pleak-tools/pleak-frontend) and [pleak-sql-analysis](https://github.com/pleak-tools/pleak-sql-analysis) directories all in the same directory and specify their names in the config.json file.
Read more from sub-repositories how to build each module.

To use all functionalities of the SQL derivative sensitivity editor, clone the [pleak-sql-analysis](https://github.com/pleak-tools/pleak-sql-analysis) tool - SQL derivative sensitivity analyser is located in the banach subdirectory. To use it, set up:

1) [Cabal](https://www.haskell.org/cabal/)

To make the analyser available for the pleak-sql-derivative-sensitivity-editor, execute:

    `cabal sandbox init`
    `cabal install --only-dependencies`
    `cabal configure`
    `cabal build`

The executable is created into dist/build/banach directory.

You can find more information from the [SQL derivative sensitivity analysis tool repository](https://github.com/pleak-tools/pleak-sql-analysis/tree/master/banach).

## Build

To build the editor you need: NodeJS with npm installed.

To install all project dependencies execute `npm install`.

Execute `npm run build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Using

You can use the editor for each model from the Action menu next to the model on Files page (of frontend) or from the URL: http://localhost:8000/sql-derivative-sensitivity-editor/id (id of the model).

## License

MIT