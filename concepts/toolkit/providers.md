---
title: Поставщики набора средств Microsoft Graph
description: Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 221258b49d9a5217829633c7882b9dd4f9d2a221
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955787"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="d81b0-103">Поставщики набора средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d81b0-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="d81b0-104">Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для всех компонентов.</span><span class="sxs-lookup"><span data-stu-id="d81b0-104">The Microsoft Graph Toolkit providers enable authentication and Microsoft Graph access for all components.</span></span> <span data-ttu-id="d81b0-105">Каждый поставщик предоставляет реализацию для получения необходимого маркера доступа для вызова API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d81b0-105">Each provider provides implementation for acquiring the necessary access token for calling the Microsoft Graph APIs.</span></span>

<span data-ttu-id="d81b0-106">Чтобы компоненты использовали поставщика, необходимо присвоить `Providers.globalProvider` свойству значение для поставщика, который вы хотите использовать.</span><span class="sxs-lookup"><span data-stu-id="d81b0-106">For the components to use a provider, you must set the `Providers.globalProvider` property to the value for a provider you'd like to use.</span></span>

<span data-ttu-id="d81b0-107">В приведенном ниже примере показано, как использовать Мсалпровидер.</span><span class="sxs-lookup"><span data-stu-id="d81b0-107">The following example shows how to use the MsalProvider.</span></span>

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

<span data-ttu-id="d81b0-108">В наборе средств реализованы следующие поставщики:</span><span class="sxs-lookup"><span data-stu-id="d81b0-108">The toolkit implements the following providers:</span></span>

- [<span data-ttu-id="d81b0-109">мсалпровидер</span><span class="sxs-lookup"><span data-stu-id="d81b0-109">MsalProvider</span></span>](./providers/msal.md)
- [<span data-ttu-id="d81b0-110">шарепоинтпровидер</span><span class="sxs-lookup"><span data-stu-id="d81b0-110">SharePointProvider</span></span>](./providers/sharepoint.md)
- [<span data-ttu-id="d81b0-111">теамспровидер</span><span class="sxs-lookup"><span data-stu-id="d81b0-111">TeamsProvider</span></span>](./providers/teams.md)
- [<span data-ttu-id="d81b0-112">проксипровидер</span><span class="sxs-lookup"><span data-stu-id="d81b0-112">ProxyProvider</span></span>](./providers/proxy.md)
- [<span data-ttu-id="d81b0-113">симплепровидер</span><span class="sxs-lookup"><span data-stu-id="d81b0-113">SimpleProvider</span></span>](./providers/custom.md)

<span data-ttu-id="d81b0-114">Вы можете создать поставщика в любое время.</span><span class="sxs-lookup"><span data-stu-id="d81b0-114">You can create a provider at any time.</span></span> <span data-ttu-id="d81b0-115">Рекомендуется создать поставщика перед использованием любого из компонентов.</span><span class="sxs-lookup"><span data-stu-id="d81b0-115">We recommend that you create the provider before you use any of the components.</span></span> <span data-ttu-id="d81b0-116">В этом разделе описывается, как инициализировать поставщика.</span><span class="sxs-lookup"><span data-stu-id="d81b0-116">This section describes how to initialize a provider.</span></span>

## <a name="providers-namespace"></a><span data-ttu-id="d81b0-117">Пространство имен поставщиков</span><span class="sxs-lookup"><span data-stu-id="d81b0-117">Providers namespace</span></span>

<span data-ttu-id="d81b0-118">`Providers` Пространство имен предоставляет следующие свойства и функции:</span><span class="sxs-lookup"><span data-stu-id="d81b0-118">The `Providers` namespace exposes the following properties and functions:</span></span>

- `globalProvider : IProvider`

<span data-ttu-id="d81b0-119">Задайте для этого свойства поставщик, который будет использоваться глобально.</span><span class="sxs-lookup"><span data-stu-id="d81b0-119">Set this property to a provider that you want to use globally.</span></span> <span data-ttu-id="d81b0-120">Все компоненты используют это свойство для получения ссылки на поставщика.</span><span class="sxs-lookup"><span data-stu-id="d81b0-120">All components use this property to get a reference to the provider.</span></span> <span data-ttu-id="d81b0-121">При задании этого свойства `onProvidersChanged` событие будет срабатывать.</span><span class="sxs-lookup"><span data-stu-id="d81b0-121">Setting this property will fire the `onProvidersChanged` event.</span></span>

- `function onProviderUpdated(callbackFunction)`

