---
title: Сообщения об ошибках API безопасности Microsoft Graph
description: Ошибки в Microsoft Graph API безопасности в Microsoft Graph возвращаются с помощью стандартных код состояния HTTP 206 Частичное контента и доставляются путем получения заголовка предупреждения.
ms.openlocfilehash: 35af0a1ed4c4bf7f6e1afb36039f812ab59f64dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028212"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="6426f-103">Сообщения об ошибках API безопасности Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6426f-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="6426f-104">Ошибки в Microsoft Graph API безопасности в Microsoft Graph возвращаются с помощью стандартных код состояния HTTP 206 Частичное контента и доставляются путем получения заголовка предупреждения.</span><span class="sxs-lookup"><span data-stu-id="6426f-104">Errors in the Microsoft Graph Security API in Microsoft Graph are returned using standard HTTP 206 Partial Content status code and are delivered by way of a warning header.</span></span>

<span data-ttu-id="6426f-105">API-Интерфейс безопасности Microsoft Graph — федеративных служба, которая получает несколько ответов от всех поставщиков данных.</span><span class="sxs-lookup"><span data-stu-id="6426f-105">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="6426f-106">При получении ошибки HTTP с API-Интерфейс безопасности Microsoft Graph возвращается предупреждение заголовка в следующем формате:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6426f-106">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="6426f-107">Этот заголовок предупреждение только отправляется обратно клиентов при один из поставщиков данных возвращает код ошибки, отличный от 2xx или 404.</span><span class="sxs-lookup"><span data-stu-id="6426f-107">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="6426f-108">Пример:</span><span class="sxs-lookup"><span data-stu-id="6426f-108">For example:</span></span>

- <span data-ttu-id="6426f-109">HttpStatusCode.Forbidden (403) может быть возвращено, если не предоставляется доступ к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="6426f-109">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="6426f-110">Если поставщик времени ожидания, HttpStatusCode.GatewayTimeout (504) возвращается в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="6426f-110">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="6426f-111">Если происходит ошибка внутреннего поставщика HttpStatusCode.InternalServerError (500) используется в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="6426f-111">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="6426f-112">Если поставщик данных возвращает 2xx или 404, он не отображается в заголовке предупреждение так как эти коды для успеха или когда данные не найдены соответственно.</span><span class="sxs-lookup"><span data-stu-id="6426f-112">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="6426f-113">В системе с федеративным 404 не найден ожидается как количество раз данные известно только один или несколько, но не для всех поставщиков.</span><span class="sxs-lookup"><span data-stu-id="6426f-113">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="6426f-114">Пример</span><span class="sxs-lookup"><span data-stu-id="6426f-114">Example</span></span>

<span data-ttu-id="6426f-115">Пользователь запрашивает `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="6426f-115">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="6426f-116">Так как 404 и 200 ожидаемых условиях, предупреждение заголовка содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6426f-116">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span> 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="6426f-117">**Примечание:** Каждого заголовка HTTP — это коллекция элементов, чтобы пользователи могли предупреждение заголовок перечислить и проверить все элементы.</span><span class="sxs-lookup"><span data-stu-id="6426f-117">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="see-also"></a><span data-ttu-id="6426f-118">См. также</span><span class="sxs-lookup"><span data-stu-id="6426f-118">See also</span></span>

<span data-ttu-id="6426f-119">Если у вас возникли неполадки с авторизацией, см в нашем [блоге](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span><span class="sxs-lookup"><span data-stu-id="6426f-119">If you’re having trouble with authorization, see our [blog post](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span></span>
