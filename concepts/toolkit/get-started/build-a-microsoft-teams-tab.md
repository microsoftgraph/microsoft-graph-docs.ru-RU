---
title: Создайте вкладку Microsoft Teams с помощью microsoft Graph набор средств
description: Начало создания вкладки Microsoft Teams с помощью microsoft Graph набор средств.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 7bd9d989d30b7fc4286a6ca78445ffb01a772084
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813169"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="e50e4-103">Создайте вкладку Microsoft Teams с помощью microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="e50e4-103">Build a Microsoft Teams tab with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="e50e4-104">В этом разделе описывается, как начать использовать microsoft Graph набор средств в Microsoft Teams решении.</span><span class="sxs-lookup"><span data-stu-id="e50e4-104">This topic covers how to get started using the Microsoft Graph Toolkit in a Microsoft Teams solution.</span></span> <span data-ttu-id="e50e4-105">Начало работы включает в себя следующие действия:</span><span class="sxs-lookup"><span data-stu-id="e50e4-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="e50e4-106">Создайте новое Teams с помощью настраиваемой вкладки.</span><span class="sxs-lookup"><span data-stu-id="e50e4-106">Create a new Teams application with a custom tab.</span></span>
2. <span data-ttu-id="e50e4-107">Добавьте microsoft Graph набор средств.</span><span class="sxs-lookup"><span data-stu-id="e50e4-107">Add the Microsoft Graph Toolkit.</span></span>
3. <span data-ttu-id="e50e4-108">Инициализация Microsoft Teams поставщика.</span><span class="sxs-lookup"><span data-stu-id="e50e4-108">Initialize the Microsoft Teams provider.</span></span>
4. <span data-ttu-id="e50e4-109">Создание всплываемой страницы auth.</span><span class="sxs-lookup"><span data-stu-id="e50e4-109">Create the auth popup page.</span></span>
5. <span data-ttu-id="e50e4-110">Добавление компонентов.</span><span class="sxs-lookup"><span data-stu-id="e50e4-110">Add components.</span></span>
6. <span data-ttu-id="e50e4-111">Проверьте приложение.</span><span class="sxs-lookup"><span data-stu-id="e50e4-111">Test your app.</span></span>

## <a name="create-a-new-teams-application-with-a-custom-tab"></a><span data-ttu-id="e50e4-112">Создание нового приложения Teams с помощью настраиваемой вкладки</span><span class="sxs-lookup"><span data-stu-id="e50e4-112">Create a new Teams application with a custom tab</span></span>

<span data-ttu-id="e50e4-113">Самый простой способ создания нового приложения Teams — использовать Microsoft Teams набор средств [для](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) Visual Studio Code.</span><span class="sxs-lookup"><span data-stu-id="e50e4-113">The easiest way to create a new Teams app is to use the [Microsoft Teams Toolkit extension](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) for Visual Studio Code.</span></span> <span data-ttu-id="e50e4-114">Следуйте инструкциям по настройкам нового [проекта Teams.](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)</span><span class="sxs-lookup"><span data-stu-id="e50e4-114">Follow the instructions to [set up a new Teams project](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project).</span></span> <span data-ttu-id="e50e4-115">Когда вы доберелись до экрана **Добавить возможности,** выберите **вкладку**, а затем **личные вкладки**.</span><span class="sxs-lookup"><span data-stu-id="e50e4-115">When you get to the **Add capabilities** screen, select **Tab**, and then **Personal tab**.</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="e50e4-116">Добавление Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="e50e4-116">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="e50e4-117">Используйте Microsoft Graph Toolkit в приложении, обратившись непосредственно к загрузчику (через unpkg) или установив пакет npm.</span><span class="sxs-lookup"><span data-stu-id="e50e4-117">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span> <span data-ttu-id="e50e4-118">Чтобы использовать набор средств, вам также потребуется Microsoft Teams [SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).</span><span class="sxs-lookup"><span data-stu-id="e50e4-118">To use the Toolkit, you will also need the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="e50e4-119">Использование с помощью mgt-loader</span><span class="sxs-lookup"><span data-stu-id="e50e4-119">Use via mgt-loader</span></span>
<span data-ttu-id="e50e4-120">Чтобы использовать набор средств и Teams SDK через загрузчики, добавьте в файл следующие `<head>` `public/index.html` ссылки:</span><span class="sxs-lookup"><span data-stu-id="e50e4-120">To use the Toolkit and the Teams SDK via the loaders, add the following references inside the `<head>` of the `public/index.html` file:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="e50e4-121">Использование через npm (модули ES6)</span><span class="sxs-lookup"><span data-stu-id="e50e4-121">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="e50e4-122">Использование Toolkit с помощью модулей ES6 обеспечивает полное управление процессом объединения и позволяет объединить только код, необходимый для приложения.</span><span class="sxs-lookup"><span data-stu-id="e50e4-122">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="e50e4-123">Чтобы использовать модули ES6, добавьте пакеты npm для набор средств и Microsoft Teams SDK в проект:</span><span class="sxs-lookup"><span data-stu-id="e50e4-123">To use the ES6 modules, add the npm packages for both the Toolkit and the Microsoft Teams SDK to your project:</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a><span data-ttu-id="e50e4-124">Инициализация Teams поставщика</span><span class="sxs-lookup"><span data-stu-id="e50e4-124">Initialize the Teams provider</span></span>

