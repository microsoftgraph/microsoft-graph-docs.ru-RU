---
title: Список monthlyPrintUsageSummariesByUser
description: Получить список ежемесячных сводок по использованию печати, сгруппных по пользователю.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e9ddbcb6980e90e9d66fa9f62af1b1125a9c1596
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982756"
---
# <a name="list-monthlyprintusagesummariesbyuser"></a><span data-ttu-id="4e300-103">Список monthlyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="4e300-103">List monthlyPrintUsageSummariesByUser</span></span>

<span data-ttu-id="4e300-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e300-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e300-105">Получить список ежемесячных сводок по использованию печати, сгруппных по пользователю.</span><span class="sxs-lookup"><span data-stu-id="4e300-105">Retrieve a list of monthly print usage summaries, grouped by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e300-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e300-106">Permissions</span></span>
<span data-ttu-id="4e300-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4e300-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="4e300-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="4e300-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e300-110">Permission type</span></span> | <span data-ttu-id="4e300-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e300-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4e300-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e300-112">Delegated (work or school account)</span></span>| <span data-ttu-id="4e300-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e300-113">Reports.Read.All</span></span> |
|<span data-ttu-id="4e300-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e300-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e300-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e300-115">Not Supported.</span></span>|
|<span data-ttu-id="4e300-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4e300-116">Application</span></span>|<span data-ttu-id="4e300-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e300-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e300-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e300-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/monthlyPrintUsageSummariesByUser
GET /print/reports/monthlyPrintUsageSummariesByUser
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e300-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4e300-119">Optional query parameters</span></span>
<span data-ttu-id="4e300-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4e300-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4e300-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4e300-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e300-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e300-122">Request headers</span></span>
| <span data-ttu-id="4e300-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4e300-123">Name</span></span>      |<span data-ttu-id="4e300-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4e300-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e300-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e300-125">Authorization</span></span> | <span data-ttu-id="4e300-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e300-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e300-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e300-128">Request body</span></span>
<span data-ttu-id="4e300-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e300-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4e300-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e300-130">Response</span></span>
<span data-ttu-id="4e300-131">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e300-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e300-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4e300-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e300-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e300-133">Request</span></span>
<span data-ttu-id="4e300-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e300-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e300-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e300-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/monthlyPrintUsageSummariesByUser
```
# <a name="c"></a>[<span data-ttu-id="4e300-136">C#</span><span class="sxs-lookup"><span data-stu-id="4e300-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e300-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e300-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e300-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e300-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e300-139">Java</span><span class="sxs-lookup"><span data-stu-id="4e300-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4e300-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e300-140">Response</span></span>
<span data-ttu-id="4e300-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e300-141">The following is an example of the response.</span></span>
><span data-ttu-id="4e300-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e300-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 268

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "userPrincipalName": "username@contoso.com",
      "usageDate": "2020-02-04T00:00:00.0000000Z",
      "completedBlackAndWhiteJobCount": 42,
      "completedColorJobCount": 0,
      "incompleteJobCount": 6
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List monthlyPrintUsageSummariesByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


