---
title: Список Ревиевсеткуериес
description: Получение списка объектов Ревиевсеткуери.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 7c4a29c9e113b33bbb2efb8b3933ffb9cfb10262
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510276"
---
# <a name="list-reviewsetqueries"></a><span data-ttu-id="129f6-103">Список Ревиевсеткуериес</span><span class="sxs-lookup"><span data-stu-id="129f6-103">List reviewSetQueries</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="129f6-104">Получение списка объектов [Ревиевсеткуери](../resources/reviewsetquery.md) обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="129f6-104">Retrieve a list of eDiscovery [reviewSetQuery](../resources/reviewsetquery.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="129f6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="129f6-105">Permissions</span></span>

<span data-ttu-id="129f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="129f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="129f6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="129f6-108">Permission type</span></span>                        | <span data-ttu-id="129f6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="129f6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="129f6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="129f6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="129f6-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="129f6-111">User.Read</span></span> |
| <span data-ttu-id="129f6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="129f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="129f6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="129f6-113">Not supported.</span></span> |
| <span data-ttu-id="129f6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="129f6-114">Application</span></span>                            | <span data-ttu-id="129f6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="129f6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="129f6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="129f6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="129f6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="129f6-117">Optional query parameters</span></span>

<span data-ttu-id="129f6-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="129f6-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="129f6-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="129f6-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="129f6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="129f6-120">Request headers</span></span>

| <span data-ttu-id="129f6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="129f6-121">Name</span></span>      |<span data-ttu-id="129f6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="129f6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="129f6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="129f6-123">Authorization</span></span> | <span data-ttu-id="129f6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="129f6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="129f6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="129f6-126">Request body</span></span>

<span data-ttu-id="129f6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="129f6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="129f6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="129f6-128">Response</span></span>

<span data-ttu-id="129f6-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ревиевсеткуери](../resources/reviewsetquery.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="129f6-129">If successful, this method returns a `200 OK` response code and a collection of [reviewSetQuery](../resources/reviewsetquery.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="129f6-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="129f6-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="129f6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="129f6-131">Request</span></span>

<span data-ttu-id="129f6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="129f6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_reviewsetquery"
}-->

```http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries
```

### <a name="response"></a><span data-ttu-id="129f6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="129f6-133">Response</span></span>

<span data-ttu-id="129f6-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="129f6-134">The following is an example of the response.</span></span>

> <span data-ttu-id="129f6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="129f6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
