# TypeScript Writing Unit Tests in VSCode

Escrevendo testes com [Jest](https://jestjs.io/) e debugando no [VSCode](https://code.visualstudio.com/).

Você pode abrir qualquer arquivo de teste e acionar `F5` ou executar a configuração `Jest Current File`.

Ou, apenas, executar no terminal...

    npm t
    npm run test
    npm run coverage

![](jest-running-terminal-coverage.png)


### Veja também

+ https://github.com/microsoft/vscode-recipes/blob/master/debugging-jest-tests/.vscode/launch.json
+ https://github.com/jest-community/vscode-jest/blob/master/.vscode/launch.json

### Update 1

Do nada começou a apresentar os seguinte erro...

    error TS2582: Cannot find name 'test'. Do you need to install type definitions for a test runner

Para resolver bastou executar: `npm install jest @types/jest ts-jest`.

https://stackoverflow.com/questions/56595053/cannot-find-name-it-in-jest-typescript


### Update 2

Não se esqueça que temos o plugin recomendado pela comunidade Jest para VSCode.

https://marketplace.visualstudio.com/items?itemName=Orta.vscode-jest

Com ele é posspível utilizar o menu de contexto (botão direito do mouse) para acionar os scripts.

