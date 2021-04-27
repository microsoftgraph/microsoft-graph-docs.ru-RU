---
title: Обзор спискаSetQueries
description: Извлечение списка объектов reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 78951f97145a16bf9543162fca4cd7362f0b46f0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044594"
---
# <a name="list-reviewsetqueries"></a><span data-ttu-id="5d606-103">Обзор спискаSetQueries</span><span class="sxs-lookup"><span data-stu-id="5d606-103">List reviewSetQueries</span></span>

<span data-ttu-id="5d606-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="5d606-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d606-105">Извлечение списка объектов проверки [электронных данныхSetQuery.](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="5d606-105">Retrieve a list of eDiscovery [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d606-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d606-106">Permissions</span></span>

<span data-ttu-id="5d606-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d606-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d606-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d606-109">Permission type</span></span>|<span data-ttu-id="5d606-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d606-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d606-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d606-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5d606-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d606-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="5d606-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d606-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d606-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d606-114">Not supported.</span></span>|
|<span data-ttu-id="5d606-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d606-115">Application</span></span>|<span data-ttu-id="5d606-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d606-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d606-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d606-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d606-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5d606-118">Optional query parameters</span></span>

<span data-ttu-id="5d606-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5d606-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5d606-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5d606-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d606-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d606-121">Request headers</span></span>

| <span data-ttu-id="5d606-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5d606-122">Name</span></span>      |<span data-ttu-id="5d606-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5d606-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5d606-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d606-124">Authorization</span></span> | <span data-ttu-id="5d606-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d606-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d606-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d606-127">Request body</span></span>

<span data-ttu-id="5d606-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d606-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d606-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d606-129">Response</span></span>

<span data-ttu-id="5d606-130">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5d606-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d606-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5d606-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d606-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d606-132">Request</span></span>

<span data-ttu-id="5d606-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d606-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d606-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d606-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_reviewsetquery"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries
```
# <a name="c"></a>[<span data-ttu-id="5d606-135">C#</span><span class="sxs-lookup"><span data-stu-id="5d606-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d606-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d606-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d606-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d606-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d606-138">Java</span><span class="sxs-lookup"><span data-stu-id="5d606-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d606-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d606-139">Response</span></span>

<span data-ttu-id="5d606-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5d606-140">The following is an example of the response.</span></span>

> <span data-ttu-id="5d606-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5d606-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries",
    "@odata.nextLink": "https://graph.microsoft.com/beta/compliance/ediscovery/cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries?$skipToken=<encodedPageToken>",
    "value": [
        {
            "id": "f7859ebb-5546-4f96-937a-9cf5723e9809",
            "displayName": "Query 1",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-03-02T12:07:52.6520503Z",
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedDateTime": "2020-03-02T12:07:52.6520503Z",
            "query": "(Cc:aa)"
        },
        {
            "id": "7c4b98e1-fe18-4887-be81-79f7a24b15c8",
            "displayName": "New query1",
            "description": null,
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-03-02T16:17:19.3564678Z",
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedDateTime": "2020-03-02T16:17:19.3564678Z",
            "query": "subject:\"Quarterly Financials\""
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List queries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


