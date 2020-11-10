---
title: Создание вкладки Microsoft Teams с набором средств Microsoft Graph
description: Приступая к созданию вкладки Microsoft Teams с помощью набора инструментов Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 0f93e041208fb22e3131c2eb4619379188c76f56
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978768"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="9c1e6-103">Создание вкладки Microsoft Teams с набором средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9c1e6-103">Build a Microsoft Teams tab with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9c1e6-104">В этом разделе описывается, как приступить к использованию набора средств Microsoft Graph в решении Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-104">This topic covers how to get started using the Microsoft Graph Toolkit in a Microsoft Teams solution.</span></span> <span data-ttu-id="9c1e6-105">Приступая к работе состоит из следующих этапов:</span><span class="sxs-lookup"><span data-stu-id="9c1e6-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="9c1e6-106">Создайте новое приложение Teams с настраиваемой вкладкой.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-106">Create a new Teams application with a custom tab.</span></span>
2. <span data-ttu-id="9c1e6-107">Настройка ngrok и создание туннеля.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-107">Set up ngrok and create a tunnel.</span></span>
3. <span data-ttu-id="9c1e6-108">Добавьте набор инструментов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-108">Add the Microsoft Graph Toolkit.</span></span>
4. <span data-ttu-id="9c1e6-109">Инициализация поставщика Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-109">Initialize the Microsoft Teams provider.</span></span>
5. <span data-ttu-id="9c1e6-110">Создайте всплывающую страницу проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-110">Create the auth popup page.</span></span>
6. <span data-ttu-id="9c1e6-111">Добавление компонентов.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-111">Add components.</span></span>
7. <span data-ttu-id="9c1e6-112">Протестируйте приложение.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-112">Test your app.</span></span>

## <a name="create-a-new-teams-application-with-a-custom-tab"></a><span data-ttu-id="9c1e6-113">Создание нового приложения Teams с настраиваемой вкладкой</span><span class="sxs-lookup"><span data-stu-id="9c1e6-113">Create a new Teams application with a custom tab</span></span>

<span data-ttu-id="9c1e6-114">Самый простой способ создать приложение Teams — использовать [расширение набора средств Microsoft Teams](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) для Visual Studio Code.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-114">The easiest way to create a new Teams app is to use the [Microsoft Teams Toolkit extension](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) for Visual Studio Code.</span></span> <span data-ttu-id="9c1e6-115">Следуйте инструкциям по [настройке нового проекта Teams](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project).</span><span class="sxs-lookup"><span data-stu-id="9c1e6-115">Follow the instructions to [set up a new Teams project](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project).</span></span> <span data-ttu-id="9c1e6-116">При **переходе** на экран **добавить возможности** выберите **вкладку** , а затем щелкните Личные.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-116">When you get to the **Add capabilities** screen, select **Tab** , and then **Personal tab**.</span></span>

## <a name="set-up-ngrok-and-create-a-tunnel"></a><span data-ttu-id="9c1e6-117">Настройка ngrok и создание туннеля</span><span class="sxs-lookup"><span data-stu-id="9c1e6-117">Set up ngrok and create a tunnel</span></span>

<span data-ttu-id="9c1e6-118">Чтобы протестировать приложение позже, вам потребуется разместить приложение по общедоступному URL-адресу с помощью HTTPS.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-118">In order to test your application later, you will need to host your application over a public-facing URL using HTTPS.</span></span> <span data-ttu-id="9c1e6-119">Установите [ngrok](https://ngrok.com/download) и создайте туннель из Интернета на localhost: 3000 с помощью следующей команды:</span><span class="sxs-lookup"><span data-stu-id="9c1e6-119">Install [ngrok](https://ngrok.com/download) and create a tunnel from the Internet to localhost:3000 with the following command:</span></span>

