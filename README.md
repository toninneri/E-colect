<h1 align=center>
<img src="https://github.com/Rocketseat/nlw-01-booster/blob/master/.github/ecoleta.png" />
</h1>

<div align="center">

![BADGE_LICENSE] ![BADGE_NODE_VERSION] ![BADGE_NPM_VERSION] ![BADGE_WEB_REACT] ![BADGE_MOBILE_REACT_NATIVE] ![BADGE_SERVER_NODEJS] ![BADGE_TYPESCRIPT] ![BADGE_OPEN_SOURCE] ![BADGE_OPEN_ISSUES] ![BADGE_CLOSED_ISSUES] ![BADGE_STARS] ![BADGE_FORKS]

</div>

<h3 align="center">


♻️ E-coleta is an **Open Source** project developed in **[Rocketseat's][rocketseat_site]** **Next Level Week (1.0** using TypeScript, Node, React and React Native technologies.
</h3>


## **:rocket: OBJECTIVE**

The project aims to ** establish a connection **between** companies and / or entities that collect waste **(organic and inorganic)** to people and / or entities that constantly need to dispose of this waste **.Solving a major recurring problem that is** inappropriate waste disposal **,facilitating the recycling and reuse process.

<!-- 
  ...
  Local Reservado para o GIF do projeto rodando.
  ...
-->

## **:computer: TECHNOLOGIES**


#### **Website** ([React][react] + [TypeScript][typescript])

  - **[React Router Dom][react_router_dom]**
  - **[React Icons][react_icons]**
  - **[Axios][axios]**
  - **[Leaflet][leaflet]**
  - **[React Leaflet][react_leaflet]**
  - **[React Dropzone][react_dropzone]**


  \* Veja o arquivo <kbd>[package.json](./sources/website/package.json)</kbd>

#### **Server** ([NodeJS][node] + [TypeScript][typescript])

  - **[Express][express]**
  - **[CORS][cors]**
  - **[KnexJS][knex]**
  - **[SQLite][sqlite3]**
  - **[ts-node][tsnode]**
  - **[dotENV][dotenv]**
  - **[Multer][multer]**
  - **[Celebrate][celebrate]**
  - **[Joi][joi]**

  \* See the file <kbd>[package.json](./sources/server/package.json)</kbd>

#### **Mobile** ([React Native][react_native] + [TypeScript][typescript])

  - **[Expo][expo]**
  - **[Expo Google Fonts][expo_google_fonts]**
  - **[React Navigation][react_navigation]**
  - **[React Native Maps][react_native_maps]**
  - **[Expo Constants][expo_constants]**
  - **[React Native SVG][react_native_svg]**
  - **[Axios][axios]**
  - **[Expo Location][expo_location]**
  - **[Expo Mail Composer][expo_mail_composer]**

  \* See the file <kbd>[package.json](./sources/mobile/package.json)</kbd>

#### **Utilitários**

- Protótipo: **[Figma](https://www.figma.com/)** &rarr; **<kbd>[Protótipo (Ecoleta)](https://www.figma.com/file/1SxgOMojOB2zYT0Mdk28lB/Ecoleta)</kbd>**
- API: **[IBGE API][ibge_api]** &rarr; **<kbd>[API de UFs][ibge_api_ufs]</kbd>**, **<kbd>[API de Municípios][ibge_api_municipios]</kbd>** 
- Maps: **[Leaflet][leaflet]**
- Editor: **[Visual Studio Code][vscode]** &rarr; Extensions: **<kbd>[SQLite][vscode_sqlite_extension]</kbd>**
- Markdown: **[StackEdit][stackedit]**, **<kbd>[Markdown Emoji][markdown_emoji]</kbd>**
- Commit Conventional: **[Commitlint][commitlint]**
- Teste de API: **[Insomnia][insomnia]**
- Ícones: **[Feather Icons][feather_icons]**, **[Font Awesome][font_awesome]**
- Fontes: **[Ubuntu][font_ubuntu]**, **[Roboto][font_roboto]**


## **:wine_glass: HOW TO USE THIS PROJECT**

### Initial Settings

First, you need to have<kbd>[NodeJS](https://nodejs.org/en/download/)</kbd> installed on your machine.

If you are using **Linux**, you can choose to install **Node** through version manager <kbd>[asdf]</kbd> to facilitate the process of changing the**Node**, when necessary.

You can also choose to use **yarn** instead of **npm**.  You can install it by clicking on this <kbd>[link][yarn]</kbd>,  or via <kbd>[asdf]</kbd>.

After having **Node** installed, install the **React and React Native (Expo)** dependencies globally, using the commands:



```sh
# React:
$ npm install create-react-app -g

# Expo (React Native):
$ npm install -g expo-cli 
```

You need to rename the file `.env-example` to `.env` and insert your **host** information :

```sh
$ mv .env-example .env
```

Install the dependencies contained in the `package.json` files at the root of the repository (for managing commits), in the **server**, directory, in the **website** directory and in the **mobile**. To install the dependencies, just open the terminal in the directory and type the command:


```sh
$ npm install

# ou
$ yarn
```

Examples:
```sh
# Installing commitlint dependencies:
$ cd ./ecoleta
$ npm install

# Installing the server dependencies:
$ cd ./sources/server
$ npm install

# Installing the website dependencies:
$ cd ./sources/website
$ npm install

# Installing the mobile dependencies:
$ cd ./sources/mobile
$ npm install
```

See the files **`package.json`** of <kbd>[commitlint](./package.json)</kbd>, <kbd>[server](./sources/server/package.json)</kbd>, <kbd>[website](./sources/website/package.json)</kbd> and <kbd>[mobile](./sources/mobile/package.json)</kbd>.

### Using the Server

```sh
# Opening the terminal in the server directory:
$ cd ./sources/server

# Running the application in development mode:
$ npm run dev

# Instantiating the database:
$ npm run knex:migrate

# Populating the database (seeds):
$ npm run knex:seed
```

> See part of **scripts {}** of file <kbd>[package.json](./sources/server/package.json)</kbd> to see which scripts are available.

### Using the Website

```sh
# Opening the terminal in the website directory:
$ cd ./sources/website

# Running the website in development mode:
$ npm run start
```

> If the browser does not open automatically, go to: http://localhost:3000.

### Using the Mobile

Install the application <kbd>[Expo](https://play.google.com/store/apps/details?id=host.exp.exponent&hl=en)</kbd> in your smartphone.

```sh
#Opening the terminal in the mobile directory:
$ cd ./sources/mobile

# Running the mobile in development mode:
$ npm run start
```

Now, open the expo app and in mode **LAN** scan the QRCode.

>If you have any problems running the application in this mode, try disabling your machine's firewall.

If you have a problem with the fonts, use the command:
```sh
$ expo install expo-font @expo-google-fonts/ubuntu @expo-google-fonts/roboto


```

**\* Remember to insert in the file `.env` the exact IP that was generated by your mobile after using the command `npm run start`.**


### :recycle: How to contribute

- Fork this repository;
- Make a uma branch with your feature: `git checkout -b my-feature`
- Commit your changes: `git commit -m 'feat: My new feature'`
- Push your branch: `git push origin my-feature`

Then, after your merge in your pull request be done, you can delete your branch.

## **:books: References**

- [React + TypeScript Cheat Sheet](https://github.com/typescript-cheatsheets/react-typescript-cheatsheet)
- [Blog Rocketseat](https://blog.rocketseat.com.br/)
- [ReactJS](https://reactjs.org/docs/getting-started.html) | [ReactJS pt-BR](https://pt-br.reactjs.org/docs/getting-started.html)
- [TypeScript](https://www.typescriptlang.org/docs/home.html)
- [React Native](https://reactnative.dev/docs/getting-started)
- [Expo](https://expo.io/learn)
- [Knex][knex]
- [Express](https://expressjs.com/pt-br/)
- [Node](https://nodejs.org/en/)
- [Celebrate](https://github.com/arb/celebrate)
- [Joi](https://hapi.dev/module/joi/)

## **:page_with_curl: LICENSE**

This repository is licensed by  **MIT LICENSE**.  For more detailed information, read the [LICENSE] file (./ LICENSE) contained in this repository.

<h3 align="center">
Done by <a href="https://www.linkedin.com/in/antonio-neri-6789828/">Antonio Neri</a>
<br><br>
<a href="https://rocketseat.com.br">
  <img alt="Made by Rocketseat" src="https://img.shields.io/badge/made%20by-Rocketseat-%237519C1">
</a>
</h3>

<!-- Website Links -->

[rocketseat_site]: https://rocketseat.com.br/

<!-- Badges -->

[BADGE_CLOSED_ISSUES]: https://img.shields.io/github/issues-closed/x0n4d0/ecoleta?color=red

[BADGE_OPEN_ISSUES]: https://img.shields.io/github/issues/x0n4d0/ecoleta?color=green

[BADGE_LICENSE]: https://img.shields.io/github/license/x0n4d0/ecoleta

[BADGE_NODE_VERSION]: https://img.shields.io/badge/node-12.17.0-green

[BADGE_NPM_VERSION]: https://img.shields.io/badge/npm-6.14.4-red

[BADGE_WEB_REACT]: https://img.shields.io/badge/web-react-blue

[BADGE_MOBILE_REACT_NATIVE]: https://img.shields.io/badge/mobile-react%20native-blueviolet

[BADGE_SERVER_NODEJS]: https://img.shields.io/badge/server-nodejs-important

[BADGE_STARS]: https://img.shields.io/github/stars/x0n4d0/ecoleta?style=social

[BADGE_FORKS]: https://img.shields.io/github/forks/x0n4d0/ecoleta?style=social

[BADGE_TYPESCRIPT]: https://badges.frapsoft.com/typescript/code/typescript.png?v=101

[BADGE_OPEN_SOURCE]: https://badges.frapsoft.com/os/v1/open-source.png?v=103

<!-- Techs -->

[react]: https://reactjs.org/

[typescript]: https://www.typescriptlang.org/

[node]: https://nodejs.org/en/

[leaflet]: https://react-leaflet.js.org/en/

[ibge_api]: https://servicodados.ibge.gov.br/api/docs/localidades?versao=1

[ibge_api_ufs]: https://servicodados.ibge.gov.br/api/docs/localidades?versao=1#api-UFs-estadosGet

[ibge_api_municipios]: https://servicodados.ibge.gov.br/api/docs/localidades?versao=1#api-Municipios-estadosUFMunicipiosGet

[vscode]: https://code.visualstudio.com/

[react_native]: http://www.reactnative.com/

[stackedit]: https://stackedit.io

[vscode_sqlite_extension]: https://marketplace.visualstudio.com/items?itemName=alexcvzz.vscode-sqlite

[markdown_emoji]: https://gist.github.com/rxaviers/7360908

[commitlint]: https://github.com/conventional-changelog/commitlint

[express]: https://expressjs.com/

[cors]: https://expressjs.com/en/resources/middleware/cors.html

[knex]: http://knexjs.org/

[sqlite3]: https://github.com/mapbox/node-sqlite3

[tsnode]: https://github.com/TypeStrong/ts-node

[feather_icons]: https://feathericons.com/

[insomnia]: https://insomnia.rest/

[react_leaflet]: https://react-leaflet.js.org/

[react_router_dom]: https://github.com/ReactTraining/react-router/tree/master/packages/react-router-dom

[react_icons]: https://react-icons.github.io/react-icons/

[axios]: https://github.com/axios/axios

[dotenv]: https://github.com/motdotla/dotenv

[expo]: https://expo.io/

[expo_google_fonts]: https://github.com/expo/google-fonts

[react_navigation]: https://reactnavigation.org/

[react_native_maps]: https://github.com/react-native-community/react-native-maps

[expo_constants]: https://docs.expo.io/versions/latest/sdk/constants/

[react_native_svg]: https://github.com/react-native-community/react-native-svg

[expo_location]: https://docs.expo.io/versions/latest/sdk/location/

[expo_mail_composer]: https://docs.expo.io/versions/latest/sdk/mail-composer/

[font_roboto]: https://fonts.google.com/specimen/Roboto

[font_ubuntu]: https://fonts.google.com/specimen/Ubuntu

[font_awesome]: https://fontawesome.com/

[multer]: https://github.com/expressjs/multer

[celebrate]: https://github.com/arb/celebrate

[joi]: https://github.com/hapijs/joi

[react_dropzone]: https://github.com/react-dropzone/react-dropzone

[asdf]: https://github.com/asdf-vm/asdf

[yarn]: https://classic.yarnpkg.com/en/docs/install/#debian-stable
