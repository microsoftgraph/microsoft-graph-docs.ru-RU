---
title: Получение Ревиевсеткуери
description: Получение свойств и связей объекта ревиевсеткуери обнаружения электронных данных.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: ea7ce88da2a48f4180f278c82616c00d64e8f875
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085404"
---
# <a name="get-reviewsetquery"></a><span data-ttu-id="f9ca0-103">Получение Ревиевсеткуери</span><span class="sxs-lookup"><span data-stu-id="f9ca0-103">Get reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9ca0-104">Получение свойств и связей объекта [Ревиевсеткуери](../resources/reviewsetquery.md) обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="f9ca0-104">Retrieve the properties and relationships of an eDiscovery [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9ca0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9ca0-105">Permissions</span></span>

<span data-ttu-id="f9ca0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9ca0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9ca0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9ca0-108">Permission type</span></span>                        | <span data-ttu-id="f9ca0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9ca0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f9ca0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9ca0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9ca0-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="f9ca0-111">User.Read</span></span> |
| <span data-ttu-id="f9ca0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9ca0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9ca0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ca0-113">Not supported.</span></span> |
| <span data-ttu-id="f9ca0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9ca0-114">Application</span></span>                            | <span data-ttu-id="f9ca0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ca0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9ca0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9ca0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9ca0-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9ca0-117">Optional query parameters</span></span>

<span data-ttu-id="f9ca0-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f9ca0-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f9ca0-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f9ca0-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9ca0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9ca0-120">Request headers</span></span>

| <span data-ttu-id="f9ca0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f9ca0-121">Name</span></span>      |<span data-ttu-id="f9ca0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f9ca0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9ca0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9ca0-123">Authorization</span></span> | <span data-ttu-id="f9ca0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9ca0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9ca0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9ca0-126">Request body</span></span>

<span data-ttu-id="f9ca0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9ca0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9ca0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9ca0-128">Response</span></span>

<span data-ttu-id="f9ca0-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [ревиевсеткуери](../resources/reviewsetquery.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9ca0-129">If successful, this method returns a `200 OK` response code and the requested [reviewSetQuery](../resources/reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9ca0-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f9ca0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9ca0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9ca0-131">Request</span></span>

<span data-ttu-id="f9ca0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9ca0-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9ca0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9ca0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reviewsetquery"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```
# <a name="c"></a>[<span data-ttu-id="f9ca0-134">C#</span><span class="sxs-lookup"><span data-stu-id="f9ca0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9ca0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9ca0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9ca0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9ca0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f9ca0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9ca0-137">Response</span></span>

<span data-ttu-id="f9ca0-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f9ca0-138">The following is an example of the response.</span></span>

> <span data-ttu-id="f9ca0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9ca0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries/$entity",
    "id": "6b5358b0-2ce2-4369-b9cf-65392fe56807",
    "displayName": "My Query 1",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-09T09:05:12.3756813Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-03-09T09:05:12.3756813Z",
    "query": "subject:\"Quarterly Financials\""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


