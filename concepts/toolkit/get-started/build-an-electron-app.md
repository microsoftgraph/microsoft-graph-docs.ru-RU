---
title: Используйте microsoft Graph набор средств с электронным
description: Начало работы с помощью microsoft Graph набор средств в приложении Electron.
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: ad0d13ceb8a6ef12535dd635bf7eb011d765db9d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471430"
---
# <a name="use-the-microsoft-graph-toolkit-with-electron"></a>Используйте microsoft Graph набор средств с электронным

В этой статье описывается пошаговой процесс использования microsoft Graph набор средств для создания приложения Electron и подключения его к Microsoft 365. После выполнения действий у вас будет приложение Electron, которое отображает предстоящие встречи подписанного пользователя из Microsoft 365.

## <a name="create-an-electron-app"></a>Создание приложения Electron 
Создайте новое приложение Electron, клонив репозиторий [электронного](https://github.com/electron/electron-quick-start-typescript) быстрого запуска. Это создаст новое приложение Electron с помощью TypeScript, которое поможет вам написать более надежный код и избежать ошибок во время работы.

```cmd
git clone https://github.com/electron/electron-quick-start-typescript
```

Измените рабочий каталог на недавно созданное приложение и установите все зависимости.

```cmd
cd electron-quick-start-typescript
npm install
```

Установите пакет @microsoft/mgt-components, содержащий все веб-компоненты, связанные с Microsoft Graph.

```cmd
npm i @microsoft/mgt-components
```

Установите `@microsoft/mgt-electron-provider` и `@microsoft/mgt-element` пакеты npm. Это позволит вам обеспечить проверку подлинности для вашего приложения с помощью MSAL и использовать компоненты Microsoft Graph набор средств.

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-electron-provider
```

Подтвердите, что вы можете запустить приложение.

```cmd
npm start
```

## <a name="create-an-appclient-id"></a>Создание идентификатора клиента/приложения

### <a name="add-new-application-registration-in-azure-ad-to-get-a-client-id"></a>Добавление новой регистрации приложений в Azure AD, чтобы получить ИД клиента

Чтобы создать приложение в Azure Active Directory (Azure AD), необходимо добавить новую регистрацию приложений, а затем настроить имя приложения и перенаправить URI.

Чтобы создать приложение в Azure AD:

1. Перейдите на [портал Azure.](https://portal.azure.com)
1. В меню выберите **Azure Active Directory**.
1. В меню Azure Active Directory выберите **Регистрация приложений**.
1. В верхнем меню нажмите кнопку **Новая регистрация**.
1. Введите имя приложения; например, `My Electron-App` .
1. Для параметра [Поддерживаемые типы учетных записей](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app) выберите **Учетные записи в любом каталоге организации (любой каталог Azure AD — мультитенантный) и персональные учетные записи Майкрософт (например, Skype, Xbox)**.
1. В поле **Перенаправление URI** в отсеве выберите общедоступный **клиент/родной (мобильный &** рабочий стол), а в поле URL-адрес введите `msal://redirect` .
1. Подтвердите изменения, нажав кнопку **Зарегистрировать**.
1. Перейдите к регистрации приложения.
1. Убедитесь, что вы находитесь на странице **Обзор**.
1. В разделе **Essentials** скопируйте значение свойства **ID** приложения (клиента).

## <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a>Настройка поставщика проверки подлинности Microsoft Graph Toolkit

### <a name="initializing-electronprovider-in-your-renderer-process"></a>Инициализация ElectronProvider в процессе отрисовки

Отвечает за взаимодействие (в основном процессе) с запросом маркеров доступа и получением сведений о подписании в состоянии, необходимом для работы компонентов `ElectronProvider` `ElectronAuthenticator` mgt. 

Чтобы инициализировать, добавьте следующий код в `ElectronProvider` *файл src/renderer.ts.*
```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
// import the mgt components so we can use them in our html
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-your-main-process"></a>Инициализация ElectronAuthenticator в основном процессе

Отвечает за настройку переменных конфигурации для проверки подлинности MSAL, приобретения маркеров доступа и общения `ElectronAuthenticator` с `ElectronProvider` . Инициализация основного процесса и настройка переменных конфигурации, таких как `ElectronAuthenticator` client ID и необходимые области. 

Сначала откройте *src/main.ts* и импортируете и в `ElectronAuthenticator`  `MsalElectronConfig` `@microsoft/mgt-electron-provider` верхней части страницы.

```ts
import { ElectronAuthenticator, MsalElectronConfig } from '@microsoft/mgt-electron-provider/dist/Authenticator'; 
```
Затем добавьте эти строки кода в функцию для инициализации `createWindow()` ElectronAuthenticator сразу после того, как `mainWindow` будет объявлено. Замените `<your_client_id>` с помощью клиентского ИД из регистрации приложения.

```ts
const config: MsalElectronConfig = {
  clientId: '<your_client_id>',
  mainWindow: mainWindow, //This is the BrowserWindow instance that requires authentication
  scopes: [
    'user.read',
        'user.read',
        'people.read',
        'user.readbasic.all',
        'contacts.read',
        'presence.read.all',
        'presence.read',
        'user.read.all',
        'calendars.read'
  ],
};
ElectronAuthenticator.initialize(config);
```

### <a name="set-nodeintegration-to-true"></a>Установите узелИнтеграция к true
 
В main.ts, где создается новый экземпляр BrowserWindow, убедитесь, что вы задались `nodeIntegration` в `true` рамках webPreferences. Если пропустить этот шаг, может возникнуть ```Uncaught ReferenceError: require is not defined``` ошибка. Чтобы сделать это простым, удалите все сценарии предварительной загрузки.

```ts
const mainWindow = new BrowserWindow({
  height: 600,
  webPreferences: {
    nodeIntegration: true //Set this to true
  },
  width: 800
});
```
 
### <a name="add-components-to-your-html-page"></a>Добавление компонентов на страницу HTML
 
Добавьте некоторое содержимое в приложение. Теперь вы можете использовать компоненты наборов инструментов Microsoft Graph на странице *index.html* и показать повестку дня пользователя. Замените содержимое страницы *index.html* следующим.
 
 ```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Sample Electron-MGT App</title>
  </head>
  <body>
    <mgt-login></mgt-login>
    <mgt-agenda group-by-day></mgt-agenda>
    <script type="module" src="./dist/renderer.js"></script>
  </body>
</html>
 ```
 >**Примечание:** Удалите все заглавные заготки или теги ответов content-Security-Policy, если `meta` вы копируете это в существующий файл.
 
 ### <a name="bundle-your-app-using-webpack"></a>Пакет приложения с помощью веб-пакета
 
Прежде чем запустить приложение, необходимо объединить код, чтобы убедиться, что все модульные зависимости включены в итоговую нагрузку. Если вы уже задав код приложения, вы можете пропустить этот шаг.
 
 #### <a name="install-webpack"></a>Установка веб-упаковки
 
 ```cmd 
 npm install webpack webpack-cli ts-loader --save-dev
 ```
 
 #### <a name="webpackconfigjs"></a>webpack.config.js
 
Создайте *новыйwebpack.config.js* файл в корневой папке проекта и вложите следующую конфигурацию.
 
 ```js
 const path = require('path');
 module.exports = [
  {
    mode: 'development',
    entry: './src/renderer.ts',
    target: 'electron-renderer',
    module: {
      rules: [
        {
          test: /\.ts$/,
          include: [/src/],
          use: [{ loader: 'ts-loader' }]
        }
      ]
    },
    output: {
      path: __dirname + '/dist',
      filename: 'renderer.js'
    },
    resolve: {
      extensions: ['.ts', '.js'],
      modules: ['node_modules', path.resolve(__dirname + 'src')]
    }
  },
  {
    mode: 'development',
    entry: './src/main.ts',
    target: 'electron-main',
    module: {
      rules: [
        {
          test: /\.ts$/,
          include: [/src/],
          use: [{ loader: 'ts-loader' }]
        }
      ]
    },
    output: {
      path: __dirname + '/dist',
      filename: 'main.js'
    },
    resolve: {
      extensions: ['.ts', '.js'],
      modules: ['node_modules', path.resolve(__dirname + 'src')]
    }
  }
 ];

 ```
 
 Как видите, передняя часть (процесс рендера) и задний (основной процесс) объединены отдельно. Это потому, что в Electron процесс рендера выполняется в контексте браузера, а основной процесс выполняется в контексте узла.
 
 #### <a name="add-the-webpacking-script-in-packagejson"></a>Добавление сценария веб-упаковки в ```package.json```
 
 Добавьте ниже в ```scripts``` вашем ```package.json``` .
 
 ```json
"scripts": {
   "webpack": "webpack",
   "start": "npm run webpack && electron dist/main.js"
 }                
 ```
 
 #### <a name="run-your-app"></a>Запуск приложения
 
 ```cmd
 npm start
 ```

### <a name="add-token-caching-capabilities-to-your-app-and-enable-silent-sign-ins-advanced"></a>Добавьте возможности кэшинга маркеров в приложение и встройте входы в бесшумный вход (расширенный)

Узел MSAL поддерживает кэш в памяти по умолчанию и предоставляет интерфейс ICachePlugin для выполнения сериализации кэша, но не предоставляет способ хранения кэша маркера на диск по умолчанию. Если вам требуется постоянное хранилище кэша для обеспечения бесшумных входных входов или межплатформенного кэширования, рекомендуется использовать реализацию по умолчанию, предоставленную узлом MSAL в качестве [расширения.](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions) Этот плагин можно импортировать и передавать экземпляр плагина кэша при инициализации. `ElectronAuthenticator`

```ts
let config: MsalElectronConfig = {
  ...
  cachePlugin: new PersistenceCachePlugin(filePersistence) //filePersistence is the instance of type IPersistence that you will need to create
};
```
Дополнительные сведения о том, как реализовать это, см. в примере [microsoft-authentication-library-for-js.](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/extensions/samples/msal-node-extensions/index.js)

## <a name="next-steps"></a>Дальнейшие действия
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задайте вопрос [в Microsoft Q&A](https://aka.ms/askgraph).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).
    