<span data-ttu-id="e50e4-125">Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="e50e4-125">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="e50e4-126">Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="e50e4-126">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="e50e4-127">Поставщик [Teams обрабатывает](../providers/teams.md) все логики и взаимодействия, которые необходимо реализовать с Teams SDK для проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="e50e4-127">The [Teams provider](../providers/teams.md) handles all of the logic and interactions that need to be implemented with the Teams SDK to authenticate the user.</span></span>

<span data-ttu-id="e50e4-128">Чтобы инициализировать поставщика, можно использовать HTML-код или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="e50e4-128">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

### <a name="initialize-in-html"></a><span data-ttu-id="e50e4-129">Инициализация в HTML</span><span class="sxs-lookup"><span data-stu-id="e50e4-129">Initialize in HTML</span></span>

<span data-ttu-id="e50e4-130">В `public/index.html` , добавьте Teams поставщика в , как `<body>` показано.</span><span class="sxs-lookup"><span data-stu-id="e50e4-130">In `public/index.html`, add the Teams provider into the `<body>`, as shown.</span></span>

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/auth.html"
></mgt-teams-provider>
```

<span data-ttu-id="e50e4-131">Замените `<YOUR_CLIENT_ID>` на идентификатор клиента для своего приложения.</span><span class="sxs-lookup"><span data-stu-id="e50e4-131">Replace `<YOUR_CLIENT_ID>` with the client ID for your application.</span></span> 

### <a name="initialize-in-javascript"></a><span data-ttu-id="e50e4-132">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="e50e4-132">Initialize in JavaScript</span></span>

<span data-ttu-id="e50e4-133">Чтобы инициализировать поставщика в коде JavaScript, найдите `src/components/App.js` файл в каталоге проекта.</span><span class="sxs-lookup"><span data-stu-id="e50e4-133">To initialize the provider in your JavaScript code, Locate the `src/components/App.js` file in your project directory.</span></span> <span data-ttu-id="e50e4-134">Импорт Teams поставщика и инициализация поставщика.</span><span class="sxs-lookup"><span data-stu-id="e50e4-134">Import the Teams Provider and initialize the provider.</span></span>

```JavaScript
import * as microsoftTeams from "@microsoft/teams-js";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
<span data-ttu-id="e50e4-135">Замените `<YOUR_CLIENT_ID>` на идентификатор клиента для своего приложения.</span><span class="sxs-lookup"><span data-stu-id="e50e4-135">Replace `<YOUR_CLIENT_ID>` with the client ID for your application.</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="e50e4-136">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="e50e4-136">Creating an app/client ID</span></span>

<span data-ttu-id="e50e4-137">Чтобы получить клиентский ID, необходимо зарегистрировать Azure Active Directory приложение.</span><span class="sxs-lookup"><span data-stu-id="e50e4-137">To get a client ID, you need to register an Azure Active Directory application.</span></span> <span data-ttu-id="e50e4-138">Выполните действия в статье [Создание Azure Active Directory приложения.](./add-aad-app-registration.md)</span><span class="sxs-lookup"><span data-stu-id="e50e4-138">Follow the steps in the [Create an Azure Active Directory app](./add-aad-app-registration.md) article.</span></span>

