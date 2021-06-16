---
title: Создание веб-приложения с помощью Microsoft Graph Toolkit
description: Знакомство с разработкой веб-приложений с помощью Microsoft Graph Toolkit
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 989e79c2b52f7e02fb61604d3011f13aced580ed
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941538"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="ab6b4-103">Создание веб-приложения с помощью Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="ab6b4-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ab6b4-104">В этом разделе описывается, как начать работу с Microsoft Graph Toolkit в веб-приложении, написанном на простом JavaScript.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="ab6b4-105">В пошаговом руководстве попробуйте начать работу с модулем [Microsoft Graph набор средств.](/learn/modules/msgraph-toolkit-intro/)</span><span class="sxs-lookup"><span data-stu-id="ab6b4-105">For a step-by-step tutorial, try the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> <span data-ttu-id="ab6b4-106">Чтобы узнать, как использовать Toolkit в веб-среде, см. статью [Создание веб-приложения (React)](./use-toolkit-with-react.md) или [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md).</span><span class="sxs-lookup"><span data-stu-id="ab6b4-106">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="ab6b4-107">Начало работы с Microsoft Graph Toolkit включает:</span><span class="sxs-lookup"><span data-stu-id="ab6b4-107">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="ab6b4-108">Добавление Microsoft Graph Toolkit в проект.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-108">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="ab6b4-109">Инициализация поставщика MSAL 2.0.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-109">Initialize the MSAL 2.0 Provider.</span></span>
3. <span data-ttu-id="ab6b4-110">Добавление компонентов.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-110">Add components.</span></span>
4. <span data-ttu-id="ab6b4-111">Тестирование приложения.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-111">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="ab6b4-112">Добавление Microsoft Graph Toolkit в проект</span><span class="sxs-lookup"><span data-stu-id="ab6b4-112">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="ab6b4-113">Используйте Microsoft Graph Toolkit в приложении, обратившись непосредственно к загрузчику (через unpkg) или установив пакет npm.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-113">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="ab6b4-114">unpkg</span><span class="sxs-lookup"><span data-stu-id="ab6b4-114">unpkg</span></span>](#tab/html)
<span data-ttu-id="ab6b4-115">Чтобы использовать Toolkit в загрузчике Microsoft Graph Toolkit, добавьте ссылку в сценарий кода:</span><span class="sxs-lookup"><span data-stu-id="ab6b4-115">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="ab6b4-116">npm</span><span class="sxs-lookup"><span data-stu-id="ab6b4-116">npm</span></span>](#tab/npm)
<span data-ttu-id="ab6b4-117">Использование Toolkit с помощью модулей ES6 обеспечивает полное управление процессом объединения и позволяет объединить только код, необходимый для приложения.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-117">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="ab6b4-118">Чтобы использовать модули ES6, добавьте в проект пакет npm:</span><span class="sxs-lookup"><span data-stu-id="ab6b4-118">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---

## <a name="initialize-the-msal-20-provider"></a><span data-ttu-id="ab6b4-119">Инициализация поставщика MSAL 2.0</span><span class="sxs-lookup"><span data-stu-id="ab6b4-119">Initialize the MSAL 2.0 Provider</span></span>
<span data-ttu-id="ab6b4-120">Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-120">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="ab6b4-121">Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="ab6b4-121">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="ab6b4-122">Поставщик [MSAL 2.0](../providers/msal2.md) использует msal-browser для регистрации пользователей и приобретения маркеров.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-122">The [MSAL 2.0 Provider](../providers/msal2.md) uses msal-browser to sign in users and acquire tokens.</span></span> <span data-ttu-id="ab6b4-123">Этот поставщик можно инициализировать в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-123">You can initialize this provider in your HTML or JavaScript.</span></span>

> <span data-ttu-id="ab6b4-124">**Примечание.** Если вы в настоящее время используете поставщика MSAL и хотите обновить до поставщика MSAL 2.0, выполните указанные [здесь действия.](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)</span><span class="sxs-lookup"><span data-stu-id="ab6b4-124">**Note**: If you are currently using MSAL Provider and would like to update to MSAL 2.0 Provider, follow the steps listed [here](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider).</span></span>
<span data-ttu-id="ab6b4-125">Если вы хотите использовать собственную проверку подлинности, используйте поставщика прокси-серверов на месте поставщика MSAL 2.0. [](../providers/proxy.md)</span><span class="sxs-lookup"><span data-stu-id="ab6b4-125">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL 2.0 provider.</span></span>

<span data-ttu-id="ab6b4-126">Чтобы инициализировать поставщика, можно использовать HTML-код или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-126">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="ab6b4-127">HTML</span><span class="sxs-lookup"><span data-stu-id="ab6b4-127">HTML</span></span>](#tab/HTML)
<span data-ttu-id="ab6b4-128">Добавьте компонент `mgt-msal2-provider` на HTML-страницу и задайте `client-id` для идентификатора клиента приложения.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-128">Add the `mgt-msal2-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID"></mgt-msal2-provider>
```
# <a name="javascript"></a>[<span data-ttu-id="ab6b4-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab6b4-129">JavaScript</span></span>](#tab/JavaScript)
<span data-ttu-id="ab6b4-130">Чтобы инициализировать поставщика MSAL в JavaScript, добавьте следующий код в приложение:</span><span class="sxs-lookup"><span data-stu-id="ab6b4-130">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```javascript
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


<span data-ttu-id="ab6b4-131">Идентификатор клиента — это единственное свойство, которое требуется для инициализации поставщика, но вы можете настроить дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-131">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="ab6b4-132">Полный список см. в [списке Msal 2.0 Provider](../providers/msal2.md).</span><span class="sxs-lookup"><span data-stu-id="ab6b4-132">For the full list, see [Msal 2.0 Provider](../providers/msal2.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="ab6b4-133">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="ab6b4-133">Creating an app/client ID</span></span>
<span data-ttu-id="ab6b4-134">Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](./add-aad-app-registration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-134">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span> 

## <a name="add-components"></a><span data-ttu-id="ab6b4-135">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="ab6b4-135">Add components</span></span>
<span data-ttu-id="ab6b4-136">После инициализации поставщика MSAL 2.0 можно начать использовать любой из набор средств компонентов.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-136">After you initialize the MSAL 2.0 provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="ab6b4-137">HTML</span><span class="sxs-lookup"><span data-stu-id="ab6b4-137">HTML</span></span>](#tab/HTML)
<span data-ttu-id="ab6b4-138">Ниже приведен рабочий пример с использованием загрузчика Microsoft Graph Toolkit, поставщика MSAL, инициализированного в HTML, и компонента входа в систему:</span><span class="sxs-lookup"><span data-stu-id="ab6b4-138">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="ab6b4-139">Это пример с использованием модулей ES6, поставщика MSAL 2.0, инициализированного в HTML-коде, и компонента Login:</span><span class="sxs-lookup"><span data-stu-id="ab6b4-139">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>

<mgt-login></mgt-login>
```
# <a name="javascript"></a>[<span data-ttu-id="ab6b4-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab6b4-140">JavaScript</span></span>](#tab/JavaScript)
<span data-ttu-id="ab6b4-141">Это пример с помощью модулей ES6, поставщика MSAL 2.0, инициализированного в JavaScript, и компонента Login:</span><span class="sxs-lookup"><span data-stu-id="ab6b4-141">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in JavaScript, and the Login component:</span></span>

```javascript
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
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


## <a name="test-your-app"></a><span data-ttu-id="ab6b4-142">Тестирование приложения</span><span class="sxs-lookup"><span data-stu-id="ab6b4-142">Test your app</span></span>

<span data-ttu-id="ab6b4-143">Чтобы протестировать приложение, MSAL требует, чтобы страница была размещена на веб-сервере для перенаправления проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-143">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="ab6b4-144">Если вы только начинаете работать и хотите поэкспериментировать с, можно использовать [Динамический сервер](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code или на любом похожем сервере облегченной разработки.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-144">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="ab6b4-145">Скачайте расширение и откройте HTML-файл с помощью динамического сервера.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-145">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="ab6b4-146">**Примечание.** Убедитесь в том, что **URI перенаправления** в приложении регистрации настроен на порт localhost, на котором размещено приложение.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-146">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="ab6b4-147">Перейдите в службу регистрации приложения на [портале Azure](https://portal.azure.com), в разделе управления выберите пункт **Проверка подлинности**, и укажите соответствующий **URI перенаправления**.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-147">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="track-a-users-sign-in-state"></a><span data-ttu-id="ab6b4-148">Отслеживание знака пользователя в состоянии</span><span class="sxs-lookup"><span data-stu-id="ab6b4-148">Track a user's sign in state</span></span>

<span data-ttu-id="ab6b4-149">Вы можете определить, когда пользователь успешно вписался и соответствующим образом отображает определенные компоненты.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-149">You can detect when a user has successfully signed in and display specific components accordingly.</span></span> <span data-ttu-id="ab6b4-150">Например, отобразить компонент повестки дня, если пользователь в него вписалась.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-150">For example, display the agenda component if the user has signed in.</span></span> <span data-ttu-id="ab6b4-151">В противном случае отобразить знак в интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-151">Otherwise, display the sign in interface.</span></span>

<span data-ttu-id="ab6b4-152">Вы можете определить, подписан ли пользователь, оценив `globalProvider` и `providerState` .</span><span class="sxs-lookup"><span data-stu-id="ab6b4-152">You can determine if a user is signed in by evaluating the `globalProvider` and `providerState`.</span></span>

# <a name="html"></a>[<span data-ttu-id="ab6b4-153">HTML</span><span class="sxs-lookup"><span data-stu-id="ab6b4-153">HTML</span></span>](#tab/HTML)

<span data-ttu-id="ab6b4-154">Если вы используете библиотеку, вы можете получить доступ к свойству `mgt-loader` `provider` и из `providerState` `mgt` него.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-154">If you're using the `mgt-loader` library, you can access the `provider` and `providerState` from the `mgt` property.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<div id="main"><mgt-login></mgt-login></div>

<script>
    const provider = mgt.Providers.globalProvider;
    const isLoggedIn = provider && provider.state === mgt.ProviderState.SignedIn

    // Show the mgt-agenda component ONLY if the user is logged in, show the mgt-login component if not
    function loadAgenda(){
        if(isLoggedIn){
            const main = document.getElementById("main");
            main.innerHTML = `<mgt-agenda></mgt-agenda>`;
        } else {
            main.innerHTML = `<mgt-login></mgt-login>`;
        }
    }

    loadAgenda();
</script>
```

# <a name="javascript"></a>[<span data-ttu-id="ab6b4-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab6b4-155">JavaScript</span></span>](#tab/JavaScript)
<span data-ttu-id="ab6b4-156">Если вы используете набор средств пакеты npm, вы можете импортировать и `provider` `providerState` из `@microsoft/mgt` .</span><span class="sxs-lookup"><span data-stu-id="ab6b4-156">If you're using the Toolkit via the npm packages, you can import the `provider` and `providerState` from `@microsoft/mgt`.</span></span>

```javascript
import {Providers, ProviderState} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})

function isLoggedIn(){
    const provider = Providers.globalProvider;
    return provider && provider.state === ProviderState.SignedIn;
}

function loadAgenda(){
    const agenda = document.createElement("mgt-agenda");
    const loginComponent = document.createElement("mgt-login");
    if(isLoggedIn()){
        // the user is logged in, load their agenda
        document.body.innerHTML = `<mgt-agenda></mgt-agenda>`;
    } else {
        // the user is not logged in, show them the login component
        document.body.innerHTML = `<mgt-login></mgt-login>`
    }
}

loadAgenda();
```

---


## <a name="next-steps"></a><span data-ttu-id="ab6b4-157">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="ab6b4-157">Next Steps</span></span>
- <span data-ttu-id="ab6b4-158">Ознакомьтесь с [пошаговой](/learn/modules/msgraph-toolkit-intro/) инструкцией по началу Graph набор средств Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ab6b4-158">Check out the [Get started with Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) step-by-step tutorial.</span></span>
- <span data-ttu-id="ab6b4-159">Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="ab6b4-159">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="ab6b4-160">Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="ab6b4-160">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="ab6b4-161">Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="ab6b4-161">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
