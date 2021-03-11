---
title: Создайте вкладку Microsoft Teams с помощью microsoft Graph набор средств
description: Начало создания вкладки Microsoft Teams с помощью microsoft Graph набор средств.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 757c7eb8a94b0f6936a21f5ecb6f126cde36b6ad
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721567"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="56756-103">Создайте вкладку Microsoft Teams с помощью microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="56756-103">Build a Microsoft Teams tab with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="56756-104">В этом разделе описывается, как начать работу с помощью microsoft Graph набор средств в решении Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="56756-104">This topic covers how to get started using the Microsoft Graph Toolkit in a Microsoft Teams solution.</span></span> <span data-ttu-id="56756-105">Начало работы включает в себя следующие действия:</span><span class="sxs-lookup"><span data-stu-id="56756-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="56756-106">Создайте новое приложение Teams с помощью настраиваемой вкладки.</span><span class="sxs-lookup"><span data-stu-id="56756-106">Create a new Teams application with a custom tab.</span></span>
2. <span data-ttu-id="56756-107">Настройка ngrok и создание туннеля.</span><span class="sxs-lookup"><span data-stu-id="56756-107">Set up ngrok and create a tunnel.</span></span>
3. <span data-ttu-id="56756-108">Добавьте microsoft Graph набор средств.</span><span class="sxs-lookup"><span data-stu-id="56756-108">Add the Microsoft Graph Toolkit.</span></span>
4. <span data-ttu-id="56756-109">Инициализация поставщика Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="56756-109">Initialize the Microsoft Teams provider.</span></span>
5. <span data-ttu-id="56756-110">Создание всплываемой страницы auth.</span><span class="sxs-lookup"><span data-stu-id="56756-110">Create the auth popup page.</span></span>
6. <span data-ttu-id="56756-111">Добавление компонентов.</span><span class="sxs-lookup"><span data-stu-id="56756-111">Add components.</span></span>
7. <span data-ttu-id="56756-112">Проверьте приложение.</span><span class="sxs-lookup"><span data-stu-id="56756-112">Test your app.</span></span>

## <a name="create-a-new-teams-application-with-a-custom-tab"></a><span data-ttu-id="56756-113">Создание нового приложения Teams с помощью настраиваемой вкладки</span><span class="sxs-lookup"><span data-stu-id="56756-113">Create a new Teams application with a custom tab</span></span>

<span data-ttu-id="56756-114">Самый простой способ создания нового приложения Teams — использовать расширение [Microsoft Teams набор средств](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) для Visual Studio кода.</span><span class="sxs-lookup"><span data-stu-id="56756-114">The easiest way to create a new Teams app is to use the [Microsoft Teams Toolkit extension](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) for Visual Studio Code.</span></span> <span data-ttu-id="56756-115">Следуйте инструкциям по [настройкам нового проекта Teams.](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)</span><span class="sxs-lookup"><span data-stu-id="56756-115">Follow the instructions to [set up a new Teams project](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project).</span></span> <span data-ttu-id="56756-116">Когда вы доберелись до экрана **Добавить возможности,** выберите **вкладку**, а затем **личные вкладки**.</span><span class="sxs-lookup"><span data-stu-id="56756-116">When you get to the **Add capabilities** screen, select **Tab**, and then **Personal tab**.</span></span>

## <a name="set-up-ngrok-and-create-a-tunnel"></a><span data-ttu-id="56756-117">Настройка ngrok и создание туннеля</span><span class="sxs-lookup"><span data-stu-id="56756-117">Set up ngrok and create a tunnel</span></span>

