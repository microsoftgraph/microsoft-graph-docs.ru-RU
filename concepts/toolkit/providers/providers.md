---
title: Поставщики набор средств Microsoft Graph
description: Поставщики набор средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 1bebdb6bd2445873d8b45412b61f8793673db216
ms.sourcegitcommit: fdd69d362d1debc7b08e78269d59b531f9dfdaae
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697181"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="26258-103">Поставщики набор средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="26258-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="26258-104">Поставщики набор средств Microsoft Graph позволяют приложению проверить подлинность с помощью Microsoft Identity и получить доступ к Microsoft Graph только в нескольких строках кода.</span><span class="sxs-lookup"><span data-stu-id="26258-104">The Microsoft Graph Toolkit providers enable your application to authenticate with Microsoft Identity and access Microsoft Graph in only few lines of code.</span></span> <span data-ttu-id="26258-105">Каждый поставщик обрабатывает проверку подлинности пользователей и приобретает маркеры доступа для вызова API Microsoft Graph, чтобы вам не нужно было самостоятельно писать этот код.</span><span class="sxs-lookup"><span data-stu-id="26258-105">Each provider handles user authentication and acquiring the access tokens to call Microsoft Graph APIs, so that you don't have to write this code yourself.</span></span> 

<span data-ttu-id="26258-106">Вы можете использовать поставщики самостоятельно, без компонентов, чтобы быстро реализовать проверку подлинности для вашего приложения и сделать вызовы в Microsoft Graph через SDK клиента JavaScript.</span><span class="sxs-lookup"><span data-stu-id="26258-106">You can use the providers on their own, without components, to quickly implement authentication for your app and make calls to Microsoft Graph via the JavaScript client SDK.</span></span>

<span data-ttu-id="26258-107">Поставщики необходимы при использовании компонентов Microsoft Graph набор средств, так как компоненты используют их для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="26258-107">The providers are required when using the Microsoft Graph Toolkit components as the components use them to access Microsoft Graph.</span></span> <span data-ttu-id="26258-108">Если у вас уже есть собственная проверка подлинности и вы хотите использовать компоненты, вместо этого можно использовать [настраиваемый поставщик.](./custom.md)</span><span class="sxs-lookup"><span data-stu-id="26258-108">If you already have your own authentication and want to use the components, you can use a [custom provider](./custom.md) instead.</span></span>

<span data-ttu-id="26258-109">В набор средств входят следующие поставщики.</span><span class="sxs-lookup"><span data-stu-id="26258-109">The Toolkit includes the following providers.</span></span>

|<span data-ttu-id="26258-110">Поставщики</span><span class="sxs-lookup"><span data-stu-id="26258-110">Providers</span></span>|<span data-ttu-id="26258-111">Описание</span><span class="sxs-lookup"><span data-stu-id="26258-111">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="26258-112">MSAL</span><span class="sxs-lookup"><span data-stu-id="26258-112">Msal</span></span>](./msal.md)|<span data-ttu-id="26258-113">Использует MSAL.js для регистрации пользователей и приобретения маркеров для использования с Помощью Microsoft Graph в веб-приложении.</span><span class="sxs-lookup"><span data-stu-id="26258-113">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph in a web application.</span></span>|
|[<span data-ttu-id="26258-114">Электрон</span><span class="sxs-lookup"><span data-stu-id="26258-114">Electron</span></span>](./electron.md)|<span data-ttu-id="26258-115">Проверка подлинности и обеспечивает доступ Microsoft Graph к компонентам в приложениях Electron.</span><span class="sxs-lookup"><span data-stu-id="26258-115">Authenticates and provides Microsoft Graph access to components inside of Electron apps.</span></span>|
|[<span data-ttu-id="26258-116">SharePoint</span><span class="sxs-lookup"><span data-stu-id="26258-116">SharePoint</span></span>](./sharepoint.md)|<span data-ttu-id="26258-117">Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.</span><span class="sxs-lookup"><span data-stu-id="26258-117">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="26258-118">Teams</span><span class="sxs-lookup"><span data-stu-id="26258-118">Teams</span></span>](./teams.md)|<span data-ttu-id="26258-119">Проверка подлинности и доступ Microsoft Graph к компонентам на вкладке Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="26258-119">Authenticates and provides Microsoft Graph access to components inside  Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="26258-120">Прокси-сервер</span><span class="sxs-lookup"><span data-stu-id="26258-120">Proxy</span></span>](./proxy.md)|<span data-ttu-id="26258-121">Позволяет использовать проверку подлинности на внутреннем сервере с помощью маршрутизации всех вызовов Microsoft Graph через внутренний сервер.</span><span class="sxs-lookup"><span data-stu-id="26258-121">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="26258-122">Настраиваемый</span><span class="sxs-lookup"><span data-stu-id="26258-122">Custom</span></span>](./custom.md)|<span data-ttu-id="26258-123">Создание настраиваемого поставщика для включения проверки подлинности и доступа к Microsoft Graph с помощью существующего кода проверки подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="26258-123">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="initializing-a-provider"></a><span data-ttu-id="26258-124">Инициализация поставщика</span><span class="sxs-lookup"><span data-stu-id="26258-124">Initializing a provider</span></span>