```bash
ngrok http 3000
```
<span data-ttu-id="9c1e6-120">В каталоге проекта выберите `.publish\Development.env` файл и замените значение на `baseUrl0` URL-адрес ngrok.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-120">In your project directory, locate the `.publish\Development.env` file and replace the value for `baseUrl0` with your ngrok URL.</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="9c1e6-121">Добавление набора средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9c1e6-121">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9c1e6-122">Вы можете использовать набор средств Microsoft Graph в приложении, обратившись непосредственно к загрузчику (через унпкг) или установив пакет NPM.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-122">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span> <span data-ttu-id="9c1e6-123">Чтобы использовать набор средств, вам также понадобится [пакет SDK Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).</span><span class="sxs-lookup"><span data-stu-id="9c1e6-123">To use the Toolkit, you will also need the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="9c1e6-124">Использование с помощью упр. загрузчиком</span><span class="sxs-lookup"><span data-stu-id="9c1e6-124">Use via mgt-loader</span></span>
<span data-ttu-id="9c1e6-125">Чтобы использовать набор средств и пакет SDK Teams с помощью загрузчиков, добавьте следующие ссылки `public/index.html` :</span><span class="sxs-lookup"><span data-stu-id="9c1e6-125">To use the Toolkit and the Teams SDK via the loaders, add the following references to `public/index.html`:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="9c1e6-126">Использование через NPM (модули ES6)</span><span class="sxs-lookup"><span data-stu-id="9c1e6-126">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="9c1e6-127">Использование набора средств с помощью модулей ES6 даст вам полный контроль над процессом создания пучка и позволяет объединить только код, который требуется для приложения.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-127">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="9c1e6-128">Чтобы использовать модули ES6, добавьте в проект пакеты NPM для набора средств и пакета SDK Microsoft teams:</span><span class="sxs-lookup"><span data-stu-id="9c1e6-128">To use the ES6 modules, add the npm packages for both the Toolkit and the Microsoft Teams SDK to your project:</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a><span data-ttu-id="9c1e6-129">Инициализация поставщика Teams</span><span class="sxs-lookup"><span data-stu-id="9c1e6-129">Initialize the Teams provider</span></span>

<span data-ttu-id="9c1e6-130">Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-130">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="9c1e6-131">Чтобы узнать больше, ознакомьтесь со статьей [Использование поставщиков](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="9c1e6-131">To learn more, see [Using the providers](../providers.md).</span></span> <span data-ttu-id="9c1e6-132">[Поставщик Teams](../providers/teams.md) обрабатывает всю логику и взаимодействия, которые необходимо реализовать с помощью пакета SDK Teams для проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-132">The [Teams provider](../providers/teams.md) handles all of the logic and interactions that need to be implemented with the Teams SDK to authenticate the user.</span></span>

<span data-ttu-id="9c1e6-133">Для инициализации поставщика можно использовать HTML-код или код JavaScript.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-133">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

### <a name="initialize-in-html"></a><span data-ttu-id="9c1e6-134">Инициализация в HTML</span><span class="sxs-lookup"><span data-stu-id="9c1e6-134">Initialize in HTML</span></span>

<span data-ttu-id="9c1e6-135">`public/index.html`Добавьте поставщика Teams, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-135">In `public/index.html`, add the Teams provider as shown.</span></span>

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

<span data-ttu-id="9c1e6-136">Замените `<YOUR_CLIENT_ID>` идентификатором клиента для вашего приложения и `<YOUR_NGROK_URL>` созданным URL-адресом ngrok.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-136">Replace `<YOUR_CLIENT_ID>` with the client ID for your application and `<YOUR_NGROK_URL>` with the ngrok URL you created.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="9c1e6-137">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c1e6-137">Initialize in JavaScript</span></span>

<span data-ttu-id="9c1e6-138">Чтобы инициализировать поставщик в коде JavaScript, откройте `src/components/App.js` файл в каталоге проекта.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-138">To initialize the provider in your JavaScript code, Locate the `src/components/App.js` file in your project directory.</span></span> <span data-ttu-id="9c1e6-139">Импортируйте поставщика Teams и инициализируйте поставщик.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-139">Import the Teams Provider and initialize the provider.</span></span>

