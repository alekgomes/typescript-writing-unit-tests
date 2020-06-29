# TypeScript Writing Unit Tests in VSCode

Escrevendo testes com [Jest](https://jestjs.io/) e debugando no [VSCode](https://code.visualstudio.com/).

Você pode abrir qualquer arquivo de teste e acionar `F5` ou executar a configuração `Jest Current File`.

Ou, apenas, executar no terminal...

    npm t
    npm run test
    npm run coverage

![jest-running-terminal-coverage](https://user-images.githubusercontent.com/1257048/86014952-602f6180-b9f7-11ea-9d8b-be4a284cc8af.png)



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


### Update 3

No Windows não estava rodando o launch corretamente.

Arrumei segundo https://stackoverflow.com/a/62622395
