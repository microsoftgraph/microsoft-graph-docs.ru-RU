---
title: PrintServices списка
description: Извлечение списка объектов printService, которые представляют службы, доступные вашему клиенту.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c5226eadd4edfd3e8d2d15534eed3fcb5ffc9619
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517518"
---
# <a name="list-printservices"></a><span data-ttu-id="e9aa9-103">PrintServices списка</span><span class="sxs-lookup"><span data-stu-id="e9aa9-103">List printServices</span></span>
<span data-ttu-id="e9aa9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9aa9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="e9aa9-105">Извлечение списка **объектов printService,** которые представляют службы, доступные вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="e9aa9-105">Retrieve a list of **printService** objects that represent the services available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9aa9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9aa9-106">Permissions</span></span>
<span data-ttu-id="e9aa9-107">Для вызова **этого API** требуется одно из делегированных разрешений универсальной печати. [](/graph/permissions-reference#universal-print-permissions)</span><span class="sxs-lookup"><span data-stu-id="e9aa9-107">One of the **delegated** Universal Print [permissions](/graph/permissions-reference#universal-print-permissions) is required to call this API.</span></span>

## <a name="http-request"></a><span data-ttu-id="e9aa9-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9aa9-108">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9aa9-109">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e9aa9-109">Optional query parameters</span></span>
<span data-ttu-id="e9aa9-110">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e9aa9-110">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e9aa9-111">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e9aa9-111">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9aa9-112">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9aa9-112">Request headers</span></span>
|<span data-ttu-id="e9aa9-113">Имя</span><span class="sxs-lookup"><span data-stu-id="e9aa9-113">Name</span></span>|<span data-ttu-id="e9aa9-114">Описание</span><span class="sxs-lookup"><span data-stu-id="e9aa9-114">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e9aa9-115">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9aa9-115">Authorization</span></span>|<span data-ttu-id="e9aa9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9aa9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9aa9-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9aa9-118">Request body</span></span>
<span data-ttu-id="e9aa9-119">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9aa9-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9aa9-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9aa9-120">Response</span></span>

<span data-ttu-id="e9aa9-121">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printService](../resources/printservice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e9aa9-121">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9aa9-122">Примеры</span><span class="sxs-lookup"><span data-stu-id="e9aa9-122">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9aa9-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9aa9-123">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printservice"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services
```


### <a name="response"></a><span data-ttu-id="e9aa9-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9aa9-124">Response</span></span>
<span data-ttu-id="e9aa9-125">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e9aa9-125">**Note:** The response object shown here might be shortened for readability.</span></span>
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