```js
import * as microsoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
<span data-ttu-id="9c1e6-140">Замените `<YOUR_CLIENT_ID>` идентификатором клиента для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-140">Replace `<YOUR_CLIENT_ID>` with the client ID for your application.</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="9c1e6-141">Создание идентификатора приложения или клиента</span><span class="sxs-lookup"><span data-stu-id="9c1e6-141">Creating an app/client ID</span></span>
<span data-ttu-id="9c1e6-142">Чтобы получить идентификатор клиента, необходимо [зарегистрировать приложение](../../auth-register-app-v2.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-142">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> <span data-ttu-id="9c1e6-143">Обязательно добавьте URL-адрес ngrok с полным путем к всплывающей странице проверки подлинности в URI перенаправления (например, `https://<YOUR_NGROK_URL>/auth.html` ).</span><span class="sxs-lookup"><span data-stu-id="9c1e6-143">Make sure to add your ngrok URL with the full path to the auth popup page to your redirect URIs (for example, `https://<YOUR_NGROK_URL>/auth.html`).</span></span>
><span data-ttu-id="9c1e6-144">**Note** : MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-144">**Note** : MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="9c1e6-145">Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен).</span><span class="sxs-lookup"><span data-stu-id="9c1e6-145">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="9c1e6-146">В разделе **Проверка подлинности** найдите раздел **неявный предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-146">Under **Authentication** , find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="create-the-auth-popup-page"></a><span data-ttu-id="9c1e6-147">Создание всплывающей страницы проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9c1e6-147">Create the auth popup page</span></span>

<span data-ttu-id="9c1e6-148">Чтобы разрешить пользователям входить в систему, необходимо указать URL-адрес, который приложение Teams будет открывать во всплывающем окне, чтобы выполнить этот процесс проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-148">In order to allow users to sign in, you need to provide a URL that the Teams app will open in a popup to follow the authentication flow.</span></span> <span data-ttu-id="9c1e6-149">URL-адрес должен находиться в вашем домене, и вся эта страница должна быть вызвана `TeamsProvider.handleAuth()` методом.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-149">The URL needs to be in your domain, and all this page needs to do is call the `TeamsProvider.handleAuth()` method.</span></span>

<span data-ttu-id="9c1e6-150">Это можно сделать в HTML-коде, добавив новый `auth.html` файл в `public` папку (который должен находиться на том же уровне, что `index.html` и), и добавьте следующий код:</span><span class="sxs-lookup"><span data-stu-id="9c1e6-150">You can do this in your HTML by adding a new `auth.html` file in the `public` folder (which should be at the same level as `index.html`) and adding the following code:</span></span> 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a><span data-ttu-id="9c1e6-151">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="9c1e6-151">Add components</span></span>

<span data-ttu-id="9c1e6-152">Теперь вы готовы добавить на вкладку любой из компонентов набора средств Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-152">Now, you're ready to add any of the Microsoft Graph Toolkit components to your tab.</span></span> 

<span data-ttu-id="9c1e6-153">Вы можете добавлять компоненты в HTML-код обычным образом.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-153">You can add components to your HTML as you normally would.</span></span> <span data-ttu-id="9c1e6-154">Например, чтобы добавить компонент входа, добавьте приведенный ниже код в текст `index.html` :</span><span class="sxs-lookup"><span data-stu-id="9c1e6-154">For example, to add the Login component add the below code to the body of your `index.html`:</span></span>

```html
<mgt-login></mgt-login>
```

<span data-ttu-id="9c1e6-155">Кроме того, вы можете добавить компоненты в ЖСКС в компонент табуляции.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-155">Or, you can add the components in JSX to the Tab component.</span></span> <span data-ttu-id="9c1e6-156">Мы рекомендуем использовать `mgt-react` библиотеку, если вы создали приложение Teams с помощью расширения набора средств Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-156">We recommend using the `mgt-react` library if you created your Teams app using the Microsoft Teams Toolkit extension.</span></span> <span data-ttu-id="9c1e6-157">Дополнительные сведения см. [Использование набора инструментов Microsoft Graph с откликом](./use-toolkit-with-react.md)</span><span class="sxs-lookup"><span data-stu-id="9c1e6-157">To learn more, see [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md)</span></span>

