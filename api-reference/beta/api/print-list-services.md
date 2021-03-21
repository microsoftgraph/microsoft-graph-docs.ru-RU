---
title: PrintServices списка
description: Извлечение списка объектов printService, которые представляют службы, доступные вашему клиенту.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d32cd0467db0106ef8d923275b7624ec4bd0dead
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962292"
---
# <a name="list-printservices"></a><span data-ttu-id="dfdfd-103">PrintServices списка</span><span class="sxs-lookup"><span data-stu-id="dfdfd-103">List printServices</span></span>

<span data-ttu-id="dfdfd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfdfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfdfd-105">Извлечение списка [объектов printService,](../resources/printservice.md) которые представляют **службы,** доступные вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-105">Retrieve a list of [printService](../resources/printservice.md) objects that represent the **services** available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfdfd-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="dfdfd-106">Permissions</span></span>
<span data-ttu-id="dfdfd-107">Для вызова этого API не требуется никаких разрешений, но для использования службы универсальной печати клиент пользователя или клиента приложения должен иметь активную подписку универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="dfdfd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfdfd-108">Permission type</span></span> | <span data-ttu-id="dfdfd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfdfd-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="dfdfd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfdfd-110">Delegated (work or school account)</span></span>|<span data-ttu-id="dfdfd-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-111">None.</span></span>|
|<span data-ttu-id="dfdfd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfdfd-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfdfd-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-113">None.</span></span>|
|<span data-ttu-id="dfdfd-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="dfdfd-114">Application</span></span>|<span data-ttu-id="dfdfd-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfdfd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfdfd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfdfd-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dfdfd-117">Optional query parameters</span></span>
<span data-ttu-id="dfdfd-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="dfdfd-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dfdfd-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfdfd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfdfd-120">Request headers</span></span>
| <span data-ttu-id="dfdfd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dfdfd-121">Name</span></span>      |<span data-ttu-id="dfdfd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dfdfd-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dfdfd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfdfd-123">Authorization</span></span> | <span data-ttu-id="dfdfd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfdfd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfdfd-126">Request body</span></span>
<span data-ttu-id="dfdfd-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dfdfd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfdfd-128">Response</span></span>
<span data-ttu-id="dfdfd-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printService](../resources/printservice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-129">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dfdfd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dfdfd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfdfd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfdfd-131">Request</span></span>
<span data-ttu-id="dfdfd-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dfdfd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfdfd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services
```
# <a name="c"></a>[<span data-ttu-id="dfdfd-134">C#</span><span class="sxs-lookup"><span data-stu-id="dfdfd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfdfd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfdfd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfdfd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfdfd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfdfd-137">Java</span><span class="sxs-lookup"><span data-stu-id="dfdfd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-services-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dfdfd-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfdfd-138">Response</span></span>
<span data-ttu-id="dfdfd-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-139">The following is an example of the response.</span></span>
><span data-ttu-id="dfdfd-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfdfd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/services",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