<span data-ttu-id="26258-125">Чтобы использовать поставщика в приложении, необходимо инициализировать нового поставщика, а затем установить его в качестве глобального поставщика в пространстве имен поставщиков.</span><span class="sxs-lookup"><span data-stu-id="26258-125">To use a provider in your app, you need to initialize a new provider and then set it as the global provider in the Providers namespace.</span></span> <span data-ttu-id="26258-126">Мы рекомендуем сделать это, прежде чем приступить к использованию любого из компонентов.</span><span class="sxs-lookup"><span data-stu-id="26258-126">We recommend doing this before you start using any of the components.</span></span> <span data-ttu-id="26258-127">Это можно сделать одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="26258-127">You can do this one of two ways:</span></span>

<span data-ttu-id="26258-128">**Вариант 1. Использование компонента поставщика**</span><span class="sxs-lookup"><span data-stu-id="26258-128">**Option 1: Use the provider component**</span></span>

<span data-ttu-id="26258-129">Компонентную версию поставщика можно использовать непосредственно в HTML.</span><span class="sxs-lookup"><span data-stu-id="26258-129">You can use the component version of the provider directly in your HTML.</span></span> <span data-ttu-id="26258-130">За кулисами новый поставщик инициализируются и устанавливается как глобальный поставщик.</span><span class="sxs-lookup"><span data-stu-id="26258-130">Behind the scenes, a new provider is initialized and set as the global provider.</span></span> <span data-ttu-id="26258-131">В следующем примере показано, как использовать MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="26258-131">The following example shows how to use the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

<span data-ttu-id="26258-132">**Вариант 2. Инициализация кода**</span><span class="sxs-lookup"><span data-stu-id="26258-132">**Option 2: Initialize in code**</span></span>

<span data-ttu-id="26258-133">Инициализация поставщика в коде JavaScript позволяет предоставить дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="26258-133">Initializing your provider in your JavaScript code enables you to provide more options.</span></span> <span data-ttu-id="26258-134">Для этого создайте новый экземпляр поставщика и установите значение свойства поставщику, который вы `Providers.globalProvider` хотите использовать.</span><span class="sxs-lookup"><span data-stu-id="26258-134">To do this, create a new provider instance and set the value of the `Providers.globalProvider` property to the provider you'd like to use.</span></span> <span data-ttu-id="26258-135">В следующем примере показано, как использовать MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="26258-135">The following example shows how to use the MsalProvider.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> <span data-ttu-id="26258-136">**Примечание:** Дополнительные сведения о том, как зарегистрировать приложение и получить клиентский ID, см. в материале [Create an Azure Active Directory app.](../get-started/add-aad-app-registration.md)</span><span class="sxs-lookup"><span data-stu-id="26258-136">**Note:** For details about how to register your app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>

## <a name="permission-scopes"></a><span data-ttu-id="26258-137">Области разрешений</span><span class="sxs-lookup"><span data-stu-id="26258-137">Permission Scopes</span></span>

<span data-ttu-id="26258-138">Мы рекомендуем добавить все области разрешений, необходимые вашему приложению, к атрибуту или свойству при инициализации поставщика (это не относится к `scopes` [поставщику SharePoint).](../providers/sharepoint.md)</span><span class="sxs-lookup"><span data-stu-id="26258-138">We recommend adding all the permission scopes your application needs to the `scopes` attribute or property when initializing your provider (this does not apply to the [SharePoint provider](../providers/sharepoint.md)).</span></span> <span data-ttu-id="26258-139">Это необязательный вариант, но улучшит пользовательский интерфейс, презентуя пользователю единый экран согласия со сводным списком разрешений, запрашиваемого всеми компонентами в вашем приложении, вместо того чтобы представлять отдельные экраны для каждого компонента.</span><span class="sxs-lookup"><span data-stu-id="26258-139">This is optional, but will improve your user experience by presenting a single consent screen to the user with an aggregated list of permissions requested by all components in your app, rather than presenting separate screens for each component.</span></span> <span data-ttu-id="26258-140">В следующих примерах покажите, как это сделать с MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="26258-140">The following examples show how to do this with the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

