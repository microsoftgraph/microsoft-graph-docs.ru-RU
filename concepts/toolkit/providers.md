---
title: Поставщики набора средств Microsoft Graph
description: Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 52b0510fdc79253cb2a448b7a454b1dcfaf01bb9
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275726"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="5c4f4-103">Поставщики набора средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5c4f4-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="5c4f4-104">Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-104">The Microsoft Graph Toolkit providers enable authentication and Microsoft Graph access for all components.</span></span> <span data-ttu-id="5c4f4-105">Каждый поставщик предоставляет реализацию для получения необходимого маркера доступа для вызова API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-105">Each provider provides implementation for acquiring the necessary access token for calling the Microsoft Graph APIs.</span></span>

<span data-ttu-id="5c4f4-106">Чтобы компоненты использовали поставщика, необходимо присвоить `Providers.globalProvider` свойству значение для поставщика, который вы хотите использовать.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-106">For the components to use a provider, you must set the `Providers.globalProvider` property to the value for a provider you'd like to use.</span></span>

<span data-ttu-id="5c4f4-107">В приведенном ниже примере показано, как использовать Мсалпровидер.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-107">The following example shows how to use the MsalProvider.</span></span>

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

<span data-ttu-id="5c4f4-108">В наборе средств реализованы следующие поставщики:</span><span class="sxs-lookup"><span data-stu-id="5c4f4-108">The toolkit implements the following providers:</span></span>

- [<span data-ttu-id="5c4f4-109">мсалпровидер</span><span class="sxs-lookup"><span data-stu-id="5c4f4-109">MsalProvider</span></span>](./providers/msal.md)
- [<span data-ttu-id="5c4f4-110">шарепоинтпровидер</span><span class="sxs-lookup"><span data-stu-id="5c4f4-110">SharePointProvider</span></span>](./providers/sharepoint.md)
- [<span data-ttu-id="5c4f4-111">теамспровидер</span><span class="sxs-lookup"><span data-stu-id="5c4f4-111">TeamsProvider</span></span>](./providers/teams.md)
- <span data-ttu-id="5c4f4-112">Поставщик надстроек Office (ожидается в ближайшее время)</span><span class="sxs-lookup"><span data-stu-id="5c4f4-112">Office Add-ins provider (coming soon)</span></span>

## <a name="get-started"></a><span data-ttu-id="5c4f4-113">Начало работы</span><span class="sxs-lookup"><span data-stu-id="5c4f4-113">Get started</span></span>

<span data-ttu-id="5c4f4-114">Вы можете создать поставщика в любое время.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-114">You can create a provider at any time.</span></span> <span data-ttu-id="5c4f4-115">Рекомендуется создать поставщика перед использованием любого из компонентов.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-115">We recommend that you create the provider before you use any of the components.</span></span> <span data-ttu-id="5c4f4-116">В этом разделе описывается, как инициализировать поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-116">This section describes how to initialize a provider.</span></span>

<span data-ttu-id="5c4f4-117">`Providers` Глобальная переменная предоставляет следующие свойства и функции</span><span class="sxs-lookup"><span data-stu-id="5c4f4-117">The `Providers` global variable exposes the following properties and functions</span></span>

- `globalProvider : IProvider`

<span data-ttu-id="5c4f4-118">Задайте для этого свойства поставщик, который будет использоваться глобально.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-118">Set this property to a provider that you want to use globally.</span></span> <span data-ttu-id="5c4f4-119">Все компоненты используют это свойство для получения ссылки на поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-119">All components use this property to get a reference to the provider.</span></span> <span data-ttu-id="5c4f4-120">При задании этого свойства `onProvidersChanged` событие будет срабатывать.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-120">Setting this property will fire the `onProvidersChanged` event.</span></span>

- `function onProviderUpdated(callbackFunction)`