<span data-ttu-id="9c1e6-158">Сначала установите `mgt-react` :</span><span class="sxs-lookup"><span data-stu-id="9c1e6-158">First, install `mgt-react`:</span></span>

```bash
npm install @microsoft/mgt-react
```

<span data-ttu-id="9c1e6-159">Выберите `src/components/Tab.js` файл и импортируйте компоненты, которые вы хотите использовать, из `mgt-react` библиотеки.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-159">Locate the `src/components/Tab.js` file and import the components you want to use from the `mgt-react` library.</span></span> <span data-ttu-id="9c1e6-160">Например, чтобы добавить компонент, выполните `Login` следующие действия:</span><span class="sxs-lookup"><span data-stu-id="9c1e6-160">For example to add the `Login` component use:</span></span>

```js
import { Login } from "@microsoft/mgt-react"
```

<span data-ttu-id="9c1e6-161">Затем добавьте компонент в `return()` оператор `render()` метода метода `Tab` :</span><span class="sxs-lookup"><span data-stu-id="9c1e6-161">Then, add the the component to the `return()` statement of the `render()` method of `Tab`:</span></span>

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a><span data-ttu-id="9c1e6-162">Тестирование приложения</span><span class="sxs-lookup"><span data-stu-id="9c1e6-162">Test your application</span></span>

<span data-ttu-id="9c1e6-163">Постройте и запустите приложение с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="9c1e6-163">Build and run your application using the following commands:</span></span>
```bash
npm install
npm start
```

<span data-ttu-id="9c1e6-164">Чтобы протестировать приложение, необходимо загрузить приложение в Teams.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-164">To test your application, you need to upload your application to Teams.</span></span> <span data-ttu-id="9c1e6-165">Откройте клиент Microsoft Teams, выберите пункт **...** в левом меню и перейдите в **Приложение App Studio**.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-165">Open the Microsoft Teams client, select the **...** on the left-hand menu and go to **App Studio**.</span></span> <span data-ttu-id="9c1e6-166">Перейдите на вкладку **редактор манифестов** и выберите пункт **Импорт существующего приложения**.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-166">Click the **Manifest Editor** tab and select **Import an existing app**.</span></span>

<span data-ttu-id="9c1e6-167">Откройте каталог проекта и отправьте файл **Development.zip** в папку **. Publish** .</span><span class="sxs-lookup"><span data-stu-id="9c1e6-167">Locate your project directory and upload the **Development.zip** file inside of the **.publish** folder.</span></span>

<span data-ttu-id="9c1e6-168">После загрузки приложения Прокрутите меню слева вниз и выберите команду **проверить и распределить**.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-168">After your app has loaded, scroll down on the left menu and select **Test and Distribute**.</span></span> <span data-ttu-id="9c1e6-169">Нажмите кнопку **установить** , а затем кнопку **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-169">Click the **Install** button and then click **Add**.</span></span> <span data-ttu-id="9c1e6-170">Вы будете перенаправлены на созданную вами вкладку.</span><span class="sxs-lookup"><span data-stu-id="9c1e6-170">You will be redirected to the tab you created.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9c1e6-171">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="9c1e6-171">Next Steps</span></span>
- <span data-ttu-id="9c1e6-172">Ознакомьтесь с пошаговыми руководствами по [созданию вкладки Teams](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).</span><span class="sxs-lookup"><span data-stu-id="9c1e6-172">Check out this step-by-step tutorial on [building a Teams tab](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).</span></span>
- <span data-ttu-id="9c1e6-173">Опробуйте компоненты в [интерактивная среда](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="9c1e6-173">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="9c1e6-174">Задайте вопрос о [переполнении стека](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="9c1e6-174">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="9c1e6-175">Сообщать об ошибках или оставлять запрос на функцию в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="9c1e6-175">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>