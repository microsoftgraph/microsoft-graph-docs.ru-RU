---
title: Получение printUsageSummaryByPrinter
description: Извлечение сводки использования принтера за определенный период времени.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
ms.date: 2/4/2020
doc_type: apiPageType
ms.openlocfilehash: bc7e8a88600a19494312e7fc2db7aebb455e8a2a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753619"
---
# <a name="get-printusagesummarybyprinter"></a><span data-ttu-id="e27d1-103">Получение printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="e27d1-103">Get printUsageSummaryByPrinter</span></span>

<span data-ttu-id="e27d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e27d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e27d1-105">[Извлечение сводки](../resources/printer.md)использования принтера за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="e27d1-105">Retrieve a [printer](../resources/printer.md)'s usage summary for a particular time period.</span></span> <span data-ttu-id="e27d1-106">Описание каждой из конечных точек см. в [printUsageSummaryByPrinter.](../resources/printUsageSummaryByPrinter.md)</span><span class="sxs-lookup"><span data-stu-id="e27d1-106">For descriptions of each of the endpoints, see [printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e27d1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e27d1-107">Permissions</span></span>
<span data-ttu-id="e27d1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e27d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e27d1-110">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e27d1-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="e27d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e27d1-111">Permission type</span></span> | <span data-ttu-id="e27d1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e27d1-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e27d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e27d1-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e27d1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e27d1-114">Reports.Read.All</span></span> |
|<span data-ttu-id="e27d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e27d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e27d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e27d1-116">Not Supported.</span></span>|
|<span data-ttu-id="e27d1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e27d1-117">Application</span></span>|<span data-ttu-id="e27d1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e27d1-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e27d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e27d1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter/{id}
GET /reports/monthlyPrintUsageSummariesByPrinter/{id}
GET /print/reports/dailyPrintUsageSummariesByPrinter/{id}
GET /print/reports/monthlyPrintUsageSummariesByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e27d1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e27d1-120">Optional query parameters</span></span>
<span data-ttu-id="e27d1-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e27d1-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e27d1-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e27d1-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e27d1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e27d1-123">Request headers</span></span>
| <span data-ttu-id="e27d1-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e27d1-124">Name</span></span>      |<span data-ttu-id="e27d1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e27d1-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e27d1-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e27d1-126">Authorization</span></span> | <span data-ttu-id="e27d1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e27d1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e27d1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e27d1-129">Request body</span></span>
<span data-ttu-id="e27d1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e27d1-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e27d1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e27d1-131">Response</span></span>
<span data-ttu-id="e27d1-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e27d1-132">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e27d1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e27d1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e27d1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e27d1-134">Request</span></span>
<span data-ttu-id="e27d1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e27d1-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e27d1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e27d1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByPrinter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter/{id}
```
# <a name="c"></a>[<span data-ttu-id="e27d1-137">C#</span><span class="sxs-lookup"><span data-stu-id="e27d1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagesummarybyprinter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e27d1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e27d1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagesummarybyprinter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e27d1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e27d1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagesummarybyprinter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e27d1-140">Java</span><span class="sxs-lookup"><span data-stu-id="e27d1-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagesummarybyprinter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e27d1-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e27d1-141">Response</span></span>
<span data-ttu-id="e27d1-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e27d1-142">The following is an example of the response.</span></span>
><span data-ttu-id="e27d1-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e27d1-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
    "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "usageDate": "2020-02-04T00:00:00.0000000Z",
    "completedBlackAndWhiteJobCount": 42,
    "completedColorJobCount": 0,
    "incompleteJobCount": 6
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printUsageSummaryByPrinter",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

