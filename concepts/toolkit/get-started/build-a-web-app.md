---
title: Создание веб-приложения с помощью набора средств Microsoft Graph
description: Приступая к созданию веб-приложения с помощью набора средств Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 6852351e39aa3754ba7458bfe6fe5cd45f5cf635
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288533"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="8a27b-103">Создание веб-приложения с помощью набора средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a27b-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8a27b-104">В этом разделе описывается, как приступить к работе с набором инструментов Microsoft Graph в веб-приложении, написанном на Ванилла JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8a27b-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="8a27b-105">Если вы хотите узнать, как использовать набор средств с Web Framework, ознакомьтесь со статьей [Использование набора инструментов с Подкликом](./use-toolkit-with-react.md) или [Использование набора инструментов с угловой](./use-toolkit-with-angular.md)страницей.</span><span class="sxs-lookup"><span data-stu-id="8a27b-105">If you would like to learn how to use the Toolkit with a web framework, see [Use the Toolkit with React](./use-toolkit-with-react.md) or [Use the Toolkit with Angular](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="8a27b-106">Начало работы с набором средств Microsoft Graph состоит из следующих этапов:</span><span class="sxs-lookup"><span data-stu-id="8a27b-106">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="8a27b-107">Добавление набора инструментов Microsoft Graph в проект.</span><span class="sxs-lookup"><span data-stu-id="8a27b-107">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="8a27b-108">Инициализация поставщика MSAL.</span><span class="sxs-lookup"><span data-stu-id="8a27b-108">Initialize the MSAL Provider.</span></span>
3. <span data-ttu-id="8a27b-109">Добавление компонентов.</span><span class="sxs-lookup"><span data-stu-id="8a27b-109">Add components.</span></span>
4. <span data-ttu-id="8a27b-110">Протестируйте приложение.</span><span class="sxs-lookup"><span data-stu-id="8a27b-110">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="8a27b-111">Добавление набора инструментов Microsoft Graph в проект</span><span class="sxs-lookup"><span data-stu-id="8a27b-111">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="8a27b-112">Вы можете использовать набор средств Microsoft Graph в приложении, обратившись непосредственно к загрузчику (через унпкг) или установив пакет NPM.</span><span class="sxs-lookup"><span data-stu-id="8a27b-112">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="8a27b-113">Использование с помощью упр. загрузчиком</span><span class="sxs-lookup"><span data-stu-id="8a27b-113">Use via mgt-loader</span></span>
<span data-ttu-id="8a27b-114">Чтобы использовать набор средств с помощью элемента управления "центр управления", добавьте ссылку в скрипт в код:</span><span class="sxs-lookup"><span data-stu-id="8a27b-114">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="8a27b-115">Использование через NPM (модули ES6)</span><span class="sxs-lookup"><span data-stu-id="8a27b-115">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="8a27b-116">Использование набора средств с помощью модулей ES6 даст вам полный контроль над процессом создания пучка и позволяет объединить только код, который требуется для приложения.</span><span class="sxs-lookup"><span data-stu-id="8a27b-116">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="8a27b-117">Чтобы использовать модули ES6, добавьте в проект пакет NPM:</span><span class="sxs-lookup"><span data-stu-id="8a27b-117">To use the ES6 modules, add the npm package to your project:</span></span>

```bash
npm install @microsoft/mgt
```
> <span data-ttu-id="8a27b-118">**Note**: Если вы используете браузер, например IE11, который не поддерживает встроенные веб-компоненты, вам может потребоваться включить знаки, которые можно [включить](./overview.md#polyfills)в набор.</span><span class="sxs-lookup"><span data-stu-id="8a27b-118">**Note**: If you're targeting a browser such as IE11 that does not support web components natively, you might need to [include polyfills](./overview.md#polyfills).</span></span>

<span data-ttu-id="8a27b-119">Теперь вы можете ссылаться на все компоненты набора инструментов в приложении с помощью следующих компонентов:</span><span class="sxs-lookup"><span data-stu-id="8a27b-119">Now, you can reference the all the Toolkit components in your application with:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```
<span data-ttu-id="8a27b-120">Кроме того, следует ссылаться только на необходимые компоненты и не загружать все остальные.</span><span class="sxs-lookup"><span data-stu-id="8a27b-120">Or, reference only the components you need and avoid loading everything else.</span></span> <span data-ttu-id="8a27b-121">Например, чтобы добавить поставщика MSAL:</span><span class="sxs-lookup"><span data-stu-id="8a27b-121">For example, to add the MSAL Provider:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>
```

## <a name="initialize-the-msal-provider"></a><span data-ttu-id="8a27b-122">Инициализация поставщика MSAL</span><span class="sxs-lookup"><span data-stu-id="8a27b-122">Initialize the MSAL Provider</span></span>
<span data-ttu-id="8a27b-123">Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="8a27b-123">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="8a27b-124">Чтобы узнать больше, ознакомьтесь со статьей [Использование поставщиков](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="8a27b-124">To learn more, see [Using the providers](../providers.md).</span></span> <span data-ttu-id="8a27b-125">[Поставщик MSAL](../providers/msal.md) использует MSAL.js для входа пользователей и получения маркеров.</span><span class="sxs-lookup"><span data-stu-id="8a27b-125">The [MSAL Provider](../providers/msal.md) uses MSAL.js to sign in users and acquire tokens.</span></span> <span data-ttu-id="8a27b-126">Вы можете инициализировать поставщик MSAL в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8a27b-126">You can initialize the MSAL provider in your HTML or JavaScript.</span></span>

<span data-ttu-id="8a27b-127">Если вы хотите использовать собственную серверную проверку подлинности, используйте [поставщика прокси-сервера](../providers/proxy.md) вместо поставщика MSAL.</span><span class="sxs-lookup"><span data-stu-id="8a27b-127">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL provider.</span></span>

<span data-ttu-id="8a27b-128">Для инициализации поставщика можно использовать HTML-код или код JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8a27b-128">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="8a27b-129">Инициализация на HTML-странице</span><span class="sxs-lookup"><span data-stu-id="8a27b-129">Initialize in your HTML page</span></span>
<span data-ttu-id="8a27b-130">Добавьте `mgt-msal-provider` компонент на HTML-страницу и задайте для него значение `client-id` Client ID.</span><span class="sxs-lookup"><span data-stu-id="8a27b-130">Add the `mgt-msal-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
### <a name="initialize-in-javascript"></a><span data-ttu-id="8a27b-131">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a27b-131">Initialize in JavaScript</span></span>
<span data-ttu-id="8a27b-132">Чтобы инициализировать поставщик MSAL в коде JavaScript, добавьте в приложение следующий код:</span><span class="sxs-lookup"><span data-stu-id="8a27b-132">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```
<span data-ttu-id="8a27b-133">Единственным свойством, необходимым для инициализации поставщика, является идентификатор клиента, но вы можете задать дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="8a27b-133">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="8a27b-134">Полный список можно найти в разделе [поставщик Msal](../providers/msal.md).</span><span class="sxs-lookup"><span data-stu-id="8a27b-134">For the full list, see [Msal Provider](../providers/msal.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="8a27b-135">Создание идентификатора приложения или клиента</span><span class="sxs-lookup"><span data-stu-id="8a27b-135">Creating an app/client ID</span></span>
<span data-ttu-id="8a27b-136">Чтобы получить идентификатор клиента, необходимо [зарегистрировать приложение](../../auth-register-app-v2.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a27b-136">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> 
><span data-ttu-id="8a27b-137">**Note**: MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="8a27b-137">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="8a27b-138">Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен).</span><span class="sxs-lookup"><span data-stu-id="8a27b-138">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="8a27b-139">В разделе **Проверка подлинности**найдите раздел **неявный предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**.</span><span class="sxs-lookup"><span data-stu-id="8a27b-139">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="add-components"></a><span data-ttu-id="8a27b-140">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="8a27b-140">Add components</span></span>
<span data-ttu-id="8a27b-141">После инициализации поставщика MSAL можно приступить к использованию любого из компонентов набора средств.</span><span class="sxs-lookup"><span data-stu-id="8a27b-141">After you initialize the MSAL provider, you can start using any of the Toolkit components.</span></span>

<span data-ttu-id="8a27b-142">Ниже приведен полный рабочий пример с помощью элемента упр-Loader, поставщика MSAL, инициализированного в HTML, и компонента входа:</span><span class="sxs-lookup"><span data-stu-id="8a27b-142">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="8a27b-143">В этом примере используются модули ES6, поставщик MSAL, инициализированный в HTML, и компонент входа:</span><span class="sxs-lookup"><span data-stu-id="8a27b-143">This is an example using the ES6 modules, the MSAL Provider initialized in HTML, and the Login component:</span></span>
```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="8a27b-144">В этом примере используются модули ES6, поставщик MSAL, инициализированный в JavaScript, и компонент входа:</span><span class="sxs-lookup"><span data-stu-id="8a27b-144">This is an example using the ES6 modules, the MSAL Provider initialized in JavaScript, and the Login component:</span></span>

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

## <a name="test-your-app"></a><span data-ttu-id="8a27b-145">Тестирование приложения</span><span class="sxs-lookup"><span data-stu-id="8a27b-145">Test your app</span></span>

<span data-ttu-id="8a27b-146">Чтобы протестировать приложение, для MSAL требуется, чтобы страница была размещена на веб-сервере для перенаправления проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8a27b-146">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="8a27b-147">Если вы только начинаете работать и хотите поиграть, вы можете использовать [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code или на любом аналогичном сервере облегченного развертывания.</span><span class="sxs-lookup"><span data-stu-id="8a27b-147">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="8a27b-148">Скачайте расширение и откройте HTML-файл с помощью Live Server.</span><span class="sxs-lookup"><span data-stu-id="8a27b-148">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="8a27b-149">**Примечание:** Убедитесь, что **URI перенаправления** в регистрации приложения настроен на порт localhost, на котором размещено приложение.</span><span class="sxs-lookup"><span data-stu-id="8a27b-149">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="8a27b-150">Перейдите к регистрации приложения на [портале Azure](https://portal.azure.com), щелкните **Проверка подлинности** в разделе Управление и добавьте правильный **URI перенаправления**.</span><span class="sxs-lookup"><span data-stu-id="8a27b-150">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8a27b-151">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="8a27b-151">Next Steps</span></span>
- <span data-ttu-id="8a27b-152">Ознакомьтесь с пошаговыми руководствами по [созданию простого веб-приложения](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).</span><span class="sxs-lookup"><span data-stu-id="8a27b-152">Check out this step-by-step tutorial on [building a simple web app](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).</span></span>
- <span data-ttu-id="8a27b-153">Опробуйте компоненты в [интерактивная среда](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="8a27b-153">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="8a27b-154">Задайте вопрос о [переполнении стека](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="8a27b-154">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="8a27b-155">Сообщать об ошибках или оставлять запрос на функцию в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="8a27b-155">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>