<span data-ttu-id="26258-141">Если вы инициализируете поставщика в коде, указать области разрешений в массиве `scopes` в свойстве.</span><span class="sxs-lookup"><span data-stu-id="26258-141">If you're initializing the provider in code, provide the permission scopes in an array in the `scopes` property.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

<span data-ttu-id="26258-142">Список областей разрешений, необходимых каждому компоненту, можно найти в разделе **Разрешения Microsoft Graph** на странице документации каждого компонента.</span><span class="sxs-lookup"><span data-stu-id="26258-142">You can find the list of permission scopes required by each component in the **Microsoft Graph permissions** section of each component's documentation page.</span></span>

## <a name="provider-state"></a><span data-ttu-id="26258-143">Состояние поставщика</span><span class="sxs-lookup"><span data-stu-id="26258-143">Provider state</span></span>

<span data-ttu-id="26258-144">Поставщик отслеживает состояние проверки подлинности пользователя и передает его компонентам.</span><span class="sxs-lookup"><span data-stu-id="26258-144">The provider keeps track of the user's authentication state and communicates it to the components.</span></span> <span data-ttu-id="26258-145">Например, когда пользователь успешно войдет, пользователь обновляется до , сигнализая компонентам, что они теперь могут делать вызовы `ProviderState` `SignedIn` в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="26258-145">For example, when a user successfully signs in, the `ProviderState` is updated to `SignedIn`, signaling to the components that they are now able to make calls to Microsoft Graph.</span></span> <span data-ttu-id="26258-146">Как показано, перечисление `ProviderState` определяет три состояния.</span><span class="sxs-lookup"><span data-stu-id="26258-146">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

<span data-ttu-id="26258-147">В некоторых сценариях необходимо показать определенные функции или выполнить действие только после успешной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="26258-147">In some scenarios, you will want to show certain functionality or perform an action only after a user has successfully signed in.</span></span> <span data-ttu-id="26258-148">Вы можете получить доступ и проверить состояние поставщика, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="26258-148">You can access and check the provider state, as shown in the following example.</span></span>

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
<span data-ttu-id="26258-149">Вы также можете использовать метод для получения уведомлений всякий раз, `Providers.onProviderUpdated` когда меняется состояние поставщика.</span><span class="sxs-lookup"><span data-stu-id="26258-149">You can also use the `Providers.onProviderUpdated` method to get notified whenever the state of the provider changes.</span></span>

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

## <a name="getting-an-access-token"></a><span data-ttu-id="26258-150">Получение маркера доступа</span><span class="sxs-lookup"><span data-stu-id="26258-150">Getting an access token</span></span>

