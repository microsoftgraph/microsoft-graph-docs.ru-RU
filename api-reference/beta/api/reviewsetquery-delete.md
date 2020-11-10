---
title: Удаление Ревиевсеткуери
description: Удаление объекта Ревиевсеткуери.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: a9f62226f721d9e0ba03742a8ea72c78ed3e9e33
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981237"
---
# <a name="delete-reviewsetquery"></a><span data-ttu-id="7e85e-103">Удаление Ревиевсеткуери</span><span class="sxs-lookup"><span data-stu-id="7e85e-103">Delete reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e85e-104">Удаление объекта [ревиевсеткуери](../resources/reviewsetquery.md) .</span><span class="sxs-lookup"><span data-stu-id="7e85e-104">Delete a [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e85e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e85e-105">Permissions</span></span>

<span data-ttu-id="7e85e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e85e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e85e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e85e-108">Permission type</span></span>                        | <span data-ttu-id="7e85e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e85e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7e85e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e85e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e85e-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="7e85e-111">User.Read</span></span> |
| <span data-ttu-id="7e85e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e85e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e85e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e85e-113">Not supported.</span></span> |
| <span data-ttu-id="7e85e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e85e-114">Application</span></span>                            | <span data-ttu-id="7e85e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e85e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e85e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e85e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7e85e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e85e-117">Request headers</span></span>

| <span data-ttu-id="7e85e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7e85e-118">Name</span></span>          | <span data-ttu-id="7e85e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7e85e-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7e85e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e85e-120">Authorization</span></span> | <span data-ttu-id="7e85e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e85e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e85e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e85e-123">Request body</span></span>

<span data-ttu-id="7e85e-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e85e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e85e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e85e-125">Response</span></span>

<span data-ttu-id="7e85e-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e85e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e85e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7e85e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7e85e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e85e-129">Request</span></span>

<span data-ttu-id="7e85e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e85e-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e85e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e85e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_reviewsetquery"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```
# <a name="c"></a>[<span data-ttu-id="7e85e-132">C#</span><span class="sxs-lookup"><span data-stu-id="7e85e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e85e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e85e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e85e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e85e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e85e-135">Java</span><span class="sxs-lookup"><span data-stu-id="7e85e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7e85e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e85e-136">Response</span></span>

<span data-ttu-id="7e85e-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7e85e-137">The following is an example of the response.</span></span>

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


