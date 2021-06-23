---
title: Создание веб-приложения с помощью Microsoft Graph Toolkit
description: Знакомство с разработкой веб-приложений с помощью Microsoft Graph Toolkit
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: a4716b97eb3bbb9e64160d1bda3e44f32705403f
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082148"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="d4227-103">Создание веб-приложения с помощью Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="d4227-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d4227-104">В этом разделе описывается, как начать работу с Microsoft Graph Toolkit в веб-приложении, написанном на простом JavaScript.</span><span class="sxs-lookup"><span data-stu-id="d4227-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="d4227-105">В пошаговом руководстве попробуйте начать работу с модулем [Microsoft Graph набор средств.](/learn/modules/msgraph-toolkit-intro/)</span><span class="sxs-lookup"><span data-stu-id="d4227-105">For a step-by-step tutorial, try the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> <span data-ttu-id="d4227-106">Чтобы узнать, как использовать Toolkit в веб-среде, см. статью [Создание веб-приложения (React)](./use-toolkit-with-react.md) или [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md).</span><span class="sxs-lookup"><span data-stu-id="d4227-106">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="d4227-107">Начало работы с Microsoft Graph Toolkit включает:</span><span class="sxs-lookup"><span data-stu-id="d4227-107">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="d4227-108">Добавление Microsoft Graph Toolkit в проект.</span><span class="sxs-lookup"><span data-stu-id="d4227-108">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="d4227-109">Инициализация поставщика MSAL 2.0.</span><span class="sxs-lookup"><span data-stu-id="d4227-109">Initialize the MSAL 2.0 Provider.</span></span>
3. <span data-ttu-id="d4227-110">Добавление компонентов.</span><span class="sxs-lookup"><span data-stu-id="d4227-110">Add components.</span></span>
4. <span data-ttu-id="d4227-111">Тестирование приложения.</span><span class="sxs-lookup"><span data-stu-id="d4227-111">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="d4227-112">Добавление Microsoft Graph Toolkit в проект</span><span class="sxs-lookup"><span data-stu-id="d4227-112">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="d4227-113">Используйте Microsoft Graph Toolkit в приложении, обратившись непосредственно к загрузчику (через unpkg) или установив пакет npm.</span><span class="sxs-lookup"><span data-stu-id="d4227-113">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="d4227-114">unpkg</span><span class="sxs-lookup"><span data-stu-id="d4227-114">unpkg</span></span>](#tab/html)
<span data-ttu-id="d4227-115">Чтобы использовать Toolkit в загрузчике Microsoft Graph Toolkit, добавьте ссылку в сценарий кода:</span><span class="sxs-lookup"><span data-stu-id="d4227-115">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="d4227-116">npm</span><span class="sxs-lookup"><span data-stu-id="d4227-116">npm</span></span>](#tab/npm)
<span data-ttu-id="d4227-117">Использование Toolkit с помощью модулей ES6 обеспечивает полное управление процессом объединения и позволяет объединить только код, необходимый для приложения.</span><span class="sxs-lookup"><span data-stu-id="d4227-117">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="d4227-118">Чтобы использовать модули ES6, добавьте в проект пакет npm:</span><span class="sxs-lookup"><span data-stu-id="d4227-118">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---

## <a name="initialize-the-msal-20-provider"></a><span data-ttu-id="d4227-119">Инициализация поставщика MSAL 2.0</span><span class="sxs-lookup"><span data-stu-id="d4227-119">Initialize the MSAL 2.0 Provider</span></span>
<span data-ttu-id="d4227-120">Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="d4227-120">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="d4227-121">Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="d4227-121">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="d4227-122">Поставщик [MSAL 2.0](../providers/msal2.md) использует msal-browser для регистрации пользователей и приобретения маркеров.</span><span class="sxs-lookup"><span data-stu-id="d4227-122">The [MSAL 2.0 Provider](../providers/msal2.md) uses msal-browser to sign in users and acquire tokens.</span></span> <span data-ttu-id="d4227-123">Этот поставщик можно инициализировать в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="d4227-123">You can initialize this provider in your HTML or JavaScript.</span></span>

> <span data-ttu-id="d4227-124">**Примечание.** Если вы в настоящее время используете поставщика MSAL и хотите обновить до поставщика MSAL 2.0, выполните указанные [здесь действия.](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)</span><span class="sxs-lookup"><span data-stu-id="d4227-124">**Note**: If you are currently using MSAL Provider and would like to update to MSAL 2.0 Provider, follow the steps listed [here](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider).</span></span>
<span data-ttu-id="d4227-125">Если вы хотите использовать собственную проверку подлинности, используйте поставщика прокси-серверов на месте поставщика MSAL 2.0. [](../providers/proxy.md)</span><span class="sxs-lookup"><span data-stu-id="d4227-125">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL 2.0 provider.</span></span>

<span data-ttu-id="d4227-126">Чтобы инициализировать поставщика, можно использовать HTML-код или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="d4227-126">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="d4227-127">HTML</span><span class="sxs-lookup"><span data-stu-id="d4227-127">HTML</span></span>](#tab/HTML)
<span data-ttu-id="d4227-128">Добавьте компонент `mgt-msal2-provider` на HTML-страницу и задайте `client-id` для идентификатора клиента приложения.</span><span class="sxs-lookup"><span data-stu-id="d4227-128">Add the `mgt-msal2-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
```
# <a name="javascript"></a>[<span data-ttu-id="d4227-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4227-129">JavaScript</span></span>](#tab/JavaScript)
<span data-ttu-id="d4227-130">Чтобы инициализировать поставщика MSAL в JavaScript, добавьте следующий код в приложение:</span><span class="sxs-lookup"><span data-stu-id="d4227-130">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```javascript
import { Providers, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});
```

---

<span data-ttu-id="d4227-131">Идентификатор клиента — это единственное свойство, которое требуется для инициализации поставщика, но вы можете настроить дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="d4227-131">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="d4227-132">Полный список см. в [списке Msal 2.0 Provider](../providers/msal2.md).</span><span class="sxs-lookup"><span data-stu-id="d4227-132">For the full list, see [Msal 2.0 Provider](../providers/msal2.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="d4227-133">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="d4227-133">Creating an app/client ID</span></span>
<span data-ttu-id="d4227-134">Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](./add-aad-app-registration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d4227-134">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span>

## <a name="add-components"></a><span data-ttu-id="d4227-135">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="d4227-135">Add components</span></span>
<span data-ttu-id="d4227-136">После инициализации поставщика MSAL 2.0 можно начать использовать любой из набор средств компонентов.</span><span class="sxs-lookup"><span data-stu-id="d4227-136">After you initialize the MSAL 2.0 provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="d4227-137">HTML</span><span class="sxs-lookup"><span data-stu-id="d4227-137">HTML</span></span>](#tab/HTML)
<span data-ttu-id="d4227-138">Ниже приведен рабочий пример с использованием загрузчика Microsoft Graph Toolkit, поставщика MSAL, инициализированного в HTML, и компонента входа в систему:</span><span class="sxs-lookup"><span data-stu-id="d4227-138">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="d4227-139">Это пример с использованием модулей ES6, поставщика MSAL 2.0, инициализированного в HTML-коде, и компонента Login:</span><span class="sxs-lookup"><span data-stu-id="d4227-139">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

# <a name="javascript"></a>[<span data-ttu-id="d4227-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4227-140">JavaScript</span></span>](#tab/JavaScript)
<span data-ttu-id="d4227-141">Это пример с помощью модулей ES6, поставщика MSAL 2.0, инициализированного в JavaScript, и компонента Login:</span><span class="sxs-lookup"><span data-stu-id="d4227-141">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in JavaScript, and the Login component:</span></span>

```javascript
import { Providers, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});

function component() {
  const element = document.createElement('div');
  element.innerHTML = '<mgt-login></mgt-login>';
  return element;
}

document.body.appendChild(component());
```

---

## <a name="test-your-app"></a><span data-ttu-id="d4227-142">Тестирование приложения</span><span class="sxs-lookup"><span data-stu-id="d4227-142">Test your app</span></span>

<span data-ttu-id="d4227-143">Чтобы протестировать приложение, MSAL требует, чтобы страница была размещена на веб-сервере для перенаправления проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d4227-143">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="d4227-144">Если вы только начинаете работать и хотите поэкспериментировать с, можно использовать [Динамический сервер](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code или на любом похожем сервере облегченной разработки.</span><span class="sxs-lookup"><span data-stu-id="d4227-144">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="d4227-145">Скачайте расширение и откройте HTML-файл с помощью динамического сервера.</span><span class="sxs-lookup"><span data-stu-id="d4227-145">Download the extension and open your HTML file using live server.</span></span>
> <span data-ttu-id="d4227-146">**Примечание.** Убедитесь в том, что **URI перенаправления** в приложении регистрации настроен на порт localhost, на котором размещено приложение.</span><span class="sxs-lookup"><span data-stu-id="d4227-146">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="d4227-147">Перейдите в службу регистрации приложения на [портале Azure](https://portal.azure.com), в разделе управления выберите пункт **Проверка подлинности**, и укажите соответствующий **URI перенаправления**.</span><span class="sxs-lookup"><span data-stu-id="d4227-147">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="track-a-users-sign-in-state"></a><span data-ttu-id="d4227-148">Отслеживание знака пользователя в состоянии</span><span class="sxs-lookup"><span data-stu-id="d4227-148">Track a user's sign in state</span></span>

<span data-ttu-id="d4227-149">Вы можете определить, когда пользователь успешно вписался и соответствующим образом отображает определенные компоненты.</span><span class="sxs-lookup"><span data-stu-id="d4227-149">You can detect when a user has successfully signed in and display specific components accordingly.</span></span> <span data-ttu-id="d4227-150">Например, отобразить компонент повестки дня, если пользователь в него вписалась.</span><span class="sxs-lookup"><span data-stu-id="d4227-150">For example, display the agenda component if the user has signed in.</span></span> <span data-ttu-id="d4227-151">В противном случае отобразить знак в интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="d4227-151">Otherwise, display the sign in interface.</span></span>

<span data-ttu-id="d4227-152">Чтобы правильно проверить вход пользователя в состояние, добавьте обработник событий `providerUpdated` в событие с помощью `Providers.onProviderUpdated` функции.</span><span class="sxs-lookup"><span data-stu-id="d4227-152">To properly inspect the user's sign in state, add an event handler to the `providerUpdated` event using the `Providers.onProviderUpdated` function.</span></span> <span data-ttu-id="d4227-153">В обработнике проверьте состояние поставщика, хранимое в `Providers.globalProvider.state` свойстве.</span><span class="sxs-lookup"><span data-stu-id="d4227-153">In the handler, check the provider state stored on the `Providers.globalProvider.state` property.</span></span>

# <a name="html"></a>[<span data-ttu-id="d4227-154">HTML</span><span class="sxs-lookup"><span data-stu-id="d4227-154">HTML</span></span>](#tab/HTML)

<span data-ttu-id="d4227-155">Если вы используете библиотеку, вы можете получить доступ к глобальному свойству и `mgt-loader` `Provider` из `ProviderState` `mgt` него.</span><span class="sxs-lookup"><span data-stu-id="d4227-155">If you're using the `mgt-loader` library, you can access the `Provider` and `ProviderState` from the global `mgt` property.</span></span>

```html
<!DOCTYPE html>
<html>
<head>
  <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
</head>
<body>
  <mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
  <div id="main">
    <mgt-login></mgt-login>
  </div>
  <script>
    const loadAgenda = () => {
      if (mgt.Providers.globalProvider.state === mgt.ProviderState.SignedIn) {
        document.getElementById('main').innerHTML = '<mgt-agenda></mgt-agenda>';
      }
    }
    mgt.Providers.onProviderUpdated(loadAgenda);
  </script>
</body>
</html>
```

# <a name="javascript"></a>[<span data-ttu-id="d4227-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4227-156">JavaScript</span></span>](#tab/JavaScript)

<span data-ttu-id="d4227-157">Если вы используете набор инструментов с помощью пакетов npm, вы можете импортировать и `Provider` `ProviderState` из `@microsoft/mgt` .</span><span class="sxs-lookup"><span data-stu-id="d4227-157">If you're using the toolkit via the npm packages, you can import the `Provider` and `ProviderState` from `@microsoft/mgt`.</span></span>

```javascript
import { Providers, ProviderState, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});

const loadAgenda = () => {
  if (Providers.globalProvider.state === ProviderState.SignedIn) {
    document.getElementById('main').innerHTML = '<mgt-agenda></mgt-agenda>';
  }
};

Providers.onProviderUpdated(loadAgenda);
```

---

## <a name="next-steps"></a><span data-ttu-id="d4227-158">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="d4227-158">Next Steps</span></span>

- <span data-ttu-id="d4227-159">Ознакомьтесь с [пошаговой](/learn/modules/msgraph-toolkit-intro/) инструкцией по началу Graph набор средств Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d4227-159">Check out the [Get started with Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) step-by-step tutorial.</span></span>
- <span data-ttu-id="d4227-160">Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="d4227-160">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="d4227-161">Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="d4227-161">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="d4227-162">Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="d4227-162">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
