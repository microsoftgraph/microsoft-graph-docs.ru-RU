---
title: Создание веб-приложения с помощью microsoft Graph набор средств
description: Начало создания веб-приложения с помощью microsoft Graph набор средств.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 73e61e9d2c1c453ec67e61dce1f088b5119d1e8d
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664018"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="84b39-103">Создание веб-приложения с помощью microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="84b39-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="84b39-104">В этом разделе описывается, как начать работу с microsoft Graph набор средств в веб-приложении, написанном на javaScript.</span><span class="sxs-lookup"><span data-stu-id="84b39-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="84b39-105">Если вы хотите узнать, как использовать веб-набор средств с веб-структурой, см. создание веб-приложения [(React)](./use-toolkit-with-react.md) или создание веб-приложения [(Angular).](./use-toolkit-with-angular.md)</span><span class="sxs-lookup"><span data-stu-id="84b39-105">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="84b39-106">Начало работы с microsoft Graph набор средств состоит из следующих этапов:</span><span class="sxs-lookup"><span data-stu-id="84b39-106">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="84b39-107">Добавьте microsoft Graph набор средств в свой проект.</span><span class="sxs-lookup"><span data-stu-id="84b39-107">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="84b39-108">Инициализация поставщика MSAL.</span><span class="sxs-lookup"><span data-stu-id="84b39-108">Initialize the MSAL Provider.</span></span>
3. <span data-ttu-id="84b39-109">Добавление компонентов.</span><span class="sxs-lookup"><span data-stu-id="84b39-109">Add components.</span></span>
4. <span data-ttu-id="84b39-110">Протестировать приложение.</span><span class="sxs-lookup"><span data-stu-id="84b39-110">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="84b39-111">Добавление в проект набор средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="84b39-111">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="84b39-112">Вы можете использовать microsoft Graph набор средств в приложении, ссылаясь на загрузчик напрямую (с помощью unpkg) или установив пакет npm.</span><span class="sxs-lookup"><span data-stu-id="84b39-112">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="84b39-113">unpkg</span><span class="sxs-lookup"><span data-stu-id="84b39-113">unpkg</span></span>](#tab/html)
<span data-ttu-id="84b39-114">Чтобы использовать набор средств mgt-loader, добавьте ссылку в сценарии в код:</span><span class="sxs-lookup"><span data-stu-id="84b39-114">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="84b39-115">npm</span><span class="sxs-lookup"><span data-stu-id="84b39-115">npm</span></span>](#tab/npm)
<span data-ttu-id="84b39-116">Использование набор средств с помощью модулей ES6 дает полный контроль над процессом пакетизации и позволяет объединить только код, необходимый для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="84b39-116">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="84b39-117">Чтобы использовать модули ES6, добавьте пакет npm в проект:</span><span class="sxs-lookup"><span data-stu-id="84b39-117">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---


> <span data-ttu-id="84b39-118">**Примечание.** Если вы нацелились на браузер, такой как IE11, который не поддерживает веб-компоненты по умолчанию, может потребоваться включить [полифайли.](./overview.md#polyfills)</span><span class="sxs-lookup"><span data-stu-id="84b39-118">**Note**: If you're targeting a browser such as IE11 that does not support web components natively, you might need to [include polyfills](./overview.md#polyfills).</span></span>

## <a name="initialize-the-msal-provider"></a><span data-ttu-id="84b39-119">Инициализация поставщика MSAL</span><span class="sxs-lookup"><span data-stu-id="84b39-119">Initialize the MSAL Provider</span></span>
<span data-ttu-id="84b39-120">Поставщики набор средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="84b39-120">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="84b39-121">Дополнительные см. [в этой теме.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="84b39-121">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="84b39-122">Поставщик [MSAL использует](../providers/msal.md) MSAL.js для регистрации пользователей и получения маркеров.</span><span class="sxs-lookup"><span data-stu-id="84b39-122">The [MSAL Provider](../providers/msal.md) uses MSAL.js to sign in users and acquire tokens.</span></span> <span data-ttu-id="84b39-123">Вы можете инициализировать поставщика MSAL в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="84b39-123">You can initialize the MSAL provider in your HTML or JavaScript.</span></span>

<span data-ttu-id="84b39-124">Если вы хотите использовать собственную проверку подлинности [](../providers/proxy.md) на сервере, используйте поставщика прокси-сервера, а не поставщика MSAL.</span><span class="sxs-lookup"><span data-stu-id="84b39-124">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL provider.</span></span>

<span data-ttu-id="84b39-125">Вы можете инициализировать поставщика в коде HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="84b39-125">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="84b39-126">html</span><span class="sxs-lookup"><span data-stu-id="84b39-126">html</span></span>](#tab/HTML)
<span data-ttu-id="84b39-127">Добавьте компонент `mgt-msal-provider` на HTML-страницу и задайте для нее код `client-id` клиента приложения.</span><span class="sxs-lookup"><span data-stu-id="84b39-127">Add the `mgt-msal-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
# <a name="js"></a>[<span data-ttu-id="84b39-128">js</span><span class="sxs-lookup"><span data-stu-id="84b39-128">js</span></span>](#tab/JavaScript)
<span data-ttu-id="84b39-129">Чтобы инициализировать поставщика MSAL в JavaScript, добавьте в приложение следующий код:</span><span class="sxs-lookup"><span data-stu-id="84b39-129">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


<span data-ttu-id="84b39-130">ИД клиента — это единственное свойство, необходимое для инициализации поставщика, но можно настроить дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="84b39-130">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="84b39-131">Полный список см. в [списке Msal Provider.](../providers/msal.md)</span><span class="sxs-lookup"><span data-stu-id="84b39-131">For the full list, see [Msal Provider](../providers/msal.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="84b39-132">Создание приложения или ИД клиента</span><span class="sxs-lookup"><span data-stu-id="84b39-132">Creating an app/client ID</span></span>
<span data-ttu-id="84b39-133">Чтобы получить ИД клиента, необходимо зарегистрировать приложение [в](./add-aad-app-registration.md) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84b39-133">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span> 
><span data-ttu-id="84b39-134">**Примечание.** MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="84b39-134">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="84b39-135">Обязательно включите неявный поток в приложении на портале Azure (по умолчанию он не включен).</span><span class="sxs-lookup"><span data-stu-id="84b39-135">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="84b39-136">В **разделе "Проверка подлинности"** найдите раздел неявного предоставления и выберите для маркеров **доступа** и **маркеров ID** свои почтовые ящики. </span><span class="sxs-lookup"><span data-stu-id="84b39-136">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="add-components"></a><span data-ttu-id="84b39-137">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="84b39-137">Add components</span></span>
<span data-ttu-id="84b39-138">После инициализации поставщика MSAL можно приступить к использованию любого из набор средств компонентов.</span><span class="sxs-lookup"><span data-stu-id="84b39-138">After you initialize the MSAL provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="84b39-139">html</span><span class="sxs-lookup"><span data-stu-id="84b39-139">html</span></span>](#tab/HTML)
<span data-ttu-id="84b39-140">Ниже приводится полный рабочий пример с использованием mgt-loader, поставщика MSAL, инициализированного в HTML, и компонента входа:</span><span class="sxs-lookup"><span data-stu-id="84b39-140">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="84b39-141">Это пример использования модулей ES6, поставщика MSAL, инициализированного в HTML, и компонента входа:</span><span class="sxs-lookup"><span data-stu-id="84b39-141">This is an example using the ES6 modules, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[<span data-ttu-id="84b39-142">js</span><span class="sxs-lookup"><span data-stu-id="84b39-142">js</span></span>](#tab/JavaScript)
<span data-ttu-id="84b39-143">Это пример использования модулей ES6, поставщика MSAL, инициализированного в JavaScript, и компонента входа:</span><span class="sxs-lookup"><span data-stu-id="84b39-143">This is an example using the ES6 modules, the MSAL Provider initialized in JavaScript, and the Login component:</span></span>

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})

function component() {
    const element = document.createElement('div');
    element.innerHTML = '<mgt-login></mgt-login>'
    return element;
}

document.body.appendChild((component()));
```

---


## <a name="test-your-app"></a><span data-ttu-id="84b39-144">Тестирование приложения</span><span class="sxs-lookup"><span data-stu-id="84b39-144">Test your app</span></span>

<span data-ttu-id="84b39-145">Чтобы протестировать приложение, MSAL требует, чтобы страница была на веб-сервере для перенаправления проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="84b39-145">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="84b39-146">Если вы только начинаете работу и хотите играть, вы можете использовать [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code или любой другой облегченный сервер разработки.</span><span class="sxs-lookup"><span data-stu-id="84b39-146">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="84b39-147">Скачайте расширение и откройте HTML-файл с помощью сервера live.</span><span class="sxs-lookup"><span data-stu-id="84b39-147">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="84b39-148">**Примечание.** Убедитесь, что **URI** перенаправления в регистрации приложения установлен на порт localhost, на который находится приложение.</span><span class="sxs-lookup"><span data-stu-id="84b39-148">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="84b39-149">Перейдите к регистрации приложения на  [портале Azure,](https://portal.azure.com)выберите "Проверка подлинности под управлением" и добавьте правильный **URI перенаправления.**</span><span class="sxs-lookup"><span data-stu-id="84b39-149">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="84b39-150">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="84b39-150">Next Steps</span></span>
- <span data-ttu-id="84b39-151">Ознакомьтесь с этим пошаговом руководстве по [построению простого веб-приложения.](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/)</span><span class="sxs-lookup"><span data-stu-id="84b39-151">Check out this step-by-step tutorial on [building a simple web app](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).</span></span>
- <span data-ttu-id="84b39-152">Попробуйте компоненты в игровой [области.](https://mgt.dev)</span><span class="sxs-lookup"><span data-stu-id="84b39-152">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="84b39-153">Задайте вопрос на [сайте Stack Overflow.](https://aka.ms/mgt-question)</span><span class="sxs-lookup"><span data-stu-id="84b39-153">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="84b39-154">Сообщать об ошибках или оставлять запросы на функции на [GitHub.](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="84b39-154">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>