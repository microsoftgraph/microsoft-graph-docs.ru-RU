---
title: Список Ревиевсеткуериес
description: Получение списка объектов Ревиевсеткуери.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: c766aace128e03b90d0de1949b384b5b3672f6c3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970688"
---
# <a name="list-reviewsetqueries"></a><span data-ttu-id="7a504-103">Список Ревиевсеткуериес</span><span class="sxs-lookup"><span data-stu-id="7a504-103">List reviewSetQueries</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a504-104">Получение списка объектов [Ревиевсеткуери](../resources/reviewsetquery.md) обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="7a504-104">Retrieve a list of eDiscovery [reviewSetQuery](../resources/reviewsetquery.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a504-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a504-105">Permissions</span></span>

<span data-ttu-id="7a504-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a504-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a504-108">Permission type</span></span>                        | <span data-ttu-id="7a504-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a504-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7a504-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a504-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a504-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="7a504-111">User.Read</span></span> |
| <span data-ttu-id="7a504-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a504-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a504-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a504-113">Not supported.</span></span> |
| <span data-ttu-id="7a504-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a504-114">Application</span></span>                            | <span data-ttu-id="7a504-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a504-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a504-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a504-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a504-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7a504-117">Optional query parameters</span></span>

<span data-ttu-id="7a504-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7a504-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7a504-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7a504-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a504-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a504-120">Request headers</span></span>

| <span data-ttu-id="7a504-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7a504-121">Name</span></span>      |<span data-ttu-id="7a504-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7a504-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7a504-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a504-123">Authorization</span></span> | <span data-ttu-id="7a504-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a504-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a504-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a504-126">Request body</span></span>

<span data-ttu-id="7a504-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a504-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a504-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a504-128">Response</span></span>

<span data-ttu-id="7a504-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ревиевсеткуери](../resources/reviewsetquery.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7a504-129">If successful, this method returns a `200 OK` response code and a collection of [reviewSetQuery](../resources/reviewsetquery.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a504-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="7a504-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a504-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a504-131">Request</span></span>

<span data-ttu-id="7a504-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a504-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a504-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a504-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_reviewsetquery"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries
```
# <a name="c"></a>[<span data-ttu-id="7a504-134">C#</span><span class="sxs-lookup"><span data-stu-id="7a504-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a504-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a504-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a504-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a504-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a504-137">Java</span><span class="sxs-lookup"><span data-stu-id="7a504-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7a504-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a504-138">Response</span></span>

<span data-ttu-id="7a504-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7a504-139">The following is an example of the response.</span></span>

> <span data-ttu-id="7a504-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a504-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery",
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


