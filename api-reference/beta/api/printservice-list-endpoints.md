---
title: PrintServiceEndpoints списка
description: Извлечение списка конечных точек, выставленных службой печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 09951136399d27caa65db2b22da4585014ffc3e3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961526"
---
# <a name="list-printserviceendpoints"></a><span data-ttu-id="13f1c-103">PrintServiceEndpoints списка</span><span class="sxs-lookup"><span data-stu-id="13f1c-103">List printServiceEndpoints</span></span>

<span data-ttu-id="13f1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13f1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13f1c-105">Извлечение списка конечных точек, выставленных службой печати.</span><span class="sxs-lookup"><span data-stu-id="13f1c-105">Retrieve a list of endpoints exposed by a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="13f1c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="13f1c-106">Permissions</span></span>
<span data-ttu-id="13f1c-107">Для вызова этого API не требуется никаких разрешений, но для использования службы универсальной печати клиент пользователя или клиента приложения должен иметь активную подписку универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="13f1c-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="13f1c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13f1c-108">Permission type</span></span> | <span data-ttu-id="13f1c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13f1c-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="13f1c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13f1c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="13f1c-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="13f1c-111">None.</span></span>|
|<span data-ttu-id="13f1c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13f1c-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13f1c-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="13f1c-113">None.</span></span>|
|<span data-ttu-id="13f1c-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="13f1c-114">Application</span></span>|<span data-ttu-id="13f1c-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="13f1c-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13f1c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13f1c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}/endpoints
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13f1c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="13f1c-117">Optional query parameters</span></span>
<span data-ttu-id="13f1c-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="13f1c-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="13f1c-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="13f1c-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="13f1c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13f1c-120">Request headers</span></span>
| <span data-ttu-id="13f1c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="13f1c-121">Name</span></span>      |<span data-ttu-id="13f1c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="13f1c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13f1c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13f1c-123">Authorization</span></span> | <span data-ttu-id="13f1c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13f1c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13f1c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13f1c-126">Request body</span></span>
<span data-ttu-id="13f1c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13f1c-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="13f1c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="13f1c-128">Response</span></span>
<span data-ttu-id="13f1c-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printServiceEndpoint](../resources/printserviceendpoint.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="13f1c-129">If successful, this method returns a `200 OK` response code and a collection of [printServiceEndpoint](../resources/printserviceendpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13f1c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="13f1c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13f1c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="13f1c-131">Request</span></span>
<span data-ttu-id="13f1c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13f1c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13f1c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="13f1c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="13f1c-134">C#</span><span class="sxs-lookup"><span data-stu-id="13f1c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13f1c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13f1c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13f1c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13f1c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13f1c-137">Java</span><span class="sxs-lookup"><span data-stu-id="13f1c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13f1c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="13f1c-138">Response</span></span>
<span data-ttu-id="13f1c-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13f1c-139">The following is an example of the response.</span></span>
><span data-ttu-id="13f1c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13f1c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printServiceEndpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "value": [
    {
      "id": "mpsdiscovery",
      "displayName": "Microsoft Universal Print Discovery Service",
      "uri": "https://discovery.print.microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


