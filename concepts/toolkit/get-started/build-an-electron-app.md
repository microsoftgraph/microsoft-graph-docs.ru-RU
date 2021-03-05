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
# <a name="use-the-microsoft-graph-toolkit-with-electron"></a><span data-ttu-id="b7298-103">Используйте microsoft Graph набор средств с электронным</span><span class="sxs-lookup"><span data-stu-id="b7298-103">Use the Microsoft Graph Toolkit with Electron</span></span>

<span data-ttu-id="b7298-104">В этой статье описывается пошаговой процесс использования microsoft Graph набор средств для создания приложения Electron и подключения его к Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b7298-104">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create an Electron app and connect it to Microsoft 365.</span></span> <span data-ttu-id="b7298-105">После выполнения действий у вас будет приложение Electron, которое отображает предстоящие встречи подписанного пользователя из Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b7298-105">After completing the steps, you'll have a Electron app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="create-an-electron-app"></a><span data-ttu-id="b7298-106">Создание приложения Electron</span><span class="sxs-lookup"><span data-stu-id="b7298-106">Create an Electron app</span></span> 
<span data-ttu-id="b7298-107">Создайте новое приложение Electron, клонив репозиторий [электронного](https://github.com/electron/electron-quick-start-typescript) быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="b7298-107">Create a new Electron app by cloning the [electron-quick-start-typescript](https://github.com/electron/electron-quick-start-typescript) repository.</span></span> <span data-ttu-id="b7298-108">Это создаст новое приложение Electron с помощью TypeScript, которое поможет вам написать более надежный код и избежать ошибок во время работы.</span><span class="sxs-lookup"><span data-stu-id="b7298-108">This will create a new Electron app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
git clone https://github.com/electron/electron-quick-start-typescript
```

<span data-ttu-id="b7298-109">Измените рабочий каталог на недавно созданное приложение и установите все зависимости.</span><span class="sxs-lookup"><span data-stu-id="b7298-109">Change the working directory to the newly created app and install all dependencies.</span></span>

```cmd
cd electron-quick-start-typescript
npm install
```

<span data-ttu-id="b7298-110">Установите пакет @microsoft/mgt-components, содержащий все веб-компоненты, связанные с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b7298-110">Install the '@microsoft/mgt-components' package that contains all the Microsoft Graph-connected web components.</span></span>

```cmd
npm i @microsoft/mgt-components
```

<span data-ttu-id="b7298-111">Установите `@microsoft/mgt-electron-provider` и `@microsoft/mgt-element` пакеты npm.</span><span class="sxs-lookup"><span data-stu-id="b7298-111">Install the `@microsoft/mgt-electron-provider` and `@microsoft/mgt-element` npm packages as well.</span></span> <span data-ttu-id="b7298-112">Это позволит вам обеспечить проверку подлинности для вашего приложения с помощью MSAL и использовать компоненты Microsoft Graph набор средств.</span><span class="sxs-lookup"><span data-stu-id="b7298-112">These will allow you to provide authentication for your app using MSAL and use the Microsoft Graph Toolkit components.</span></span>

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-electron-provider
```

<span data-ttu-id="b7298-113">Подтвердите, что вы можете запустить приложение.</span><span class="sxs-lookup"><span data-stu-id="b7298-113">Confirm that you can run the app.</span></span>

```cmd
npm start
```

## <a name="create-an-appclient-id"></a><span data-ttu-id="b7298-114">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="b7298-114">Create an app/client ID</span></span>

### <a name="add-new-application-registration-in-azure-ad-to-get-a-client-id"></a><span data-ttu-id="b7298-115">Добавление новой регистрации приложений в Azure AD, чтобы получить ИД клиента</span><span class="sxs-lookup"><span data-stu-id="b7298-115">Add new application registration in Azure AD to get a client ID</span></span>

<span data-ttu-id="b7298-116">Чтобы создать приложение в Azure Active Directory (Azure AD), необходимо добавить новую регистрацию приложений, а затем настроить имя приложения и перенаправить URI.</span><span class="sxs-lookup"><span data-stu-id="b7298-116">To create an application in Azure Active Directory (Azure AD), you need to add a new application registration, and then configure an app name and redirect URI.</span></span>

<span data-ttu-id="b7298-117">Чтобы создать приложение в Azure AD:</span><span class="sxs-lookup"><span data-stu-id="b7298-117">To create the app in Azure AD:</span></span>

1. <span data-ttu-id="b7298-118">Перейдите на [портал Azure.](https://portal.azure.com)</span><span class="sxs-lookup"><span data-stu-id="b7298-118">Go to the [Azure portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="b7298-119">В меню выберите **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="b7298-119">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="b7298-120">В меню Azure Active Directory выберите **Регистрация приложений**.</span><span class="sxs-lookup"><span data-stu-id="b7298-120">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="b7298-121">В верхнем меню нажмите кнопку **Новая регистрация**.</span><span class="sxs-lookup"><span data-stu-id="b7298-121">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="b7298-122">Введите имя приложения; например, `My Electron-App` .</span><span class="sxs-lookup"><span data-stu-id="b7298-122">Enter the name for your app; for example, `My Electron-App`.</span></span>
1. <span data-ttu-id="b7298-123">Для параметра [Поддерживаемые типы учетных записей](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app) выберите **Учетные записи в любом каталоге организации (любой каталог Azure AD — мультитенантный) и персональные учетные записи Майкрософт (например, Skype, Xbox)**.</span><span class="sxs-lookup"><span data-stu-id="b7298-123">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="b7298-124">В поле **Перенаправление URI** в отсеве выберите общедоступный **клиент/родной (мобильный &** рабочий стол), а в поле URL-адрес введите `msal://redirect` .</span><span class="sxs-lookup"><span data-stu-id="b7298-124">In the **Redirect URI** field, in the dropdown, select **Public client/native (mobile & desktop)**, and in the URL field, enter `msal://redirect`.</span></span>
1. <span data-ttu-id="b7298-125">Подтвердите изменения, нажав кнопку **Зарегистрировать**.</span><span class="sxs-lookup"><span data-stu-id="b7298-125">Confirm changes by selecting the **Register** button.</span></span>
1. <span data-ttu-id="b7298-126">Перейдите к регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="b7298-126">Go to your application registration.</span></span>
1. <span data-ttu-id="b7298-127">Убедитесь, что вы находитесь на странице **Обзор**.</span><span class="sxs-lookup"><span data-stu-id="b7298-127">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="b7298-128">В разделе **Essentials** скопируйте значение свойства **ID** приложения (клиента).</span><span class="sxs-lookup"><span data-stu-id="b7298-128">From the **Essentials** section, copy the value of the **Application (client) ID** property.</span></span>

## <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="b7298-129">Настройка поставщика проверки подлинности Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="b7298-129">Configure the Microsoft Graph Toolkit authentication provider</span></span>

### <a name="initializing-electronprovider-in-your-renderer-process"></a><span data-ttu-id="b7298-130">Инициализация ElectronProvider в процессе отрисовки</span><span class="sxs-lookup"><span data-stu-id="b7298-130">Initializing ElectronProvider in your renderer process</span></span>

<span data-ttu-id="b7298-131">Отвечает за взаимодействие (в основном процессе) с запросом маркеров доступа и получением сведений о подписании в состоянии, необходимом для работы компонентов `ElectronProvider` `ElectronAuthenticator` mgt.</span><span class="sxs-lookup"><span data-stu-id="b7298-131">The `ElectronProvider` is responsible for communicating with `ElectronAuthenticator` (in the main process) to request access tokens and receive information regarding signed in state that is required for the mgt components to work.</span></span> 

<span data-ttu-id="b7298-132">Чтобы инициализировать, добавьте следующий код в `ElectronProvider` *файл src/renderer.ts.*</span><span class="sxs-lookup"><span data-stu-id="b7298-132">To initialize the `ElectronProvider`, add the following code to the *src/renderer.ts* file.</span></span>
```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
// import the mgt components so we can use them in our html
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-your-main-process"></a><span data-ttu-id="b7298-133">Инициализация ElectronAuthenticator в основном процессе</span><span class="sxs-lookup"><span data-stu-id="b7298-133">Initializing ElectronAuthenticator in your main process</span></span>

<span data-ttu-id="b7298-134">Отвечает за настройку переменных конфигурации для проверки подлинности MSAL, приобретения маркеров доступа и общения `ElectronAuthenticator` с `ElectronProvider` .</span><span class="sxs-lookup"><span data-stu-id="b7298-134">The `ElectronAuthenticator` is responsible for setting up the configuration variables for MSAL authentication, acquiring access tokens, and communicating with the `ElectronProvider`.</span></span> <span data-ttu-id="b7298-135">Инициализация основного процесса и настройка переменных конфигурации, таких как `ElectronAuthenticator` client ID и необходимые области.</span><span class="sxs-lookup"><span data-stu-id="b7298-135">Initialize the `ElectronAuthenticator` in the main process and set up the configuration variables such as client ID and required scopes.</span></span> 

<span data-ttu-id="b7298-136">Сначала откройте *src/main.ts* и импортируете и в `ElectronAuthenticator`  `MsalElectronConfig` `@microsoft/mgt-electron-provider` верхней части страницы.</span><span class="sxs-lookup"><span data-stu-id="b7298-136">First, open *src/main.ts* and import `ElectronAuthenticator` and  `MsalElectronConfig` from `@microsoft/mgt-electron-provider` at the top of the page.</span></span>

```ts
import { ElectronAuthenticator, MsalElectronConfig } from '@microsoft/mgt-electron-provider/dist/Authenticator'; 
```
<span data-ttu-id="b7298-137">Затем добавьте эти строки кода в функцию для инициализации `createWindow()` ElectronAuthenticator сразу после того, как `mainWindow` будет объявлено.</span><span class="sxs-lookup"><span data-stu-id="b7298-137">Next, add these lines of code in the `createWindow()` function to initialize the ElectronAuthenticator, right after where `mainWindow` is declared.</span></span> <span data-ttu-id="b7298-138">Замените `<your_client_id>` с помощью клиентского ИД из регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="b7298-138">Replace `<your_client_id>` with the client ID from your app registration.</span></span>

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

### <a name="set-nodeintegration-to-true"></a><span data-ttu-id="b7298-139">Установите узелИнтеграция к true</span><span class="sxs-lookup"><span data-stu-id="b7298-139">Set nodeIntegration to true</span></span>
 
<span data-ttu-id="b7298-140">В main.ts, где создается новый экземпляр BrowserWindow, убедитесь, что вы задались `nodeIntegration` в `true` рамках webPreferences.</span><span class="sxs-lookup"><span data-stu-id="b7298-140">In main.ts, where the new instance of BrowserWindow is created, make sure that you set `nodeIntegration` to `true` under webPreferences.</span></span> <span data-ttu-id="b7298-141">Если пропустить этот шаг, может возникнуть ```Uncaught ReferenceError: require is not defined``` ошибка.</span><span class="sxs-lookup"><span data-stu-id="b7298-141">If you skip this step, you might run into a ```Uncaught ReferenceError: require is not defined``` error.</span></span> <span data-ttu-id="b7298-142">Чтобы сделать это простым, удалите все сценарии предварительной загрузки.</span><span class="sxs-lookup"><span data-stu-id="b7298-142">To keep this simple, remove any preloading scripts.</span></span>

```ts
const mainWindow = new BrowserWindow({
  height: 600,
  webPreferences: {
    nodeIntegration: true //Set this to true
  },
  width: 800
});
```
 
### <a name="add-components-to-your-html-page"></a><span data-ttu-id="b7298-143">Добавление компонентов на страницу HTML</span><span class="sxs-lookup"><span data-stu-id="b7298-143">Add components to your HTML page</span></span>
 
<span data-ttu-id="b7298-144">Добавьте некоторое содержимое в приложение.</span><span class="sxs-lookup"><span data-stu-id="b7298-144">Add some content to your app.</span></span> <span data-ttu-id="b7298-145">Теперь вы можете использовать компоненты наборов инструментов Microsoft Graph на странице *index.html* и показать повестку дня пользователя.</span><span class="sxs-lookup"><span data-stu-id="b7298-145">You can now use the Microsoft Graph toolkit components in your *index.html* page and show the user's agenda.</span></span> <span data-ttu-id="b7298-146">Замените содержимое страницы *index.html* следующим.</span><span class="sxs-lookup"><span data-stu-id="b7298-146">Replace the content of the *index.html* page with the following.</span></span>
 
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
 ><span data-ttu-id="b7298-147">**Примечание:** Удалите все заглавные заготки или теги ответов content-Security-Policy, если `meta` вы копируете это в существующий файл.</span><span class="sxs-lookup"><span data-stu-id="b7298-147">**Note:** Remove any Content-Security-Policy response headers or `meta` tags if you are copying this onto an existing file.</span></span>
 
 ### <a name="bundle-your-app-using-webpack"></a><span data-ttu-id="b7298-148">Пакет приложения с помощью веб-пакета</span><span class="sxs-lookup"><span data-stu-id="b7298-148">Bundle your app using webpack</span></span>
 
<span data-ttu-id="b7298-149">Прежде чем запустить приложение, необходимо объединить код, чтобы убедиться, что все модульные зависимости включены в итоговую нагрузку.</span><span class="sxs-lookup"><span data-stu-id="b7298-149">Before you can run the app, you  need to bundle your code to ensure that all your modular dependencies are included in the final payload.</span></span> <span data-ttu-id="b7298-150">Если вы уже задав код приложения, вы можете пропустить этот шаг.</span><span class="sxs-lookup"><span data-stu-id="b7298-150">If you are already bundling your app code, you can skip this step.</span></span>
 
 #### <a name="install-webpack"></a><span data-ttu-id="b7298-151">Установка веб-упаковки</span><span class="sxs-lookup"><span data-stu-id="b7298-151">Install webpack</span></span>
 
 ```cmd 
 npm install webpack webpack-cli ts-loader --save-dev
 ```
 
 #### <a name="webpackconfigjs"></a><span data-ttu-id="b7298-152">webpack.config.js</span><span class="sxs-lookup"><span data-stu-id="b7298-152">webpack.config.js</span></span>
 
<span data-ttu-id="b7298-153">Создайте *новыйwebpack.config.js* файл в корневой папке проекта и вложите следующую конфигурацию.</span><span class="sxs-lookup"><span data-stu-id="b7298-153">Create a new *webpack.config.js* file in the root folder of your project, and paste the following configuration.</span></span>
 
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
 
 <span data-ttu-id="b7298-154">Как видите, передняя часть (процесс рендера) и задний (основной процесс) объединены отдельно.</span><span class="sxs-lookup"><span data-stu-id="b7298-154">As you can see, the front end (renderer process) and the back-end (main process), are bundled separately.</span></span> <span data-ttu-id="b7298-155">Это потому, что в Electron процесс рендера выполняется в контексте браузера, а основной процесс выполняется в контексте узла.</span><span class="sxs-lookup"><span data-stu-id="b7298-155">This is because in Electron, the renderer process runs in the browser context and the main process runs in the node context.</span></span>
 
 #### <a name="add-the-webpacking-script-in-packagejson"></a><span data-ttu-id="b7298-156">Добавление сценария веб-упаковки в ```package.json```</span><span class="sxs-lookup"><span data-stu-id="b7298-156">Add the webpacking script in ```package.json```</span></span>
 
 <span data-ttu-id="b7298-157">Добавьте ниже в ```scripts``` вашем ```package.json``` .</span><span class="sxs-lookup"><span data-stu-id="b7298-157">Add the following under ```scripts``` in your ```package.json```.</span></span>
 
 ```json
"scripts": {
   "webpack": "webpack",
   "start": "npm run webpack && electron dist/main.js"
 }                
 ```
 
 #### <a name="run-your-app"></a><span data-ttu-id="b7298-158">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="b7298-158">Run your app</span></span>
 
 ```cmd
 npm start
 ```

### <a name="add-token-caching-capabilities-to-your-app-and-enable-silent-sign-ins-advanced"></a><span data-ttu-id="b7298-159">Добавьте возможности кэшинга маркеров в приложение и встройте входы в бесшумный вход (расширенный)</span><span class="sxs-lookup"><span data-stu-id="b7298-159">Add token caching capabilities to your app and enable silent sign ins (advanced)</span></span>

<span data-ttu-id="b7298-160">Узел MSAL поддерживает кэш в памяти по умолчанию и предоставляет интерфейс ICachePlugin для выполнения сериализации кэша, но не предоставляет способ хранения кэша маркера на диск по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b7298-160">MSAL Node supports an in-memory cache by default and provides the ICachePlugin interface to perform cache serialization, but does not provide a default way of storing the token cache to disk.</span></span> <span data-ttu-id="b7298-161">Если вам требуется постоянное хранилище кэша для обеспечения бесшумных входных входов или межплатформенного кэширования, рекомендуется использовать реализацию по умолчанию, предоставленную узлом MSAL в качестве [расширения.](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions)</span><span class="sxs-lookup"><span data-stu-id="b7298-161">If you need persistent cache storage to enable silent sign ins or cross-platform caching, we recommend using the default implementation provided by MSAL Node as an [extension](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions).</span></span> <span data-ttu-id="b7298-162">Этот плагин можно импортировать и передавать экземпляр плагина кэша при инициализации. `ElectronAuthenticator`</span><span class="sxs-lookup"><span data-stu-id="b7298-162">You can import this plugin, and pass the instance of the cache plugin while initializing `ElectronAuthenticator`.</span></span>

```ts
let config: MsalElectronConfig = {
  ...
  cachePlugin: new PersistenceCachePlugin(filePersistence) //filePersistence is the instance of type IPersistence that you will need to create
};
```
<span data-ttu-id="b7298-163">Дополнительные сведения о том, как реализовать это, см. в примере [microsoft-authentication-library-for-js.](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/extensions/samples/msal-node-extensions/index.js)</span><span class="sxs-lookup"><span data-stu-id="b7298-163">For more details about how to implement this, see the [microsoft-authentication-library-for-js](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/extensions/samples/msal-node-extensions/index.js) sample.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b7298-164">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b7298-164">Next Steps</span></span>
- <span data-ttu-id="b7298-165">Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="b7298-165">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="b7298-166">Задайте вопрос [в Microsoft Q&A](https://aka.ms/askgraph).</span><span class="sxs-lookup"><span data-stu-id="b7298-166">Ask a question on [Microsoft Q&A](https://aka.ms/askgraph).</span></span>
- <span data-ttu-id="b7298-167">Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="b7298-167">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
    
