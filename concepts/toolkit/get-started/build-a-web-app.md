---
title: Создание веб-приложения с помощью Microsoft Graph Toolkit
description: Знакомство с разработкой веб-приложений с помощью Microsoft Graph Toolkit
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 73e61e9d2c1c453ec67e61dce1f088b5119d1e8d
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664018"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="922fe-103">Создание веб-приложения с помощью Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="922fe-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="922fe-104">В этом разделе описывается, как начать работу с Microsoft Graph Toolkit в веб-приложении, написанном на простом JavaScript.</span><span class="sxs-lookup"><span data-stu-id="922fe-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="922fe-105">Чтобы узнать, как использовать Toolkit в веб-среде, см. статью [Создание веб-приложения (React)](./use-toolkit-with-react.md) или [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md).</span><span class="sxs-lookup"><span data-stu-id="922fe-105">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="922fe-106">Начало работы с Microsoft Graph Toolkit включает:</span><span class="sxs-lookup"><span data-stu-id="922fe-106">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="922fe-107">Добавление Microsoft Graph Toolkit в проект.</span><span class="sxs-lookup"><span data-stu-id="922fe-107">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="922fe-108">Инициализация поставщика MSAL.</span><span class="sxs-lookup"><span data-stu-id="922fe-108">Initialize the MSAL Provider.</span></span>
3. <span data-ttu-id="922fe-109">Добавление компонентов.</span><span class="sxs-lookup"><span data-stu-id="922fe-109">Add components.</span></span>
4. <span data-ttu-id="922fe-110">Тестирование приложения.</span><span class="sxs-lookup"><span data-stu-id="922fe-110">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="922fe-111">Добавление Microsoft Graph Toolkit в проект</span><span class="sxs-lookup"><span data-stu-id="922fe-111">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="922fe-112">Используйте Microsoft Graph Toolkit в приложении, обратившись непосредственно к загрузчику (через unpkg) или установив пакет npm.</span><span class="sxs-lookup"><span data-stu-id="922fe-112">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="922fe-113">unpkg</span><span class="sxs-lookup"><span data-stu-id="922fe-113">unpkg</span></span>](#tab/html)
<span data-ttu-id="922fe-114">Чтобы использовать Toolkit в загрузчике Microsoft Graph Toolkit, добавьте ссылку в сценарий кода:</span><span class="sxs-lookup"><span data-stu-id="922fe-114">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="922fe-115">npm</span><span class="sxs-lookup"><span data-stu-id="922fe-115">npm</span></span>](#tab/npm)
<span data-ttu-id="922fe-116">Использование Toolkit с помощью модулей ES6 обеспечивает полное управление процессом объединения и позволяет объединить только код, необходимый для приложения.</span><span class="sxs-lookup"><span data-stu-id="922fe-116">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="922fe-117">Чтобы использовать модули ES6, добавьте в проект пакет npm:</span><span class="sxs-lookup"><span data-stu-id="922fe-117">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---


> <span data-ttu-id="922fe-118">**Примечание**. Если вы ориентируетесь на браузер, например IE11, который изначально не поддерживает веб-компоненты, потребуется [включить полизаполнение](./overview.md#polyfills).</span><span class="sxs-lookup"><span data-stu-id="922fe-118">**Note**: If you're targeting a browser such as IE11 that does not support web components natively, you might need to [include polyfills](./overview.md#polyfills).</span></span>

## <a name="initialize-the-msal-provider"></a><span data-ttu-id="922fe-119">Инициализация поставщика MSAL</span><span class="sxs-lookup"><span data-stu-id="922fe-119">Initialize the MSAL Provider</span></span>
<span data-ttu-id="922fe-120">Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="922fe-120">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="922fe-121">Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="922fe-121">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="922fe-122">[Поставщик MSAL](../providers/msal.md) использует MSAL.js для входа в систему и получения маркеров.</span><span class="sxs-lookup"><span data-stu-id="922fe-122">The [MSAL Provider](../providers/msal.md) uses MSAL.js to sign in users and acquire tokens.</span></span> <span data-ttu-id="922fe-123">Поставщика MSAL можно инициализировать в HTML-коде или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="922fe-123">You can initialize the MSAL provider in your HTML or JavaScript.</span></span>

<span data-ttu-id="922fe-124">Чтобы использовать собственную внутреннюю проверку подлинности, используйте [Поставщик прокси-сервера](../providers/proxy.md) вместо поставщика MSAL.</span><span class="sxs-lookup"><span data-stu-id="922fe-124">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL provider.</span></span>

<span data-ttu-id="922fe-125">Чтобы инициализировать поставщика, можно использовать HTML-код или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="922fe-125">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="922fe-126">html</span><span class="sxs-lookup"><span data-stu-id="922fe-126">html</span></span>](#tab/HTML)
<span data-ttu-id="922fe-127">Добавьте компонент `mgt-msal-provider` на HTML-страницу и задайте `client-id` для идентификатора клиента приложения.</span><span class="sxs-lookup"><span data-stu-id="922fe-127">Add the `mgt-msal-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
# <a name="js"></a>[<span data-ttu-id="922fe-128">js</span><span class="sxs-lookup"><span data-stu-id="922fe-128">js</span></span>](#tab/JavaScript)
<span data-ttu-id="922fe-129">Чтобы инициализировать поставщика MSAL в JavaScript, добавьте следующий код в приложение:</span><span class="sxs-lookup"><span data-stu-id="922fe-129">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


<span data-ttu-id="922fe-130">Идентификатор клиента — это единственное свойство, которое требуется для инициализации поставщика, но вы можете настроить дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="922fe-130">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="922fe-131">Полный список см. в статье [Поставщик Msal](../providers/msal.md).</span><span class="sxs-lookup"><span data-stu-id="922fe-131">For the full list, see [Msal Provider](../providers/msal.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="922fe-132">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="922fe-132">Creating an app/client ID</span></span>
<span data-ttu-id="922fe-133">Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](./add-aad-app-registration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="922fe-133">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span> 
><span data-ttu-id="922fe-134">**Примечание**. MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="922fe-134">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="922fe-135">Включите неявный поток в своем приложении на портале Azure (он не включен по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="922fe-135">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="922fe-136">В области **Проверка подлинности** найдите раздел **Неявное предоставление** и установите флажки **Маркеры доступа** и **Маркеры идентификаторов**.</span><span class="sxs-lookup"><span data-stu-id="922fe-136">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="add-components"></a><span data-ttu-id="922fe-137">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="922fe-137">Add components</span></span>
<span data-ttu-id="922fe-138">После инициализации поставщика MSAL можно приступить к работе с любыми компонентами Toolkit.</span><span class="sxs-lookup"><span data-stu-id="922fe-138">After you initialize the MSAL provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="922fe-139">html</span><span class="sxs-lookup"><span data-stu-id="922fe-139">html</span></span>](#tab/HTML)
<span data-ttu-id="922fe-140">Ниже приведен рабочий пример с использованием загрузчика Microsoft Graph Toolkit, поставщика MSAL, инициализированного в HTML, и компонента входа в систему:</span><span class="sxs-lookup"><span data-stu-id="922fe-140">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="922fe-141">Пример использования модулей ES6, поставщика MSAL, инициализированного в HTML, и компонента входа в систему:</span><span class="sxs-lookup"><span data-stu-id="922fe-141">This is an example using the ES6 modules, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[<span data-ttu-id="922fe-142">js</span><span class="sxs-lookup"><span data-stu-id="922fe-142">js</span></span>](#tab/JavaScript)
<span data-ttu-id="922fe-143">Пример использования модулей ES6, поставщика MSAL, инициализированного в JavaScript, и компонента входа в систему:</span><span class="sxs-lookup"><span data-stu-id="922fe-143">This is an example using the ES6 modules, the MSAL Provider initialized in JavaScript, and the Login component:</span></span>

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


## <a name="test-your-app"></a><span data-ttu-id="922fe-144">Тестирование приложения</span><span class="sxs-lookup"><span data-stu-id="922fe-144">Test your app</span></span>

<span data-ttu-id="922fe-145">Чтобы протестировать приложение, MSAL требует, чтобы страница была размещена на веб-сервере для перенаправления проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="922fe-145">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="922fe-146">Если вы только начинаете работать и хотите поэкспериментировать с, можно использовать [Динамический сервер](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code или на любом похожем сервере облегченной разработки.</span><span class="sxs-lookup"><span data-stu-id="922fe-146">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="922fe-147">Скачайте расширение и откройте HTML-файл с помощью динамического сервера.</span><span class="sxs-lookup"><span data-stu-id="922fe-147">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="922fe-148">**Примечание.** Убедитесь в том, что **URI перенаправления** в приложении регистрации настроен на порт localhost, на котором размещено приложение.</span><span class="sxs-lookup"><span data-stu-id="922fe-148">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="922fe-149">Перейдите в службу регистрации приложения на [портале Azure](https://portal.azure.com), в разделе управления выберите пункт **Проверка подлинности**, и укажите соответствующий **URI перенаправления**.</span><span class="sxs-lookup"><span data-stu-id="922fe-149">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="922fe-150">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="922fe-150">Next Steps</span></span>
- <span data-ttu-id="922fe-151">Ознакомьтесь с пошаговыми инструкциями для [создания простого веб-приложения](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).</span><span class="sxs-lookup"><span data-stu-id="922fe-151">Check out this step-by-step tutorial on [building a simple web app](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).</span></span>
- <span data-ttu-id="922fe-152">Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="922fe-152">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="922fe-153">Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="922fe-153">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="922fe-154">Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="922fe-154">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>