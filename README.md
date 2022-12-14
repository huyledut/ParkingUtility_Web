<h1 align="center">Angular Boilerplate</h1>

<p align="center">
  <img src="https://img.icons8.com/ios-filled/150/000000/angularjs.png" alt="angular-logo" width="120px" height="120px"/>
  <br>
  <i>Lightweight & minimalistic Angular starter</i>
  <br>
</p>

<p align="center">
  <a href="https://angularboilerplate.vercel.app"><strong>https://angularboilerplate.vercel.app</strong></a>
  <br>
</p>

<p align="center">
  <a href="CONTRIBUTING.md">Contributing Guidelines</a>
  Â·
  <a href="https://github.com/juanmesa2097/angular-boilerplate/issues">Submit an Issue</a>
  <br>
  <br>
</p>
<hr>

## âï¸ Features

- Lazy loading
- Standalone components
- OS/Light/Dark modes
- Strongly-typed storage
- TailwindCSS

## ð ï¸ Tweaks

- TailwindCSS configuration:

  You can find the `tailwind.config.js` file in the project root, then you can refer to https://tailwindcss.com/docs/configuration to learn how to make your own adjustments.

- Set default theme (first time load)

  Go to `src\app\lib\constants.ts` and choose the default theme.

  OS preference

  ```ts
  export const DEFAULT_BASE_THEME: AppTheme = 'system' as const;
  ```

  Light mode

  ```ts
  export const DEFAULT_BASE_THEME: AppTheme = 'light' as const;
  ```

  Dark mode

  ```ts
  export const DEFAULT_BASE_THEME: AppTheme = 'dark' as const;
  ```

- Enable a new local/session storage item

  Go to `src\app\lib\utils\storage\storage.types.ts` and add a new item name in the `StorageObjectType` type and a new key value pair in the `StorageObjectMap` type.

  ![image](https://user-images.githubusercontent.com/64181348/173276010-a4b95a63-2fe0-4104-9b09-34eeea5f0025.png)

  After that, you can use the new item.
  ![image](https://user-images.githubusercontent.com/64181348/173276575-09322722-387d-4c20-95af-fa9915079e3a.png)

## â©ï¸ Project structure

```console
ââââapp
â   ââââlib
â   â   ââââcomponents
â   â   â   ââââfooter
â   â   â   ââââlayouts
â   â   â   â   ââââlayout-horizontal
â   â   â   ââââlogo
â   â   â   âââânavbar
â   â   ââââguards
â   â   ââââinterceptors
â   â   ââââinterfaces
â   â   ââââenums
â   â   ââââservices
â   â   â   ââââauth
â   â   â   ââââtheme
â   â   ââââutils
â   â       ââââstorage
â   ââââpages
â       ââââauth
â       â   ââââlogin
â       â   ââââregister
â       ââââhome
â       ââââprofile
â       ââââscreens
â       â   âââânot-found
â       ââââsettings
â           ââââaccessibility
â           ââââaccount
â           ââââappearance
ââââassets
ââââenvironments
ââââtheme
    ââââ01-base
    ââââ02-components
    ââââ03-utilities
    ââââtailwindcss
```

## ð§ââï¸ Commands

| Command  | Description                                                 | NPM              | Yarn          | PNPM          | Background command                              |
| -------- | ----------------------------------------------------------- | ---------------- | ------------- | ------------- | ----------------------------------------------- |
| ng       | See available commands                                      | npm run ng       | yarn ng       | pnpm ng       | ng                                              |
| start    | Run app in development mode                                 | npm start        | yarn start    | pnpm start    | ng serve                                        |
| build    | Build app for production                                    | npm run build    | yarn build    | pnpm build    | ng build                                        |
| watch    | Run build when files change                                 | npm run watch    | yarn watch    | pnpm watch    | ng build --watch --configuration development    |
| test     | Run unit tests                                              | npm run test     | yarn test     | pnpm test     | ng test                                         |
| test:run | Run unit tests with headless browser and without watch mode | npm run test:run | yarn test:run | pnpm test:run | ng test --watch=false --browsers ChromeHeadless |
| lint     | Lint code                                                   | npm run lint     | yarn lint     | pnpm lint     | ng lint                                         |
