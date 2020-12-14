---
title: Поставщики набор средств Microsoft Graph
description: Поставщики набор средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: a4cd1b58bb29e42ecb0283709e71a3ce3a7e86d7
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658261"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="a0e6e-103">Поставщики набор средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a0e6e-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="a0e6e-104">Поставщики набор средств Microsoft Graph позволяют приложению проверить подлинность с помощью microsoft Identity и получить доступ к Microsoft Graph всего за несколько строк кода.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-104">The Microsoft Graph Toolkit providers enable your application to authenticate with Microsoft Identity and access Microsoft Graph in only few lines of code.</span></span> <span data-ttu-id="a0e6e-105">Каждый поставщик обрабатывает проверку подлинности пользователей и получает маркеры доступа для вызова API Microsoft Graph, чтобы вам не нужно было писать этот код самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-105">Each provider handles user authentication and acquiring the access tokens to call Microsoft Graph APIs, so that you don't have to write this code yourself.</span></span> 

<span data-ttu-id="a0e6e-106">Вы можете использовать поставщики самостоятельно без компонентов, чтобы быстро реализовать проверку подлинности для вашего приложения и выполнить вызовы Microsoft Graph через клиентский SDK JavaScript.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-106">You can use the providers on their own, without components, to quickly implement authentication for your app and make calls to Microsoft Graph via the JavaScript client SDK.</span></span>

<span data-ttu-id="a0e6e-107">Поставщики необходимы при использовании microsoft Graph набор средств компонентов, которые используют их для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-107">The providers are required when using the Microsoft Graph Toolkit components as the components use them to access Microsoft Graph.</span></span> <span data-ttu-id="a0e6e-108">Если у вас уже есть собственная проверка подлинности и вы хотите использовать компоненты, можно использовать [настраиваемую службу.](./custom.md)</span><span class="sxs-lookup"><span data-stu-id="a0e6e-108">If you already have your own authentication and want to use the components, you can use a [custom provider](./custom.md) instead.</span></span>

<span data-ttu-id="a0e6e-109">В набор средств входят следующие поставщики.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-109">The Toolkit includes the following providers.</span></span>

|<span data-ttu-id="a0e6e-110">Поставщики</span><span class="sxs-lookup"><span data-stu-id="a0e6e-110">Providers</span></span>|<span data-ttu-id="a0e6e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a0e6e-111">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="a0e6e-112">Msal</span><span class="sxs-lookup"><span data-stu-id="a0e6e-112">Msal</span></span>](./msal.md)|<span data-ttu-id="a0e6e-113">Использует MSAL.js для входов пользователей и получения маркеров для использования с Microsoft Graph в веб-приложении.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-113">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph in a web application.</span></span>|
|[<span data-ttu-id="a0e6e-114">SharePoint</span><span class="sxs-lookup"><span data-stu-id="a0e6e-114">SharePoint</span></span>](./sharepoint.md)|<span data-ttu-id="a0e6e-115">Проверка подлинности и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-115">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="a0e6e-116">Teams</span><span class="sxs-lookup"><span data-stu-id="a0e6e-116">Teams</span></span>](./teams.md)|<span data-ttu-id="a0e6e-117">Проверка подлинности и предоставляет Microsoft Graph доступ к компонентам на вкладке Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-117">Authenticates and provides Microsoft Graph access to components inside  Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="a0e6e-118">Прокси-сервер</span><span class="sxs-lookup"><span data-stu-id="a0e6e-118">Proxy</span></span>](./proxy.md)|<span data-ttu-id="a0e6e-119">Позволяет использовать проверку подлинности на тыловом компьютере путем маршрутизации всех вызовов в Microsoft Graph через ваш тыл.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-119">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="a0e6e-120">Custom</span><span class="sxs-lookup"><span data-stu-id="a0e6e-120">Custom</span></span>](./custom.md)|<span data-ttu-id="a0e6e-121">Создайте настраиваемого поставщика, чтобы включить проверку подлинности и доступ к Microsoft Graph с помощью существующего кода проверки подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-121">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="initializing-a-provider"></a><span data-ttu-id="a0e6e-122">Инициализация поставщика</span><span class="sxs-lookup"><span data-stu-id="a0e6e-122">Initializing a provider</span></span>

