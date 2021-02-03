---
title: Поставщик прокси
description: Поставщик прокси-сервера позволяет использовать собственную проверку подлинности на стороне сервера с microsoft Graph набор средств.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c62718471c361cd9537bc8ee098c33e7b65830ec
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092255"
---
# <a name="proxy-provider"></a><span data-ttu-id="54e96-103">Поставщик прокси</span><span class="sxs-lookup"><span data-stu-id="54e96-103">Proxy provider</span></span>

<span data-ttu-id="54e96-104">При использовании поставщика прокси-сервера можно использовать серверную проверку подлинности (например, поток "От имени" Auth2.0) для работы microsoft Graph набор средств путем маршрутизации всех вызовов в Microsoft Graph через собственный сервер.</span><span class="sxs-lookup"><span data-stu-id="54e96-104">When you use the proxy provider, you can use your backend authentication (such as Auth2.0 On-Behalf-Of flow) to power the Microsoft Graph Toolkit by routing all calls to Microsoft Graph through your own backend.</span></span>

<span data-ttu-id="54e96-105">Во второй службе должен быть доступ к API, который будет вызываться для каждого вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="54e96-105">Your backend service must expose an API that will be called for every call to Microsoft Graph.</span></span> <span data-ttu-id="54e96-106">Например, когда компонент пытается получить ресурс, ProxyProvider будет вызывать базовый API и прибавлять этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="54e96-106">For example, when a component attempts to get a resource, the ProxyProvider will instead call your base API and append that resource.</span></span>

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

<span data-ttu-id="54e96-107">После этого реализация API должна вызывать Microsoft Graph от имени пользователя и возвращать результаты компоненту.</span><span class="sxs-lookup"><span data-stu-id="54e96-107">Your API implementation should then call Microsoft Graph on behalf of the user and return the results to the component.</span></span>

<span data-ttu-id="54e96-108">Пример реализации см. в примере [ASP.NET MVC.](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc)</span><span class="sxs-lookup"><span data-stu-id="54e96-108">For an implementation example, see the [ASP.NET MVC sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc).</span></span> 

<span data-ttu-id="54e96-109">Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="54e96-109">To learn more about authentication providers, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="54e96-110">Начало работы</span><span class="sxs-lookup"><span data-stu-id="54e96-110">Get started</span></span>

<span data-ttu-id="54e96-111">Поставщик прокси-сервера можно инициализировать в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="54e96-111">You can initialize the proxy provider in HTML or JavaScript.</span></span> <span data-ttu-id="54e96-112">Это следует сделать только один раз для каждой страницы.</span><span class="sxs-lookup"><span data-stu-id="54e96-112">You should do this only once per page.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="54e96-113">Инициализация на HTML-странице</span><span class="sxs-lookup"><span data-stu-id="54e96-113">Initialize in your HTML page</span></span>

<span data-ttu-id="54e96-114">Инициализация поставщика прокси-сервера в HTML является простейшим способом определения собственного маршрута для пользовательской проверки подлинности на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="54e96-114">Initializing the proxy provider in HTML is the simplest way to define your own route for custom server-side authentication.</span></span> <span data-ttu-id="54e96-115">С помощью `mgt-proxy-provider` компонента можно настроить **url-адрес graph-proxy-url.**</span><span class="sxs-lookup"><span data-stu-id="54e96-115">Use the `mgt-proxy-provider` component to set the **graph-proxy-url**.</span></span> <span data-ttu-id="54e96-116">При этом определенный поставщик прокси-сервера будет установлен в качестве глобального поставщика.</span><span class="sxs-lookup"><span data-stu-id="54e96-116">This will set the defined proxy provider as the global provider.</span></span>

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| <span data-ttu-id="54e96-117">Атрибут</span><span class="sxs-lookup"><span data-stu-id="54e96-117">Attribute</span></span> | <span data-ttu-id="54e96-118">Описание</span><span class="sxs-lookup"><span data-stu-id="54e96-118">Description</span></span> |
| --- | --- |
| <span data-ttu-id="54e96-119">graph-proxy-url</span><span class="sxs-lookup"><span data-stu-id="54e96-119">graph-proxy-url</span></span>  | <span data-ttu-id="54e96-120">Базовый URL-адрес прокси-API.</span><span class="sxs-lookup"><span data-stu-id="54e96-120">Base URL for the proxy API.</span></span> |


### <a name="initialize-in-javascript"></a><span data-ttu-id="54e96-121">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="54e96-121">Initialize in JavaScript</span></span>

<span data-ttu-id="54e96-122">Вы можете предоставить дополнительные параметры, инициализируя поставщика в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="54e96-122">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

<span data-ttu-id="54e96-123">При желании можно отправлять дополнительные заголовки с каждым запросом в прокси-API, используя дополнительную функцию в качестве второго параметра в конструкторе.</span><span class="sxs-lookup"><span data-stu-id="54e96-123">Optionally, you can send additional headers with each request to your proxy api by using an optional function as the second parameter in the constructor.</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
);
```

<span data-ttu-id="54e96-124">Это полезно, если вам нужно передать маркеры или другие заглавные символы на ваш тыл.</span><span class="sxs-lookup"><span data-stu-id="54e96-124">This is useful when you need to pass tokens or other headers to your backend.</span></span>

<span data-ttu-id="54e96-125">Если вы будете использовать компонент, необходимо также указать и функции `mgt-login` `login` для `logout` поставщика:</span><span class="sxs-lookup"><span data-stu-id="54e96-125">If you will be using the `mgt-login` component, you should also specify the `login` and `logout` functions for the provider:</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

