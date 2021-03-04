---
title: Создание reviewSetQuery
description: Используйте этот API для создания нового обзораSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 311b9d4571e9b83122d7a69d596a4856342bb941
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446936"
---
# <a name="create-reviewsetquery"></a><span data-ttu-id="71f52-103">Создание reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="71f52-103">Create reviewSetQuery</span></span>

<span data-ttu-id="71f52-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="71f52-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71f52-105">Создайте новый [объект reviewSetQuery.](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="71f52-105">Create a new [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="71f52-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71f52-106">Permissions</span></span>

<span data-ttu-id="71f52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71f52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71f52-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71f52-109">Permission type</span></span>|<span data-ttu-id="71f52-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71f52-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71f52-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71f52-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71f52-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71f52-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="71f52-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71f52-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71f52-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71f52-114">Not supported.</span></span>|
|<span data-ttu-id="71f52-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71f52-115">Application</span></span>|<span data-ttu-id="71f52-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71f52-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71f52-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71f52-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="request-headers"></a><span data-ttu-id="71f52-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71f52-118">Request headers</span></span>

| <span data-ttu-id="71f52-119">Имя</span><span class="sxs-lookup"><span data-stu-id="71f52-119">Name</span></span>          | <span data-ttu-id="71f52-120">Описание</span><span class="sxs-lookup"><span data-stu-id="71f52-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="71f52-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71f52-121">Authorization</span></span> | <span data-ttu-id="71f52-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71f52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71f52-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="71f52-124">Request body</span></span>

<span data-ttu-id="71f52-125">В теле запроса поставляем представление JSON объекта [reviewSetQuery.](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="71f52-125">In the request body, supply a JSON representation of [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span> <span data-ttu-id="71f52-126">В следующей таблице перечислены необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="71f52-126">The following table lists the required properties.</span></span>

| <span data-ttu-id="71f52-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="71f52-127">Property</span></span>     | <span data-ttu-id="71f52-128">Тип</span><span class="sxs-lookup"><span data-stu-id="71f52-128">Type</span></span>        | <span data-ttu-id="71f52-129">Описание</span><span class="sxs-lookup"><span data-stu-id="71f52-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="71f52-130">displayName</span><span class="sxs-lookup"><span data-stu-id="71f52-130">displayName</span></span>  | <span data-ttu-id="71f52-131">string</span><span class="sxs-lookup"><span data-stu-id="71f52-131">string</span></span>      | <span data-ttu-id="71f52-132">Имя запроса набора отзывов</span><span class="sxs-lookup"><span data-stu-id="71f52-132">The name of the review set query</span></span> |

## <a name="response"></a><span data-ttu-id="71f52-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="71f52-133">Response</span></span>

<span data-ttu-id="71f52-134">В случае успешного решения этот метод возвращает код отклика и новый `201 Created` [объект microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="71f52-134">If successful, this method returns a `201 Created` response code and a new [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71f52-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="71f52-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71f52-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="71f52-136">Request</span></span>

<span data-ttu-id="71f52-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71f52-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71f52-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="71f52-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reviewsetquery"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries
Content-type: application/json

{
   "displayName":"My Query 1",
   "query":"(subject:\"Quarterly Financials\")"
}
```
# <a name="c"></a>[<span data-ttu-id="71f52-139">C#</span><span class="sxs-lookup"><span data-stu-id="71f52-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71f52-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71f52-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71f52-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71f52-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71f52-142">Java</span><span class="sxs-lookup"><span data-stu-id="71f52-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="71f52-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="71f52-143">Response</span></span>

<span data-ttu-id="71f52-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71f52-144">The following is an example of the response.</span></span>

> <span data-ttu-id="71f52-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71f52-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery"
} -->

```http
HTTP/1.1 201 Created
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
    "query": "(subject:\"Quarterly Financials\")"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