<span data-ttu-id="a0e6e-123">Чтобы использовать поставщика в приложении, необходимо инициализировать нового поставщика, а затем установить его в качестве глобального поставщика в пространстве имен поставщиков.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-123">To use a provider in your app, you need to initialize a new provider and then set it as the global provider in the Providers namespace.</span></span> <span data-ttu-id="a0e6e-124">Рекомендуем сделать это перед началом использования какого-либо из компонентов.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-124">We recommend doing this before you start using any of the components.</span></span> <span data-ttu-id="a0e6e-125">Это можно сделать одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="a0e6e-125">You can do this one of two ways:</span></span>

<span data-ttu-id="a0e6e-126">**Вариант 1. Использование компонента поставщика**</span><span class="sxs-lookup"><span data-stu-id="a0e6e-126">**Option 1: Use the provider component**</span></span>

<span data-ttu-id="a0e6e-127">Версию компонента поставщика можно использовать непосредственно в HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-127">You can use the component version of the provider directly in your HTML.</span></span> <span data-ttu-id="a0e6e-128">За кадром новый поставщик инициализируются и устанавливается в качестве глобального поставщика.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-128">Behind the scenes, a new provider is initialized and set as the global provider.</span></span> <span data-ttu-id="a0e6e-129">В следующем примере показано, как использовать MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-129">The following example shows how to use the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

<span data-ttu-id="a0e6e-130">**Вариант 2. Инициализация в коде**</span><span class="sxs-lookup"><span data-stu-id="a0e6e-130">**Option 2: Initialize in code**</span></span>

<span data-ttu-id="a0e6e-131">Инициализация поставщика в коде JavaScript позволяет предоставить дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-131">Initializing your provider in your JavaScript code enables you to provide more options.</span></span> <span data-ttu-id="a0e6e-132">Для этого создайте новый экземпляр поставщика и установите значение свойства для поставщика, который вы `Providers.globalProvider` хотите использовать.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-132">To do this, create a new provider instance and set the value of the `Providers.globalProvider` property to the provider you'd like to use.</span></span> <span data-ttu-id="a0e6e-133">В следующем примере показано, как использовать MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-133">The following example shows how to use the MsalProvider.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> <span data-ttu-id="a0e6e-134">**Примечание.** Дополнительные сведения о том, как зарегистрировать приложение и получить ИД клиента, см. в примере создания приложения [Azure Active Directory.](../get-started/add-aad-app-registration.md)</span><span class="sxs-lookup"><span data-stu-id="a0e6e-134">**Note:** For details about how to register your app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>

## <a name="permission-scopes"></a><span data-ttu-id="a0e6e-135">Области разрешений</span><span class="sxs-lookup"><span data-stu-id="a0e6e-135">Permission Scopes</span></span>

<span data-ttu-id="a0e6e-136">Мы рекомендуем добавить все области разрешений, необходимые приложению, к атрибуту или свойству при инициализации поставщика (это не относится к поставщику `scopes` [SharePoint).](../providers/sharepoint.md)</span><span class="sxs-lookup"><span data-stu-id="a0e6e-136">We recommend adding all the permission scopes your application needs to the `scopes` attribute or property when initializing your provider (this does not apply to the [SharePoint provider](../providers/sharepoint.md)).</span></span> <span data-ttu-id="a0e6e-137">Это необязательный вариант, но позволит улучшить пользовательский интерфейс, выведя пользователю единый экран согласия со сводным списком разрешений, запрашиваемого всеми компонентами приложения, вместо того чтобы представлять отдельные экраны для каждого компонента.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-137">This is optional, but will improve your user experience by presenting a single consent screen to the user with an aggregated list of permissions requested by all components in your app, rather than presenting separate screens for each component.</span></span> <span data-ttu-id="a0e6e-138">В следующих примерах покажите, как это сделать с помощью MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-138">The following examples show how to do this with the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

<span data-ttu-id="a0e6e-139">Если вы инициализируете поставщика в коде, в свойстве предозначим области разрешений в `scopes` массиве.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-139">If you're initializing the provider in code, provide the permission scopes in an array in the `scopes` property.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

