---
title: Оценка спискаStatisticsOperation
description: Получите последний объект estimateStatisticsOperation, связанный с исходным набором.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c9f1cf37baa5bb816d34290065bf74eb5419cdc8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772620"
---
# <a name="list-estimatestatisticsoperation"></a><span data-ttu-id="3c8d4-103">Оценка спискаStatisticsOperation</span><span class="sxs-lookup"><span data-stu-id="3c8d4-103">List estimateStatisticsOperation</span></span>

<span data-ttu-id="3c8d4-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3c8d4-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c8d4-105">Получите последний [объект estimateStatisticsOperation,](../resources/ediscovery-estimatestatisticsoperation.md) связанный с исходным набором.</span><span class="sxs-lookup"><span data-stu-id="3c8d4-105">Get the last [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) object associated with a source collection.</span></span> 

><span data-ttu-id="3c8d4-106">**Примечание:** В этом методе перечислены только последние операции; он не возвращает историю всех операций.</span><span class="sxs-lookup"><span data-stu-id="3c8d4-106">**Note:** This method only lists the last operation; it does not return a history of all operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c8d4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c8d4-107">Permissions</span></span>

<span data-ttu-id="3c8d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c8d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c8d4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c8d4-110">Permission type</span></span>|<span data-ttu-id="3c8d4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c8d4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c8d4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c8d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c8d4-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c8d4-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="3c8d4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c8d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c8d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c8d4-115">Not supported.</span></span>|
|<span data-ttu-id="3c8d4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c8d4-116">Application</span></span>|<span data-ttu-id="3c8d4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c8d4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c8d4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c8d4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/lastEstimateStatisticsOperation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c8d4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c8d4-119">Optional query parameters</span></span>

<span data-ttu-id="3c8d4-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3c8d4-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3c8d4-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3c8d4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c8d4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c8d4-122">Request headers</span></span>

|<span data-ttu-id="3c8d4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3c8d4-123">Name</span></span>|<span data-ttu-id="3c8d4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3c8d4-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3c8d4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c8d4-125">Authorization</span></span>|<span data-ttu-id="3c8d4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c8d4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c8d4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c8d4-128">Request body</span></span>

<span data-ttu-id="3c8d4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c8d4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c8d4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c8d4-130">Response</span></span>

<span data-ttu-id="3c8d4-131">В случае успеха этот метод возвращает код отклика и `200 OK` [объект microsoft.graph.ediscovery.estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3c8d4-131">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c8d4-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="3c8d4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c8d4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c8d4-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3c8d4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c8d4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_estimatestatisticsoperation"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/95bdbf84f02f4bdaafbbb2fe945a4962/lastEstimateStatisticsOperation
```
# <a name="c"></a>[<span data-ttu-id="3c8d4-135">C#</span><span class="sxs-lookup"><span data-stu-id="3c8d4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-estimatestatisticsoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c8d4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c8d4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-estimatestatisticsoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c8d4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c8d4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-estimatestatisticsoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c8d4-138">Java</span><span class="sxs-lookup"><span data-stu-id="3c8d4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-estimatestatisticsoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3c8d4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c8d4-139">Response</span></span>

<span data-ttu-id="3c8d4-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3c8d4-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.estimateStatisticsOperation)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "createdDateTime": "2021-01-12T20:12:01.4443402Z",
        "completedDateTime": "2021-01-12T20:12:35.4818899Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "estimateStatistics",
        "id": "95bdbf84f02f4bdaafbbb2fe945a4962",
        "indexedItemCount": 3,
        "indexedItemsSize": 68848,
        "unindexedItemCount": 0,
        "unindexedItemsSize": 0,
        "mailboxCount": 2,
        "siteCount": 0
    }
  ]
}
```
