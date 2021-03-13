---
title: PrintServices списка
description: Извлечение списка объектов printService, которые представляют службы, доступные вашему клиенту.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 72bc0f46df6eccd5462a776f0d38aa70175ab6f0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777217"
---
# <a name="list-printservices"></a><span data-ttu-id="33522-103">PrintServices списка</span><span class="sxs-lookup"><span data-stu-id="33522-103">List printServices</span></span>
<span data-ttu-id="33522-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33522-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="33522-105">Извлечение списка **объектов printService,** которые представляют службы, доступные вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="33522-105">Retrieve a list of **printService** objects that represent the services available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="33522-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33522-106">Permissions</span></span>
<span data-ttu-id="33522-107">Для вызова **этого API** требуется одно из делегированных разрешений универсальной печати. [](/graph/permissions-reference#universal-print-permissions)</span><span class="sxs-lookup"><span data-stu-id="33522-107">One of the **delegated** Universal Print [permissions](/graph/permissions-reference#universal-print-permissions) is required to call this API.</span></span>

## <a name="http-request"></a><span data-ttu-id="33522-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33522-108">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33522-109">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="33522-109">Optional query parameters</span></span>
<span data-ttu-id="33522-110">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="33522-110">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="33522-111">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="33522-111">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="33522-112">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33522-112">Request headers</span></span>
|<span data-ttu-id="33522-113">Имя</span><span class="sxs-lookup"><span data-stu-id="33522-113">Name</span></span>|<span data-ttu-id="33522-114">Описание</span><span class="sxs-lookup"><span data-stu-id="33522-114">Description</span></span>|
|:---|:---|
|<span data-ttu-id="33522-115">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33522-115">Authorization</span></span>|<span data-ttu-id="33522-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33522-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="33522-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33522-118">Request body</span></span>
<span data-ttu-id="33522-119">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33522-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33522-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="33522-120">Response</span></span>

<span data-ttu-id="33522-121">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printService](../resources/printservice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="33522-121">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33522-122">Примеры</span><span class="sxs-lookup"><span data-stu-id="33522-122">Examples</span></span>

### <a name="request"></a><span data-ttu-id="33522-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="33522-123">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="33522-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="33522-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printservice"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services
```
# <a name="c"></a>[<span data-ttu-id="33522-125">C#</span><span class="sxs-lookup"><span data-stu-id="33522-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33522-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33522-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33522-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33522-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33522-128">Java</span><span class="sxs-lookup"><span data-stu-id="33522-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="33522-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="33522-129">Response</span></span>
<span data-ttu-id="33522-130">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="33522-130">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printService)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/services",
  "value": [
    {
      "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
      "endpoints": [
        {
          "id": "mpsdiscovery",
          "displayName": "Microsoft Universal Print Discovery Service",
          "uri": "https://discovery.print.microsoft.com"
        }
      ]
    }
  ]
}
```

