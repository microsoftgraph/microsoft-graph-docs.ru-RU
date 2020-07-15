---
title: Убрать tokenIssuancePolicy
description: Удаление Токениссуанцеполици из приложения.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64d3a74ff0397a35b1cefa7943186918ecc0c23f
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142275"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="89b55-103">Убрать tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="89b55-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="89b55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89b55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89b55-105">Удаление [токениссуанцеполици](../resources/tokenissuancepolicy.md) из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="89b55-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="89b55-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89b55-106">Permissions</span></span>

<span data-ttu-id="89b55-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="89b55-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="89b55-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89b55-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89b55-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89b55-109">Permission type</span></span>                        | <span data-ttu-id="89b55-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89b55-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89b55-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89b55-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="89b55-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="89b55-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="89b55-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89b55-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89b55-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89b55-114">Not supported.</span></span> |
| <span data-ttu-id="89b55-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="89b55-115">Application</span></span>                            | <span data-ttu-id="89b55-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="89b55-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89b55-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89b55-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="89b55-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89b55-118">Request headers</span></span>

| <span data-ttu-id="89b55-119">Имя</span><span class="sxs-lookup"><span data-stu-id="89b55-119">Name</span></span>          | <span data-ttu-id="89b55-120">Описание</span><span class="sxs-lookup"><span data-stu-id="89b55-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="89b55-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89b55-121">Authorization</span></span> | <span data-ttu-id="89b55-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="89b55-122">Bearer {token}.</span></span> <span data-ttu-id="89b55-123">Required.</span><span class="sxs-lookup"><span data-stu-id="89b55-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89b55-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89b55-124">Request body</span></span>

<span data-ttu-id="89b55-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89b55-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89b55-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="89b55-126">Response</span></span>

<span data-ttu-id="89b55-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="89b55-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="89b55-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="89b55-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89b55-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="89b55-129">Request</span></span>

<span data-ttu-id="89b55-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89b55-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="89b55-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="89b55-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="89b55-132">C#</span><span class="sxs-lookup"><span data-stu-id="89b55-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89b55-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89b55-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89b55-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89b55-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89b55-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="89b55-135">Response</span></span>

<span data-ttu-id="89b55-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89b55-136">The following is an example of the response.</span></span>

> <span data-ttu-id="89b55-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="89b55-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="89b55-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="89b55-138">All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