<span data-ttu-id="56756-118">Чтобы протестировать приложение позже, необходимо будет использовать HTTPS-адрес с общедоступным URL-адресом.</span><span class="sxs-lookup"><span data-stu-id="56756-118">In order to test your application later, you will need to host your application over a public-facing URL using HTTPS.</span></span> <span data-ttu-id="56756-119">Установите [ngrok](https://ngrok.com/download) и создайте туннель из Интернета в localhost:3000 со следующей командой:</span><span class="sxs-lookup"><span data-stu-id="56756-119">Install [ngrok](https://ngrok.com/download) and create a tunnel from the Internet to localhost:3000 with the following command:</span></span>

```bash
ngrok http 3000
```
<span data-ttu-id="56756-120">В каталоге проектов найдите файл и замените значение `.publish\Development.env` `baseUrl0` url-адресом ngrok.</span><span class="sxs-lookup"><span data-stu-id="56756-120">In your project directory, locate the `.publish\Development.env` file and replace the value for `baseUrl0` with your ngrok URL.</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="56756-121">Добавление Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="56756-121">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="56756-122">Используйте Microsoft Graph Toolkit в приложении, обратившись непосредственно к загрузчику (через unpkg) или установив пакет npm.</span><span class="sxs-lookup"><span data-stu-id="56756-122">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span> <span data-ttu-id="56756-123">Чтобы использовать набор средств, вам также потребуется [SDK Microsoft Teams.](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)</span><span class="sxs-lookup"><span data-stu-id="56756-123">To use the Toolkit, you will also need the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="56756-124">Использование с помощью mgt-loader</span><span class="sxs-lookup"><span data-stu-id="56756-124">Use via mgt-loader</span></span>
<span data-ttu-id="56756-125">Чтобы использовать набор средств и команд SDK через погрузчики, добавьте следующие ссылки `public/index.html` на:</span><span class="sxs-lookup"><span data-stu-id="56756-125">To use the Toolkit and the Teams SDK via the loaders, add the following references to `public/index.html`:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="56756-126">Использование через npm (модули ES6)</span><span class="sxs-lookup"><span data-stu-id="56756-126">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="56756-127">Использование Toolkit с помощью модулей ES6 обеспечивает полное управление процессом объединения и позволяет объединить только код, необходимый для приложения.</span><span class="sxs-lookup"><span data-stu-id="56756-127">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="56756-128">Чтобы использовать модули ES6, добавьте пакеты npm как для набор средств, так и для SDK Microsoft Teams:</span><span class="sxs-lookup"><span data-stu-id="56756-128">To use the ES6 modules, add the npm packages for both the Toolkit and the Microsoft Teams SDK to your project:</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a><span data-ttu-id="56756-129">Инициализация поставщика Teams</span><span class="sxs-lookup"><span data-stu-id="56756-129">Initialize the Teams provider</span></span>

<span data-ttu-id="56756-130">Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="56756-130">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="56756-131">Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="56756-131">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="56756-132">Поставщик [Teams обрабатывает](../providers/teams.md) все логики и взаимодействия, которые необходимо реализовать с командой SDK для проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="56756-132">The [Teams provider](../providers/teams.md) handles all of the logic and interactions that need to be implemented with the Teams SDK to authenticate the user.</span></span>

<span data-ttu-id="56756-133">Чтобы инициализировать поставщика, можно использовать HTML-код или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="56756-133">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

### <a name="initialize-in-html"></a><span data-ttu-id="56756-134">Инициализация в HTML</span><span class="sxs-lookup"><span data-stu-id="56756-134">Initialize in HTML</span></span>

<span data-ttu-id="56756-135">В `public/index.html` , добавьте поставщика Teams, как показано.</span><span class="sxs-lookup"><span data-stu-id="56756-135">In `public/index.html`, add the Teams provider as shown.</span></span>

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

<span data-ttu-id="56756-136">Замените `<YOUR_CLIENT_ID>` с помощью клиентского ИД для приложения и `<YOUR_NGROK_URL>` созданного URL-адреса ngrok.</span><span class="sxs-lookup"><span data-stu-id="56756-136">Replace `<YOUR_CLIENT_ID>` with the client ID for your application and `<YOUR_NGROK_URL>` with the ngrok URL you created.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="56756-137">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="56756-137">Initialize in JavaScript</span></span>

<span data-ttu-id="56756-138">Чтобы инициализировать поставщика в коде JavaScript, найдите `src/components/App.js` файл в каталоге проекта.</span><span class="sxs-lookup"><span data-stu-id="56756-138">To initialize the provider in your JavaScript code, Locate the `src/components/App.js` file in your project directory.</span></span> <span data-ttu-id="56756-139">Импорт поставщика teams и инициализация поставщика.</span><span class="sxs-lookup"><span data-stu-id="56756-139">Import the Teams Provider and initialize the provider.</span></span>

```js
import * as microsoftTeams from "@microsoft/teams-js";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
<span data-ttu-id="56756-140">Замените `<YOUR_CLIENT_ID>` на идентификатор клиента для своего приложения.</span><span class="sxs-lookup"><span data-stu-id="56756-140">Replace `<YOUR_CLIENT_ID>` with the client ID for your application.</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="56756-141">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="56756-141">Creating an app/client ID</span></span>
<span data-ttu-id="56756-142">Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](../../auth-register-app-v2.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="56756-142">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> <span data-ttu-id="56756-143">Обязательно добавьте URL-адрес ngrok с полным путем к всплываемой странице auth в URL-адреса перенаправления (например, `https://<YOUR_NGROK_URL>/auth.html` ).</span><span class="sxs-lookup"><span data-stu-id="56756-143">Make sure to add your ngrok URL with the full path to the auth popup page to your redirect URIs (for example, `https://<YOUR_NGROK_URL>/auth.html`).</span></span>
><span data-ttu-id="56756-144">**Примечание**. MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="56756-144">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="56756-145">Включите неявный поток в своем приложении на портале Azure (он не включен по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="56756-145">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="56756-146">В области **Проверка подлинности** найдите раздел **Неявное предоставление** и установите флажки **Маркеры доступа** и **Маркеры идентификаторов**.</span><span class="sxs-lookup"><span data-stu-id="56756-146">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="create-the-auth-popup-page"></a><span data-ttu-id="56756-147">Создание всплываемой страницы auth</span><span class="sxs-lookup"><span data-stu-id="56756-147">Create the auth popup page</span></span>

<span data-ttu-id="56756-148">Чтобы разрешить пользователям войти, необходимо указать URL-адрес, который приложение Teams откроет в всплывающее приложение, чтобы следовать потоку проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="56756-148">In order to allow users to sign in, you need to provide a URL that the Teams app will open in a popup to follow the authentication flow.</span></span> <span data-ttu-id="56756-149">URL-адрес должен быть в домене, и все, что нужно сделать на этой странице, это вызвать `TeamsProvider.handleAuth()` метод.</span><span class="sxs-lookup"><span data-stu-id="56756-149">The URL needs to be in your domain, and all this page needs to do is call the `TeamsProvider.handleAuth()` method.</span></span>

<span data-ttu-id="56756-150">Вы можете сделать это в HTML, добавив новый файл в папку (который должен быть на том же уровне, что и) и добавив `auth.html` `public` следующий `index.html` код:</span><span class="sxs-lookup"><span data-stu-id="56756-150">You can do this in your HTML by adding a new `auth.html` file in the `public` folder (which should be at the same level as `index.html`) and adding the following code:</span></span> 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a><span data-ttu-id="56756-151">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="56756-151">Add components</span></span>

<span data-ttu-id="56756-152">Теперь вы готовы добавить в вкладку любой набор средств Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="56756-152">Now, you're ready to add any of the Microsoft Graph Toolkit components to your tab.</span></span> 

<span data-ttu-id="56756-153">Вы можете добавлять компоненты в HTML, как обычно.</span><span class="sxs-lookup"><span data-stu-id="56756-153">You can add components to your HTML as you normally would.</span></span> <span data-ttu-id="56756-154">Например, чтобы добавить компонент Login, добавьте ниже код в тело `index.html` вашего :</span><span class="sxs-lookup"><span data-stu-id="56756-154">For example, to add the Login component add the below code to the body of your `index.html`:</span></span>

```html
<mgt-login></mgt-login>
```

<span data-ttu-id="56756-155">Или можно добавить компоненты jSX в компонент Tab.</span><span class="sxs-lookup"><span data-stu-id="56756-155">Or, you can add the components in JSX to the Tab component.</span></span> <span data-ttu-id="56756-156">Рекомендуется использовать библиотеку, если вы создали приложение Teams с помощью расширения `mgt-react` Microsoft Teams набор средств.</span><span class="sxs-lookup"><span data-stu-id="56756-156">We recommend using the `mgt-react` library if you created your Teams app using the Microsoft Teams Toolkit extension.</span></span> <span data-ttu-id="56756-157">Дополнительные данные см. в [набор средств Microsoft Graph с React](./use-toolkit-with-react.md)</span><span class="sxs-lookup"><span data-stu-id="56756-157">To learn more, see [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md)</span></span>

<span data-ttu-id="56756-158">Во-первых, `mgt-react` установите:</span><span class="sxs-lookup"><span data-stu-id="56756-158">First, install `mgt-react`:</span></span>

```bash
npm install @microsoft/mgt-react
```

<span data-ttu-id="56756-159">Найдите `src/components/Tab.js` файл и импортируете компоненты, которые необходимо использовать из `mgt-react` библиотеки.</span><span class="sxs-lookup"><span data-stu-id="56756-159">Locate the `src/components/Tab.js` file and import the components you want to use from the `mgt-react` library.</span></span> <span data-ttu-id="56756-160">Например, чтобы добавить использование `Login` компонентов:</span><span class="sxs-lookup"><span data-stu-id="56756-160">For example, to add the `Login` component use:</span></span>

```js
import { Login } from "@microsoft/mgt-react"
```

<span data-ttu-id="56756-161">Затем добавьте компонент в утверждение `return()` метода `render()` `Tab` :</span><span class="sxs-lookup"><span data-stu-id="56756-161">Then, add the the component to the `return()` statement of the `render()` method of `Tab`:</span></span>

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a><span data-ttu-id="56756-162">Тестирование приложения</span><span class="sxs-lookup"><span data-stu-id="56756-162">Test your application</span></span>

<span data-ttu-id="56756-163">Создайте и запустите приложение с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="56756-163">Build and run your application using the following commands:</span></span>
```bash
npm install
npm start
```

<span data-ttu-id="56756-164">Чтобы протестировать приложение, необходимо загрузить приложение в Teams.</span><span class="sxs-lookup"><span data-stu-id="56756-164">To test your application, you need to upload your application to Teams.</span></span> <span data-ttu-id="56756-165">Откройте клиент Microsoft Teams, выберите **... в левом** меню и перейдите в **App Studio**.</span><span class="sxs-lookup"><span data-stu-id="56756-165">Open the Microsoft Teams client, select the **...** on the left-hand menu and go to **App Studio**.</span></span> <span data-ttu-id="56756-166">Щелкните **вкладку Редактор Манифеста** и **выберите Импорт существующего приложения.**</span><span class="sxs-lookup"><span data-stu-id="56756-166">Click the **Manifest Editor** tab and select **Import an existing app**.</span></span>

<span data-ttu-id="56756-167">Найдите каталог проекта и загрузите **Development.zip** файл внутри **папки .publish.**</span><span class="sxs-lookup"><span data-stu-id="56756-167">Locate your project directory and upload the **Development.zip** file inside of the **.publish** folder.</span></span>

<span data-ttu-id="56756-168">После загрузки приложения прокрутите в левом меню и выберите **Test and Distribute**.</span><span class="sxs-lookup"><span data-stu-id="56756-168">After your app has loaded, scroll down on the left menu and select **Test and Distribute**.</span></span> <span data-ttu-id="56756-169">Нажмите **кнопку Установка** и нажмите кнопку **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="56756-169">Click the **Install** button and then click **Add**.</span></span> <span data-ttu-id="56756-170">Вы будете перенаправлены на созданную вкладку.</span><span class="sxs-lookup"><span data-stu-id="56756-170">You will be redirected to the tab you created.</span></span>

## <a name="next-steps"></a><span data-ttu-id="56756-171">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="56756-171">Next Steps</span></span>
- <span data-ttu-id="56756-172">Ознакомьтесь с этим пошаговом руководстве по [построению вкладки Teams.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)</span><span class="sxs-lookup"><span data-stu-id="56756-172">Check out this step-by-step tutorial on [building a Teams tab](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).</span></span>
- <span data-ttu-id="56756-173">Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="56756-173">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="56756-174">Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="56756-174">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="56756-175">Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="56756-175">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