<span data-ttu-id="a0e6e-140">Список областей разрешений, необходимых каждому компоненту, можно найти в разделе разрешений **Microsoft Graph** на странице документации каждого компонента.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-140">You can find the list of permission scopes required by each component in the **Microsoft Graph permissions** section of each component's documentation page.</span></span>

## <a name="provider-state"></a><span data-ttu-id="a0e6e-141">Состояние поставщика</span><span class="sxs-lookup"><span data-stu-id="a0e6e-141">Provider state</span></span>

<span data-ttu-id="a0e6e-142">Поставщик отслеживает состояние проверки подлинности пользователя и передает его компонентам.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-142">The provider keeps track of the user's authentication state and communicates it to the components.</span></span> <span data-ttu-id="a0e6e-143">Например, когда пользователь успешно войдет, он обновляется до , сообщает компонентам, что теперь он может звонить `ProviderState` `SignedIn` в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-143">For example, when a user successfully signs in, the `ProviderState` is updated to `SignedIn`, signaling to the components that they are now able to make calls to Microsoft Graph.</span></span> <span data-ttu-id="a0e6e-144">В `ProviderState` этом коде определяются три состояния, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-144">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

<span data-ttu-id="a0e6e-145">В некоторых сценариях необходимо показать определенные функции или выполнить действие только после успешного выполнения пользователем.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-145">In some scenarios, you will want to show certain functionality or perform an action only after a user has successfully signed in.</span></span> <span data-ttu-id="a0e6e-146">Вы можете получить доступ к поставщику и проверить его состояние, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-146">You can access and check the provider state, as shown in the following example.</span></span>

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
<span data-ttu-id="a0e6e-147">Этот метод также можно использовать для получения уведомлений при изменениях состояния `Providers.onProviderUpdated` поставщика.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-147">You can also use the `Providers.onProviderUpdated` method to get notified whenever the state of the provider changes.</span></span>

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

const providerStateChanged = () => {
  if (Providers.globalProvider.state === ProviderState.SignedIn) {
    // user is now signed in
  }
}

// register a callback for when the state changes
Providers.onProviderUpdated(providerStateChanged);

