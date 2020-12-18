---
title: Создание reviewSetQuery
description: Используйте этот API для создания нового reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 2635c446c6e0332df780c71be61232bb364ad683
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714104"
---
# <a name="create-reviewsetquery"></a><span data-ttu-id="a6df5-103">Создание reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="a6df5-103">Create reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6df5-104">Создание объекта [reviewSetQuery.](../resources/reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="a6df5-104">Create a new [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6df5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6df5-105">Permissions</span></span>

<span data-ttu-id="a6df5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6df5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6df5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6df5-108">Permission type</span></span>                        | <span data-ttu-id="a6df5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6df5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a6df5-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6df5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6df5-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="a6df5-111">User.Read</span></span> |
| <span data-ttu-id="a6df5-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6df5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6df5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6df5-113">Not supported.</span></span> |
| <span data-ttu-id="a6df5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6df5-114">Application</span></span>                            | <span data-ttu-id="a6df5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6df5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6df5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6df5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="request-headers"></a><span data-ttu-id="a6df5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6df5-117">Request headers</span></span>

| <span data-ttu-id="a6df5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a6df5-118">Name</span></span>          | <span data-ttu-id="a6df5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a6df5-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a6df5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6df5-120">Authorization</span></span> | <span data-ttu-id="a6df5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6df5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6df5-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6df5-123">Request body</span></span>

<span data-ttu-id="a6df5-124">В теле запроса укажу представление объекта [reviewSetQuery](../resources/reviewsetquery.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="a6df5-124">In the request body, supply a JSON representation of [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span> <span data-ttu-id="a6df5-125">В следующей таблице перечислены необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="a6df5-125">The following table lists the required properties.</span></span>

| <span data-ttu-id="a6df5-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6df5-126">Property</span></span>     | <span data-ttu-id="a6df5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a6df5-127">Type</span></span>        | <span data-ttu-id="a6df5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a6df5-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a6df5-129">displayName</span><span class="sxs-lookup"><span data-stu-id="a6df5-129">displayName</span></span>  | <span data-ttu-id="a6df5-130">string</span><span class="sxs-lookup"><span data-stu-id="a6df5-130">string</span></span>      | <span data-ttu-id="a6df5-131">Имя запроса набора для проверки</span><span class="sxs-lookup"><span data-stu-id="a6df5-131">The name of the review set query</span></span> |

## <a name="response"></a><span data-ttu-id="a6df5-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6df5-132">Response</span></span>

<span data-ttu-id="a6df5-133">В случае успеха этот метод возвращает код отклика и новый объект `201 Created` [reviewSetQuery](../resources/reviewsetquery.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6df5-133">If successful, this method returns a `201 Created` response code and a new [reviewSetQuery](../resources/reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6df5-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="a6df5-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6df5-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6df5-135">Request</span></span>

<span data-ttu-id="a6df5-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6df5-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6df5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6df5-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a6df5-138">C#</span><span class="sxs-lookup"><span data-stu-id="a6df5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6df5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6df5-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6df5-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6df5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6df5-141">Java</span><span class="sxs-lookup"><span data-stu-id="a6df5-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a6df5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6df5-142">Response</span></span>

<span data-ttu-id="a6df5-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a6df5-143">The following is an example of the response.</span></span>

> <span data-ttu-id="a6df5-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6df5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery"
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