<span data-ttu-id="26258-151">Каждый поставщик предоставляет функцию, которая может получить текущий маркер доступа или получить новый маркер доступа `getAccessToken` для предоставленных областей.</span><span class="sxs-lookup"><span data-stu-id="26258-151">Each provider exposes a function called `getAccessToken` that can retrieve the current access token or retrieve a new access token for the provided scopes.</span></span> <span data-ttu-id="26258-152">В следующем примере показано, как получить новый маркер доступа с `User.Read` областью разрешений.</span><span class="sxs-lookup"><span data-stu-id="26258-152">The following example shows how to get a new access token with the `User.Read` permission scope.</span></span>

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = await Providers.globalProvider.getAccessToken({scopes: ['User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="26258-153">Создание собственных вызовов в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="26258-153">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="26258-154">Все компоненты могут получать доступ к Microsoft Graph без каких-либо настроек, необходимых при инициализации поставщика (как описано в предыдущих разделах).</span><span class="sxs-lookup"><span data-stu-id="26258-154">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous sections).</span></span> <span data-ttu-id="26258-155">Если вы хотите сделать собственные вызовы в Microsoft Graph, вы можете сделать это, получив ссылку на тот же SDK Microsoft Graph, используемый компонентами.</span><span class="sxs-lookup"><span data-stu-id="26258-155">If you want to make your own calls to Microsoft Graph, you can do so by getting a reference to the same Microsoft Graph SDK used by the components.</span></span> <span data-ttu-id="26258-156">Сначала получите ссылку на глобальный, а `IProvider` затем используйте `graph` объект, как показано:</span><span class="sxs-lookup"><span data-stu-id="26258-156">First, get a reference to the global `IProvider` and then use the `graph` object as shown:</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
<span data-ttu-id="26258-157">Могут быть случаи, когда вам необходимо передать дополнительные разрешения в зависимости от API, который вы вызываете.</span><span class="sxs-lookup"><span data-stu-id="26258-157">There might be cases where you need to pass additional permissions, depending on the API you're calling.</span></span> <span data-ttu-id="26258-158">В следующем примере показывается, как это можно сделать.</span><span class="sxs-lookup"><span data-stu-id="26258-158">The following example shows how to do this.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a><span data-ttu-id="26258-159">Использование нескольких поставщиков</span><span class="sxs-lookup"><span data-stu-id="26258-159">Using multiple providers</span></span>

<span data-ttu-id="26258-160">В некоторых сценариях приложение будет работать в разных средах и для каждого из них потребуется другой поставщик.</span><span class="sxs-lookup"><span data-stu-id="26258-160">In some scenarios, your application will run in different environments and require a different provider for each.</span></span> <span data-ttu-id="26258-161">Например, приложение может работать как веб-приложение, так и вкладка Microsoft Teams, что означает, что вам может потребоваться использовать как MsalProvider, так и TeamsProvider.</span><span class="sxs-lookup"><span data-stu-id="26258-161">For example, the app might run as both a web application and a Microsoft Teams tab, which means you might need to use both the MsalProvider and the TeamsProvider.</span></span> <span data-ttu-id="26258-162">Для этого сценария все компоненты поставщика имеют атрибут для создания цепочки откатов, как показано `depends-on` в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="26258-162">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

<span data-ttu-id="26258-163">В этом сценарии msalProvider будет использоваться только в том случае, если ваше приложение работает в качестве веб-приложения, а TeamsProvider не доступен в текущей среде.</span><span class="sxs-lookup"><span data-stu-id="26258-163">In this scenario, the MsalProvider will only be used if your app is running as a web application and the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="26258-164">Чтобы выполнить то же самое в коде, можно использовать свойство `isAvailable` на поставщике, как показано.</span><span class="sxs-lookup"><span data-stu-id="26258-164">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a><span data-ttu-id="26258-165">Вход пользователя/вход в систему</span><span class="sxs-lookup"><span data-stu-id="26258-165">User Login/Logout</span></span>

<span data-ttu-id="26258-166">Если у вас есть правильные поставщики, инициализированные для вашего приложения, вы можете добавить компонент [login](../components/login.md) набор средств для легкой и быстрой реализации входа и входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="26258-166">When you have the right providers initialized for your application, you can add the Toolkit's [Login component](../components/login.md) to easily and quickly implement user login and logout.</span></span> <span data-ttu-id="26258-167">Компонент работает с поставщиком для обработки всей логики проверки подлинности и функций входа/входа.</span><span class="sxs-lookup"><span data-stu-id="26258-167">The component works with the provider to handle all of the authentication logic and login/logout functionality.</span></span> <span data-ttu-id="26258-168">В следующем примере используются компонент MsalProvider и компонент Login.</span><span class="sxs-lookup"><span data-stu-id="26258-168">The following example uses the MsalProvider and the Login component.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="26258-169">В сценариях, в которых вы хотите реализовать это самостоятельно, а не использовать компонент login набор средств, вы можете сделать это с помощью и методов `login` `logout` поставщика.</span><span class="sxs-lookup"><span data-stu-id="26258-169">In scenarios where you want to implement this yourself, rather than using the Toolkit's Login component, you can do so by using the `login` and `logout` methods of the provider.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="26258-170">Реализация собственного поставщика</span><span class="sxs-lookup"><span data-stu-id="26258-170">Implement your own provider</span></span>

<span data-ttu-id="26258-171">В сценариях, когда необходимо добавить набор средств в приложение с уже существующим кодом проверки подлинности, можно создать настраиваемого поставщика, который подключается к вашему механизму проверки подлинности, а не с помощью наших предопределяющих поставщиков.</span><span class="sxs-lookup"><span data-stu-id="26258-171">In scenarios where you want to add Toolkit components to an application with pre-existing authentication code, you can create a custom provider that hooks into your authentication mechanism, instead of using our predefined providers.</span></span> <span data-ttu-id="26258-172">Набор инструментов предоставляет два способа создания новых поставщиков:</span><span class="sxs-lookup"><span data-stu-id="26258-172">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="26258-173">Создайте новый маркер доступа из кода проверки подлинности, передав `SimpleProvider` функцию.</span><span class="sxs-lookup"><span data-stu-id="26258-173">Create a new `SimpleProvider` that returns an access token from your authentication code by passing in a function.</span></span>
- <span data-ttu-id="26258-174">Расширение `IProvider` абстрактного класса.</span><span class="sxs-lookup"><span data-stu-id="26258-174">Extend the `IProvider` abstract class.</span></span>

<span data-ttu-id="26258-175">Дополнительные сведения о каждом из них см. в [пользовательских поставщиках.](../providers/custom.md)</span><span class="sxs-lookup"><span data-stu-id="26258-175">For more details about each one, see [custom providers](../providers/custom.md).</span></span>