// remove callback if necessary
Providers.removeProviderUpdatedListener(providerStateChanged);
```

## <a name="getting-an-access-token"></a><span data-ttu-id="a0e6e-148">Получение маркера доступа</span><span class="sxs-lookup"><span data-stu-id="a0e6e-148">Getting an access token</span></span>

<span data-ttu-id="a0e6e-149">Каждый поставщик предоставляет функцию, которая может получить текущий маркер доступа или получить новый маркер доступа `getAccessToken` для предоставленных областей.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-149">Each provider exposes a function called `getAccessToken` that can retrieve the current access token or retrieve a new access token for the provided scopes.</span></span> <span data-ttu-id="a0e6e-150">В следующем примере показано, как получить новый маркер доступа с `User.Read` областью разрешений.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-150">The following example shows how to get a new access token with the `User.Read` permission scope.</span></span>

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = Provider.globalProvider.getAccessToken({scopes: 'User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="a0e6e-151">Самостоятельное вызовы Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a0e6e-151">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="a0e6e-152">Все компоненты могут получить доступ к Microsoft Graph без какой-либо настройки, необходимой при инициализации поставщика (как описано в предыдущих разделах).</span><span class="sxs-lookup"><span data-stu-id="a0e6e-152">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous sections).</span></span> <span data-ttu-id="a0e6e-153">Если вы хотите самостоятельно звонить в Microsoft Graph, вы можете получить ссылку на тот же SDK Microsoft Graph, который используется компонентами.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-153">If you want to make your own calls to Microsoft Graph, you can do so by getting a reference to the same Microsoft Graph SDK used by the components.</span></span> <span data-ttu-id="a0e6e-154">Сначала получите ссылку на глобальный объект, а `IProvider` затем `graph` используйте объект, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-154">First, get a reference to the global `IProvider` and then use the `graph` object as shown:</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
<span data-ttu-id="a0e6e-155">В некоторых случаях может потребоваться передать дополнительные разрешения в зависимости от вызываемой API.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-155">There might be cases where you need to pass additional permissions, depending on the API you're calling.</span></span> <span data-ttu-id="a0e6e-156">В следующем примере показывается, как это можно сделать.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-156">The following example shows how to do this.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a><span data-ttu-id="a0e6e-157">Использование нескольких поставщиков</span><span class="sxs-lookup"><span data-stu-id="a0e6e-157">Using multiple providers</span></span>

<span data-ttu-id="a0e6e-158">В некоторых сценариях приложение будет работать в разных средах и для каждого из них потребуется другой поставщик.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-158">In some scenarios, your application will run in different environments and require a different provider for each.</span></span> <span data-ttu-id="a0e6e-159">Например, приложение может работать как веб-приложение и как вкладка Microsoft Teams, что означает, что вам может потребоваться использовать msalProvider и TeamsProvider.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-159">For example, the app might run as both a web application and a Microsoft Teams tab, which means you might need to use both the MsalProvider and the TeamsProvider.</span></span> <span data-ttu-id="a0e6e-160">В этом сценарии все компоненты поставщика имеют атрибут для создания цепочки отката, как показано `depends-on` в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-160">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

<span data-ttu-id="a0e6e-161">В этом сценарии MsalProvider будет использоваться, только если ваше приложение работает как веб-приложение и TeamsProvider не доступен в текущей среде.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-161">In this scenario, the MsalProvider will only be used if your app is running as a web application and the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="a0e6e-162">Чтобы выполнить то же самое в коде, можно использовать свойство `isAvailable` поставщика, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-162">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a><span data-ttu-id="a0e6e-163">Вход и вход пользователя</span><span class="sxs-lookup"><span data-stu-id="a0e6e-163">User Login/Logout</span></span>

<span data-ttu-id="a0e6e-164">При инициализации нужных поставщиков для приложения можно добавить [](../components/login.md) компонент входа набор средств, чтобы легко и быстро реализовать вход и вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-164">When you have the right providers initialized for your application, you can add the Toolkit's [Login component](../components/login.md) to easily and quickly implement user login and logout.</span></span> <span data-ttu-id="a0e6e-165">Компонент работает с поставщиком для обработки всей логики проверки подлинности и функций входа и входа в систему.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-165">The component works with the provider to handle all of the authentication logic and login/logout functionality.</span></span> <span data-ttu-id="a0e6e-166">В следующем примере используются MsalProvider и компонент Login.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-166">The following example uses the MsalProvider and the Login component.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="a0e6e-167">В сценариях, где вы хотите реализовать это самостоятельно, а не использовать компонент входа набор средств входа в систему, это можно сделать с помощью и методов `login` `logout` поставщика.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-167">In scenarios where you want to implement this yourself, rather than using the Toolkit's Login component, you can do so by using the `login` and `logout` methods of the provider.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="a0e6e-168">Реализация собственного поставщика</span><span class="sxs-lookup"><span data-stu-id="a0e6e-168">Implement your own provider</span></span>

<span data-ttu-id="a0e6e-169">В сценариях, где вы хотите добавить набор средств в приложение с уже существующим кодом проверки подлинности, можно создать настраиваемого поставщика, который подключается к вашему механизму проверки подлинности вместо использования наших предопределенных поставщиков.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-169">In scenarios where you want to add Toolkit components to an application with pre-existing authentication code, you can create a custom provider that hooks into your authentication mechanism, instead of using our predefined providers.</span></span> <span data-ttu-id="a0e6e-170">Набор средств предоставляет два способа создания новых поставщиков:</span><span class="sxs-lookup"><span data-stu-id="a0e6e-170">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="a0e6e-171">Создайте новый маркер доступа из кода проверки подлинности, передав `SimpleProvider` функцию.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-171">Create a new `SimpleProvider` that returns an access token from your authentication code by passing in a function.</span></span>
- <span data-ttu-id="a0e6e-172">Расширение `IProvider` абстрактного класса.</span><span class="sxs-lookup"><span data-stu-id="a0e6e-172">Extend the `IProvider` abstract class.</span></span>

<span data-ttu-id="a0e6e-173">Дополнительные сведения о каждом из них см. [в настраиваемом поставщике.](../providers/custom.md)</span><span class="sxs-lookup"><span data-stu-id="a0e6e-173">For more details about each one, see [custom providers](../providers/custom.md).</span></span>