<span data-ttu-id="d81b0-122">`callbackFunction` Функция будет вызываться при изменении поставщика или при изменении состояния поставщика.</span><span class="sxs-lookup"><span data-stu-id="d81b0-122">The `callbackFunction` function will be called when a provider is changed or when the state of a provider changes.</span></span> <span data-ttu-id="d81b0-123">В `ProvidersChangedState` функцию передается значение перечисления, которое указывает, что было обновлено.</span><span class="sxs-lookup"><span data-stu-id="d81b0-123">A `ProvidersChangedState` enum value will be passed to the function to indicate what updated.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="d81b0-124">Реализация собственного поставщика</span><span class="sxs-lookup"><span data-stu-id="d81b0-124">Implement your own provider</span></span>

<span data-ttu-id="d81b0-125">В наборе инструментов предусмотрено два способа создания новых поставщиков:</span><span class="sxs-lookup"><span data-stu-id="d81b0-125">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="d81b0-126">Создайте новый `SimpleProvider` , передав функцию для получения маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="d81b0-126">Create a new `SimpleProvider` by passing in a function for getting an access token.</span></span>
- <span data-ttu-id="d81b0-127">Расширьте `IProvider` абстрактный класс.</span><span class="sxs-lookup"><span data-stu-id="d81b0-127">Extend the `IProvider` abstract class.</span></span>

<span data-ttu-id="d81b0-128">Дополнительные сведения о каждом из них можно найти в разделе [Настраиваемые поставщики](./providers/custom.md).</span><span class="sxs-lookup"><span data-stu-id="d81b0-128">For more details about each one, see [custom providers](./providers/custom.md).</span></span>

## <a name="using-multiple-providers"></a><span data-ttu-id="d81b0-129">Использование нескольких поставщиков</span><span class="sxs-lookup"><span data-stu-id="d81b0-129">Using multiple providers</span></span>

<span data-ttu-id="d81b0-130">В некоторых сценариях приложение будет запускаться в другой среде и потребует другого поставщика.</span><span class="sxs-lookup"><span data-stu-id="d81b0-130">In some scenarios, your application will run in a different environment and require a different provider.</span></span> <span data-ttu-id="d81b0-131">Например, приложение может работать в качестве веб-приложения и вкладки Microsoft Teams, и вам может потребоваться использовать Мсалпровидер и Теамспровидер.</span><span class="sxs-lookup"><span data-stu-id="d81b0-131">For example, the app might run as both a web application and a Microsoft Teams tab and you might need to use the MsalProvider and the TeamsProvider.</span></span> <span data-ttu-id="d81b0-132">В этом сценарии все компоненты поставщика имеют `depends-on` атрибут для создания резервной цепочки, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="d81b0-132">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

<span data-ttu-id="d81b0-133">В этом сценарии Мсалпровидер будет использоваться только в том случае, если Теамспровидер недоступен в текущей среде.</span><span class="sxs-lookup"><span data-stu-id="d81b0-133">In this scenario, the MsalProvider will only be used if the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="d81b0-134">Чтобы сделать то же самое в коде, можно использовать `isAvailable` свойство поставщика, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="d81b0-134">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="d81b0-135">Выполнение собственных вызовов в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d81b0-135">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="d81b0-136">Все компоненты могут получать доступ к Microsoft Graph без какой-либо настройки, если вы инициализируем поставщик (как описано в предыдущем разделе).</span><span class="sxs-lookup"><span data-stu-id="d81b0-136">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous section).</span></span> <span data-ttu-id="d81b0-137">Чтобы получить ссылку на тот же пакет SDK Microsoft Graph, используемый компонентами, сначала получите ссылку на глобальный Ипровидер, а затем используйте `Graph` объект, как показано ниже:</span><span class="sxs-lookup"><span data-stu-id="d81b0-137">To get a reference to the same Microsoft Graph SDK used by the components, first get a reference to the global IProvider and then use the `Graph` object, as shown:</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

<span data-ttu-id="d81b0-138">Возможны случаи, когда вам потребуется передать дополнительные разрешения в зависимости от интерфейса API, который вы вызываете.</span><span class="sxs-lookup"><span data-stu-id="d81b0-138">There might be cases were you will need to pass additional permissions, depending on the API you're calling.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

<span data-ttu-id="d81b0-139">`graph` Объект — это экземпляр [пакета SDK JavaScript для Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) , который можно использовать для совершения вызовов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d81b0-139">The `graph` object is an instance of the [Microsoft Graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) and you can use it to make any calls to Microsoft Graph.</span></span>
