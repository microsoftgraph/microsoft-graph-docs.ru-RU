---
title: PrintServiceEndpoints списка
description: Извлечение списка конечных точек, выставленных службой печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8b454326bbc270f2d7c1bf65fc7e7dbed9555431
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518093"
---
# <a name="list-endpoints"></a><span data-ttu-id="255e2-103">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="255e2-103">List endpoints</span></span>
<span data-ttu-id="255e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="255e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="255e2-105">Извлечение списка конечных точек, выставленных службой печати.</span><span class="sxs-lookup"><span data-stu-id="255e2-105">Retrieve a list of endpoints exposed by a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="255e2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="255e2-106">Permissions</span></span>
<span data-ttu-id="255e2-107">Для вызова **этого API** требуется одно из делегированных разрешений универсальной печати. [](/graph/permissions-reference#universal-print-permissions)</span><span class="sxs-lookup"><span data-stu-id="255e2-107">One of the **delegated** Universal Print [permissions](/graph/permissions-reference#universal-print-permissions) is required to call this API.</span></span>

## <a name="http-request"></a><span data-ttu-id="255e2-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="255e2-108">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services/{printServiceId}/endpoints
```

## <a name="optional-query-parameters"></a><span data-ttu-id="255e2-109">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="255e2-109">Optional query parameters</span></span>
<span data-ttu-id="255e2-110">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="255e2-110">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="255e2-111">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="255e2-111">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="255e2-112">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="255e2-112">Request headers</span></span>
|<span data-ttu-id="255e2-113">Имя</span><span class="sxs-lookup"><span data-stu-id="255e2-113">Name</span></span>|<span data-ttu-id="255e2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="255e2-114">Description</span></span>|
|:---|:---|
|<span data-ttu-id="255e2-115">Авторизация</span><span class="sxs-lookup"><span data-stu-id="255e2-115">Authorization</span></span>|<span data-ttu-id="255e2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="255e2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="255e2-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="255e2-118">Request body</span></span>
<span data-ttu-id="255e2-119">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="255e2-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="255e2-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="255e2-120">Response</span></span>

<span data-ttu-id="255e2-121">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printServiceEndpoint](../resources/printserviceendpoint.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="255e2-121">If successful, this method returns a `200 OK` response code and a collection of [printServiceEndpoint](../resources/printserviceendpoint.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="255e2-122">Примеры</span><span class="sxs-lookup"><span data-stu-id="255e2-122">Examples</span></span>

### <a name="request"></a><span data-ttu-id="255e2-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="255e2-123">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printserviceendpoint"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services/{printServiceId}/endpoints
```


### <a name="response"></a><span data-ttu-id="255e2-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="255e2-124">Response</span></span>
<span data-ttu-id="255e2-125">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="255e2-125">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printServiceEndpoint)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "value": [
    {
      "id": "mpsdiscovery",
      "displayName": "Microsoft Universal Print Discovery Service",
      "uri": "https://discovery.print.microsoft.com"
    }
  ]
}
```