<span data-ttu-id="5c4f4-121">`callbackFunction` Функция будет вызываться при изменении поставщика или при изменении состояния поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-121">The `callbackFunction` function will be called when a provider is changed or when the state of a provider changes.</span></span> <span data-ttu-id="5c4f4-122">В `ProvidersChangedState` функцию передается значение перечисления, которое указывает, что было обновлено.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-122">A `ProvidersChangedState` enum value will be passed to the function to indicate what updated.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="5c4f4-123">Реализация собственного поставщика</span><span class="sxs-lookup"><span data-stu-id="5c4f4-123">Implement your own provider</span></span>

<span data-ttu-id="5c4f4-124">В наборе инструментов предусмотрено два способа создания новых поставщиков:</span><span class="sxs-lookup"><span data-stu-id="5c4f4-124">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="5c4f4-125">Создание нового `SimpleProvider` путем передачи функции для получения маркера доступа</span><span class="sxs-lookup"><span data-stu-id="5c4f4-125">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="5c4f4-126">Расширение `IProvider` абстрактного класса</span><span class="sxs-lookup"><span data-stu-id="5c4f4-126">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="5c4f4-127">Дополнительные сведения о каждом из них содержатся в документации по [настраиваемым поставщикам](./providers/custom.md) .</span><span class="sxs-lookup"><span data-stu-id="5c4f4-127">Read more about each one in the [custom providers](./providers/custom.md) documentation.</span></span>

## <a name="using-multiple-providers"></a><span data-ttu-id="5c4f4-128">Использование нескольких поставщиков</span><span class="sxs-lookup"><span data-stu-id="5c4f4-128">Using multiple providers</span></span>

<span data-ttu-id="5c4f4-129">В некоторых сценариях приложение будет запускаться в другой среде и потребует другого поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-129">In some scenarios your application will run in a different environment and require a different provider.</span></span> <span data-ttu-id="5c4f4-130">Например, приложение может работать в качестве веб-приложения и вкладки Microsoft Teams, и вам может потребоваться использовать Мсалпровидер и Теамспровидер.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-130">For example, the app might run as both a web application and a Microsoft Teams tab and you might need to use the MsalProvider and the TeamsProvider.</span></span> <span data-ttu-id="5c4f4-131">В этом сценарии все компоненты поставщика имеют `depends-on` атрибут для создания резервной цепочки, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-131">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

<span data-ttu-id="5c4f4-132">В этом сценарии Мсалпровидер будет использоваться только в том случае, если Теамспровидер недоступен в текущей среде.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-132">In this scenario, the MsalProvider will only be used if the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="5c4f4-133">Чтобы сделать то же самое в коде, можно использовать `isAvailable` свойство поставщика, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-133">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="5c4f4-134">Выполнение собственных вызовов в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5c4f4-134">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="5c4f4-135">Все компоненты могут получать доступ к Microsoft Graph без какой-либо настройки, если вы инициализируем поставщик (как описано в предыдущем разделе).</span><span class="sxs-lookup"><span data-stu-id="5c4f4-135">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous section).</span></span> <span data-ttu-id="5c4f4-136">Чтобы получить ссылку на тот же пакет SDK Microsoft Graph, используемый компонентами, сначала получите ссылку на глобальный Ипровидер, а затем используйте `Graph` объект, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-136">To get a reference to the same Microsoft Graph SDK used by the components, first get a reference to the global IProvider and then use the `Graph` object, as shown.</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

<span data-ttu-id="5c4f4-137">Возможны случаи, когда вам потребуется передать дополнительные разрешения в зависимости от интерфейса API, который вы вызываете.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-137">There might be cases were you will need to pass additional permissions, depending on the API you're calling.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

<span data-ttu-id="5c4f4-138">`graph` Объект — это экземпляр [пакета SDK JavaScript для Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) , который можно использовать для совершения вызовов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5c4f4-138">The `graph` object is an instance of the [Microsoft Graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) and you can use it to make any calls to Microsoft Graph.</span></span>
