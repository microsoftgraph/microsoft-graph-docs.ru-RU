---
title: Удаление просмотретьSetQuery
description: Удаление объекта reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 01120e7702c2dc055ed0827d41b827a7330827bb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446951"
---
# <a name="delete-reviewsetquery"></a><span data-ttu-id="51fbc-103">Удаление просмотретьSetQuery</span><span class="sxs-lookup"><span data-stu-id="51fbc-103">Delete reviewSetQuery</span></span>

<span data-ttu-id="51fbc-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="51fbc-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51fbc-105">Удаление [объекта reviewSetQuery.](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="51fbc-105">Delete a [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="51fbc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51fbc-106">Permissions</span></span>

<span data-ttu-id="51fbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51fbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51fbc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51fbc-109">Permission type</span></span>|<span data-ttu-id="51fbc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51fbc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51fbc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51fbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51fbc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51fbc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="51fbc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51fbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51fbc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51fbc-114">Not supported.</span></span>|
|<span data-ttu-id="51fbc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51fbc-115">Application</span></span>|<span data-ttu-id="51fbc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51fbc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51fbc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51fbc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="51fbc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51fbc-118">Request headers</span></span>

| <span data-ttu-id="51fbc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="51fbc-119">Name</span></span>          | <span data-ttu-id="51fbc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="51fbc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="51fbc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51fbc-121">Authorization</span></span> | <span data-ttu-id="51fbc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51fbc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51fbc-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51fbc-124">Request body</span></span>

<span data-ttu-id="51fbc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51fbc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51fbc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="51fbc-126">Response</span></span>

<span data-ttu-id="51fbc-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51fbc-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51fbc-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="51fbc-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51fbc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="51fbc-130">Request</span></span>

<span data-ttu-id="51fbc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51fbc-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51fbc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="51fbc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_reviewsetquery"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```
# <a name="c"></a>[<span data-ttu-id="51fbc-133">C#</span><span class="sxs-lookup"><span data-stu-id="51fbc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51fbc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51fbc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51fbc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51fbc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51fbc-136">Java</span><span class="sxs-lookup"><span data-stu-id="51fbc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="51fbc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="51fbc-137">Response</span></span>

<span data-ttu-id="51fbc-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="51fbc-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


