---
title: Список ежемесячныхPrintUsageByPrinter
description: Извлечение списка ежемесячных сводок использования печати, сгруппив по принтеру.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 69d8fc406f83b2ec82379767c188594fa4090ab9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959597"
---
# <a name="list-monthlyprintusagebyprinter"></a><span data-ttu-id="c980a-103">Список ежемесячныхPrintUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="c980a-103">List monthlyPrintUsageByPrinter</span></span>
<span data-ttu-id="c980a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c980a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c980a-105">Извлечение списка ежемесячных сводок использования печати, сгруппив по [принтеру.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="c980a-105">Retrieve a list of monthly print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c980a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c980a-106">Permissions</span></span>
<span data-ttu-id="c980a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c980a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c980a-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="c980a-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c980a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c980a-110">Permission type</span></span> | <span data-ttu-id="c980a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c980a-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c980a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c980a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c980a-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c980a-113">Reports.Read.All</span></span> |
|<span data-ttu-id="c980a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c980a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c980a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c980a-115">Not Supported.</span></span>|
|<span data-ttu-id="c980a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c980a-116">Application</span></span>|<span data-ttu-id="c980a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c980a-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c980a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c980a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/monthlyPrintUsageByPrinter
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c980a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c980a-119">Optional query parameters</span></span>
<span data-ttu-id="c980a-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c980a-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c980a-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c980a-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c980a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c980a-122">Request headers</span></span>
|<span data-ttu-id="c980a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c980a-123">Name</span></span>|<span data-ttu-id="c980a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c980a-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c980a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c980a-125">Authorization</span></span>|<span data-ttu-id="c980a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c980a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c980a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c980a-128">Request body</span></span>
<span data-ttu-id="c980a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c980a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c980a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c980a-130">Response</span></span>

<span data-ttu-id="c980a-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printUsageByPrinter](../resources/printusagebyprinter.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c980a-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageByPrinter](../resources/printusagebyprinter.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c980a-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="c980a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c980a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c980a-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c980a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c980a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printusagebyprinter_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/monthlyPrintUsageByPrinter
```
# <a name="c"></a>[<span data-ttu-id="c980a-135">C#</span><span class="sxs-lookup"><span data-stu-id="c980a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printusagebyprinter-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c980a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c980a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printusagebyprinter-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c980a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c980a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printusagebyprinter-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c980a-138">Java</span><span class="sxs-lookup"><span data-stu-id="c980a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printusagebyprinter-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c980a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c980a-139">Response</span></span>
<span data-ttu-id="c980a-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c980a-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printUsageByPrinter)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "usageDate": "Date",
      "completedBlackAndWhiteJobCount": 42,
      "completedColorJobCount": 0,
      "incompleteJobCount": 6
    }
  ]
}
```