<span data-ttu-id="e50e4-139">Обязательно установите **URI перенаправления** в регистрации приложения, чтобы указать на `auth.html` страницу.</span><span class="sxs-lookup"><span data-stu-id="e50e4-139">Make sure to set the **redirect URI** in your app registration to point to your `auth.html` page.</span></span> <span data-ttu-id="e50e4-140">Например, если вы работаете с `localhost:3000` приложением, установите URI перенаправления. `https://localhost:3000/auth.html`</span><span class="sxs-lookup"><span data-stu-id="e50e4-140">For example, if you are running your app on `localhost:3000`, set the redirect URI to `https://localhost:3000/auth.html`.</span></span>

><span data-ttu-id="e50e4-141">**Примечание**. MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="e50e4-141">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="e50e4-142">Включите неявный поток в своем приложении на портале Azure (он не включен по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="e50e4-142">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="e50e4-143">В области **Проверка подлинности** найдите раздел **Неявное предоставление** и установите флажки **Маркеры доступа** и **Маркеры идентификаторов**.</span><span class="sxs-lookup"><span data-stu-id="e50e4-143">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="create-the-auth-popup-page"></a><span data-ttu-id="e50e4-144">Создание всплываемой страницы auth</span><span class="sxs-lookup"><span data-stu-id="e50e4-144">Create the auth popup page</span></span>

<span data-ttu-id="e50e4-145">Чтобы разрешить пользователям войти, необходимо указать URL-адрес, Teams приложение откроется в всплывающее приложение, чтобы следовать потоку проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e50e4-145">In order to allow users to sign in, you need to provide a URL that the Teams app will open in a popup to follow the authentication flow.</span></span> <span data-ttu-id="e50e4-146">URL-адрес должен быть в домене, и все, что нужно сделать на этой странице, это вызвать `TeamsProvider.handleAuth()` метод.</span><span class="sxs-lookup"><span data-stu-id="e50e4-146">The URL needs to be in your domain, and all this page needs to do is call the `TeamsProvider.handleAuth()` method.</span></span>

<span data-ttu-id="e50e4-147">Это можно сделать, добавив новый файл в папку (который должен быть на том же уровне, что и) и добавив `auth.html` `public` следующий `index.html` код:</span><span class="sxs-lookup"><span data-stu-id="e50e4-147">You can do this by adding a new `auth.html` file in the `public` folder (which should be at the same level as `index.html`) and adding the following code:</span></span> 

```html
<!DOCTYPE html>
<html>
  <head>
    <script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
    <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
  </head>

  <body>
    <script>
      mgt.TeamsProvider.handleAuth();
    </script>
  </body>
</html>
```

## <a name="add-components"></a><span data-ttu-id="e50e4-148">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="e50e4-148">Add components</span></span>

<span data-ttu-id="e50e4-149">Теперь вы готовы добавить любой из компонентов Microsoft Graph набор средств на вкладку.</span><span class="sxs-lookup"><span data-stu-id="e50e4-149">Now, you're ready to add any of the Microsoft Graph Toolkit components to your tab.</span></span> 

<span data-ttu-id="e50e4-150">Вы можете добавлять компоненты в HTML, как обычно.</span><span class="sxs-lookup"><span data-stu-id="e50e4-150">You can add components to your HTML as you normally would.</span></span> <span data-ttu-id="e50e4-151">Например, чтобы добавить компонент Login, добавьте ниже код в тело `index.html` вашего :</span><span class="sxs-lookup"><span data-stu-id="e50e4-151">For example, to add the Login component add the below code to the body of your `index.html`:</span></span>

```HTML
<mgt-login></mgt-login>
```

<span data-ttu-id="e50e4-152">Или можно добавить компоненты jSX в компонент Tab.</span><span class="sxs-lookup"><span data-stu-id="e50e4-152">Or, you can add the components in JSX to the Tab component.</span></span> <span data-ttu-id="e50e4-153">Рекомендуется использовать библиотеку, если вы создали `mgt-react` Teams приложение с помощью Microsoft Teams набор средств расширения.</span><span class="sxs-lookup"><span data-stu-id="e50e4-153">We recommend using the `mgt-react` library if you created your Teams app using the Microsoft Teams Toolkit extension.</span></span> <span data-ttu-id="e50e4-154">Дополнительные дополнительные ссылки см. в [Graph набор средств Microsoft React](./use-toolkit-with-react.md)</span><span class="sxs-lookup"><span data-stu-id="e50e4-154">To learn more, see [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md)</span></span>

<span data-ttu-id="e50e4-155">Во-первых, `mgt-react` установите:</span><span class="sxs-lookup"><span data-stu-id="e50e4-155">First, install `mgt-react`:</span></span>

```Command Line
npm install @microsoft/mgt-react
```

<span data-ttu-id="e50e4-156">Найдите `src/components/Tab.js` файл и импортируете компоненты, которые необходимо использовать из `mgt-react` библиотеки.</span><span class="sxs-lookup"><span data-stu-id="e50e4-156">Locate the `src/components/Tab.js` file and import the components you want to use from the `mgt-react` library.</span></span> <span data-ttu-id="e50e4-157">Например, чтобы добавить использование `Login` компонентов:</span><span class="sxs-lookup"><span data-stu-id="e50e4-157">For example, to add the `Login` component use:</span></span>

```JavaScript
import { Login } from "@microsoft/mgt-react"
```

<span data-ttu-id="e50e4-158">Затем добавьте компонент в утверждение `return()` метода `render()` `Tab` :</span><span class="sxs-lookup"><span data-stu-id="e50e4-158">Then, add the the component to the `return()` statement of the `render()` method of `Tab`:</span></span>

```JavaScript
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a><span data-ttu-id="e50e4-159">Тестирование приложения</span><span class="sxs-lookup"><span data-stu-id="e50e4-159">Test your application</span></span>

<span data-ttu-id="e50e4-160">Создайте и запустите приложение с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="e50e4-160">Build and run your application using the following commands:</span></span>
```bash
npm install
npm start
```

<span data-ttu-id="e50e4-161">Чтобы протестировать приложение, можно установить приложение для Teams с помощью Teams набор средств расширения.</span><span class="sxs-lookup"><span data-stu-id="e50e4-161">To test your application, you can install your app to Teams via the Teams Toolkit Extension.</span></span> <span data-ttu-id="e50e4-162">Откройте расширение Teams набор средств и нажмите **кнопку Открыть Microsoft Teams набор средств**.</span><span class="sxs-lookup"><span data-stu-id="e50e4-162">Open the Teams Toolkit Extension and click **Open Microsoft Teams Toolkit**.</span></span> <span data-ttu-id="e50e4-163">Щелкните **App Studio** в левом меню, прокрутите вниз и выберите Тест **и Распространение**, а затем **Установите**.</span><span class="sxs-lookup"><span data-stu-id="e50e4-163">Click **App Studio** in the left menu, scroll down and select **Test and Distribute**, then **Install**.</span></span> <span data-ttu-id="e50e4-164">Teams откроется в браузере, и вы будете перенаправлены на созданную вкладку.</span><span class="sxs-lookup"><span data-stu-id="e50e4-164">Teams will open in your browser, and you will be redirected to the tab you created.</span></span> <span data-ttu-id="e50e4-165">Вы должны иметь возможность видеть компонент Login и использовать его для входа в приложение.</span><span class="sxs-lookup"><span data-stu-id="e50e4-165">You should be able to see the Login component and use it to sign in to your application.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e50e4-166">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e50e4-166">Next Steps</span></span>
- <span data-ttu-id="e50e4-167">Ознакомьтесь с этим пошаговом руководстве по построению [вкладки Teams.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)</span><span class="sxs-lookup"><span data-stu-id="e50e4-167">Check out this step-by-step tutorial on [building a Teams tab](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).</span></span>
- <span data-ttu-id="e50e4-168">Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="e50e4-168">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="e50e4-169">Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="e50e4-169">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="e50e4-170">Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="e50e4-170">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
