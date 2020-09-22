---
title: Список dailyPrintUsageSummariesByUser
description: Получение списка сводных сведений об использовании печати с ежедневной группировкой по пользователям.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: fa12b040ca775391dd4081eac99d1cf3d7cfd4d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017297"
---
# <a name="list-dailyprintusagesummariesbyuser"></a><span data-ttu-id="809df-103">Список dailyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="809df-103">List dailyPrintUsageSummariesByUser</span></span>

<span data-ttu-id="809df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="809df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="809df-105">Получение списка сводных сведений об использовании печати с ежедневной группировкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="809df-105">Retrieve a list of daily print usage summaries, grouped by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="809df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="809df-106">Permissions</span></span>
<span data-ttu-id="809df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="809df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="809df-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="809df-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="809df-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="809df-110">Permission type</span></span> | <span data-ttu-id="809df-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="809df-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="809df-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="809df-112">Delegated (work or school account)</span></span>| <span data-ttu-id="809df-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="809df-113">Users.Read.All</span></span> |
|<span data-ttu-id="809df-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="809df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="809df-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="809df-115">Not Supported.</span></span>|
|<span data-ttu-id="809df-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="809df-116">Application</span></span>|<span data-ttu-id="809df-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="809df-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="809df-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="809df-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByUser
GET /print/reports/dailyPrintUsageSummariesByUser
```

## <a name="optional-query-parameters"></a><span data-ttu-id="809df-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="809df-119">Optional query parameters</span></span>
<span data-ttu-id="809df-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="809df-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="809df-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="809df-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="809df-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="809df-122">Request headers</span></span>
| <span data-ttu-id="809df-123">Имя</span><span class="sxs-lookup"><span data-stu-id="809df-123">Name</span></span>      |<span data-ttu-id="809df-124">Описание</span><span class="sxs-lookup"><span data-stu-id="809df-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="809df-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="809df-125">Authorization</span></span> | <span data-ttu-id="809df-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="809df-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="809df-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="809df-128">Request body</span></span>
<span data-ttu-id="809df-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="809df-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="809df-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="809df-130">Response</span></span>
<span data-ttu-id="809df-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтусажесуммарибюсер](../resources/printusagesummarybyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="809df-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="809df-132">Пример</span><span class="sxs-lookup"><span data-stu-id="809df-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="809df-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="809df-133">Request</span></span>
<span data-ttu-id="809df-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="809df-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="809df-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="809df-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByUser
```
# <a name="c"></a>[<span data-ttu-id="809df-136">C#</span><span class="sxs-lookup"><span data-stu-id="809df-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="809df-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="809df-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="809df-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="809df-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="809df-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="809df-139">Response</span></span>
<span data-ttu-id="809df-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="809df-140">The following is an example of the response.</span></span>
><span data-ttu-id="809df-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="809df-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "userPrincipalName": "username@microsoft.com",
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
  "description": "List dailyPrintUsageSummariesByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


