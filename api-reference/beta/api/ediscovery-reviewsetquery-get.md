---
title: Получить обзорSetQuery
description: Извлечение свойств и связей объекта проверки проверки электронной почты.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3ddc2c3e3c7231d0bdf8ec81a12e49b4c016a83a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446945"
---
# <a name="get-reviewsetquery"></a><span data-ttu-id="26347-103">Получить обзорSetQuery</span><span class="sxs-lookup"><span data-stu-id="26347-103">Get reviewSetQuery</span></span>

<span data-ttu-id="26347-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="26347-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26347-105">Извлечение свойств и связей объекта eDiscovery [reviewSetQuery.](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="26347-105">Retrieve the properties and relationships of an eDiscovery [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26347-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26347-106">Permissions</span></span>

<span data-ttu-id="26347-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26347-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26347-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26347-109">Permission type</span></span>|<span data-ttu-id="26347-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26347-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26347-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26347-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26347-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26347-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="26347-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26347-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26347-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26347-114">Not supported.</span></span>|
|<span data-ttu-id="26347-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26347-115">Application</span></span>|<span data-ttu-id="26347-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26347-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26347-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26347-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26347-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="26347-118">Optional query parameters</span></span>

<span data-ttu-id="26347-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="26347-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="26347-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="26347-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="26347-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26347-121">Request headers</span></span>

| <span data-ttu-id="26347-122">Имя</span><span class="sxs-lookup"><span data-stu-id="26347-122">Name</span></span>      |<span data-ttu-id="26347-123">Описание</span><span class="sxs-lookup"><span data-stu-id="26347-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="26347-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26347-124">Authorization</span></span> | <span data-ttu-id="26347-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26347-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26347-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26347-127">Request body</span></span>

<span data-ttu-id="26347-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26347-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26347-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="26347-129">Response</span></span>

<span data-ttu-id="26347-130">В случае успешного решения этот метод возвращает код ответа и запрашиваемого `200 OK` [объекта microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="26347-130">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26347-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="26347-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26347-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="26347-132">Request</span></span>

<span data-ttu-id="26347-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26347-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26347-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="26347-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reviewsetquery"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```
# <a name="c"></a>[<span data-ttu-id="26347-135">C#</span><span class="sxs-lookup"><span data-stu-id="26347-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26347-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26347-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26347-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26347-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26347-138">Java</span><span class="sxs-lookup"><span data-stu-id="26347-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26347-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="26347-139">Response</span></span>

<span data-ttu-id="26347-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26347-140">The following is an example of the response.</span></span>

> <span data-ttu-id="26347-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26347-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery"
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


