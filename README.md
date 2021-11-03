# Audio Player

Este simples Audio Player Music App busca músicas no iTunes e toca um trechinho na tela

![celular com o aplicativo Audio Player sendo executado](https://github.com/jmanoel7/Audio-Player/blob/main/audio-player-preview.png?raw=true)

## Para fazer este App foi necessário o uso de

- [Git](https://git-scm.com/)       - para hospedagem do código fonte
- [Node.js](https://nodejs.org/)   - para instalar as demais ferramentas javascript
- [Angular](https://angular.io/)   - para interface (frontend) foi usado Angular Material
- [RxJS](https://rxjs.dev/)      - para baixar dados usando a API do iTunes
- [Capacitor](https://capacitorjs.com/) - para aproveitar o mesmo código fonte e construir em iOS, Android e PWA

## Baixe e instale o Git e o Node.js

- [Git](https://git-scm.com/download/win)

- [Node.js](https://nodejs.org/en/download/), estou usando a versão [LTS 14](https://nodejs.org/dist/latest-v14.x/), mas você pode usar outra versão >= 14 sem problemas

## Depois, execute os seguintes comandos no terminal

```sh
git clone https://github.com/jmanoel7/Audio-Player
cd Audio-Player
npm install @angular/cli
npm install --save-dev --force @angular-devkit/build-angular
npm install rxjs
```

Agora já temos o reposiório git clonado localmente, instalado **Angular** e **RxJS** dentro do repositório git

**OBS:** Não precisamos instalar o **Capacitor** pois o mesmo já está instalado e configurado para desenvolvimento na plataforma iOS

## Servidor de desenvolvimento

Execute `ng serve` para um servidor de desenvolvimento. Navegue até `http://localhost:4200/`. O aplicativo será recarregado automaticamente se você alterar qualquer um dos arquivos fontes.

**OBS:** se `ng serve` der erro, tente `ng serve -o`.

## Andaime de código

Execute `ng generate component component-name` para gerar um novo componente. Você também pode usar `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Construção

Execute `ng build` para construir o projeto. Os artefatos de construção serão armazenados no diretório `dist/`. Use a opção `--prod` para uma construção de produção.
**OBS:** já se encontra em `dist/` uma versão PWA (Progressive Web App) em produção para uso em web server como apache, nginx, etc.

## Executando testes de unidade

Execute:

- `npm install karma` na raíz do projeto para instalar o [Karma](https://karma-runner.github.io).
- `ng test` para executar os testes de unidade via [Karma](https://karma-runner.github.io).

## Executando testes end-to-end

Execute:

- `npm install protractor` na raíz do projeto para instalar o [Protractor](http://www.protractortest.org/).
- `ng e2e` para executar os testes end-to-end via [Protractor](http://www.protractortest.org/).

## Mais ajuda

Para obter mais ajuda sobre o Angular CLI, use `ng help` ou confira o [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

## ATENÇÃO

- Já foi adicionado o código para desenvolvimento pwa: `ng add @angular/pwa --project music-list`
- Também já foram adicionados os códigos para desenvolvimento do iOS e do Android:
  - `npm install @capacitor/ios @capacitor/android`
  - `npx cap add ios`
  - `npx cap add android`

**OBS:** esses comandos **não** precisam ser repetidos

## TODO

- construção do aplicativo para iOS
- construção do aplicativo para Android
