---
title: Список dailyPrintUsageSummariesByPrinter
description: Извлечение списка сводок ежедневного использования печати, сгруппив по принтеру.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a7ba73373ee0c575ca32ab9a1e594089ae9cc93e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753616"
---
# <a name="list-dailyprintusagesummariesbyprinter"></a><span data-ttu-id="0d5ee-103">Список dailyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="0d5ee-103">List dailyPrintUsageSummariesByPrinter</span></span>

<span data-ttu-id="0d5ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d5ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d5ee-105">Извлечение списка сводок ежедневного использования печати, сгруппив по [принтеру.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="0d5ee-105">Retrieve a list of daily print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d5ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d5ee-106">Permissions</span></span>
<span data-ttu-id="0d5ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d5ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0d5ee-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="0d5ee-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0d5ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d5ee-110">Permission type</span></span> | <span data-ttu-id="0d5ee-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d5ee-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0d5ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d5ee-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0d5ee-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d5ee-113">Reports.Read.All</span></span> |
|<span data-ttu-id="0d5ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d5ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d5ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d5ee-115">Not Supported.</span></span>|
|<span data-ttu-id="0d5ee-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0d5ee-116">Application</span></span>|<span data-ttu-id="0d5ee-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d5ee-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d5ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d5ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter
GET /print/reports/dailyPrintUsageSummariesByPrinter
```

## <a name="request-headers"></a><span data-ttu-id="0d5ee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d5ee-119">Request headers</span></span>
| <span data-ttu-id="0d5ee-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0d5ee-120">Name</span></span>      |<span data-ttu-id="0d5ee-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0d5ee-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d5ee-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d5ee-122">Authorization</span></span> | <span data-ttu-id="0d5ee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d5ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d5ee-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d5ee-125">Request body</span></span>
<span data-ttu-id="0d5ee-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d5ee-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0d5ee-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d5ee-127">Response</span></span>
<span data-ttu-id="0d5ee-128">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0d5ee-128">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d5ee-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0d5ee-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d5ee-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d5ee-130">Request</span></span>
<span data-ttu-id="0d5ee-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d5ee-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d5ee-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d5ee-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter
```
# <a name="c"></a>[<span data-ttu-id="0d5ee-133">C#</span><span class="sxs-lookup"><span data-stu-id="0d5ee-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d5ee-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d5ee-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d5ee-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d5ee-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d5ee-136">Java</span><span class="sxs-lookup"><span data-stu-id="0d5ee-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0d5ee-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d5ee-137">Response</span></span>
<span data-ttu-id="0d5ee-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0d5ee-138">The following is an example of the response.</span></span>
><span data-ttu-id="0d5ee-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0d5ee-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 314

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
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
  "description": "List dailyPrintUsageSummariesByPrinter",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


