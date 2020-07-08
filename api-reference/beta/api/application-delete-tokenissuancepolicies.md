---
title: Убрать tokenIssuancePolicy
description: Удаление Токениссуанцеполици из приложения.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e5f795000414ebecfbb002b96feb490207b44a94
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081305"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="13e30-103">Убрать tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="13e30-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="13e30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13e30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13e30-105">Удаление [токениссуанцеполици](../resources/tokenissuancepolicy.md) из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="13e30-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="13e30-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13e30-106">Permissions</span></span>

<span data-ttu-id="13e30-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="13e30-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="13e30-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13e30-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13e30-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13e30-109">Permission type</span></span>                        | <span data-ttu-id="13e30-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13e30-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="13e30-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13e30-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="13e30-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="13e30-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="13e30-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13e30-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13e30-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13e30-114">Not supported.</span></span> |
| <span data-ttu-id="13e30-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="13e30-115">Application</span></span>                            | <span data-ttu-id="13e30-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="13e30-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13e30-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13e30-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="13e30-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13e30-118">Request headers</span></span>

| <span data-ttu-id="13e30-119">Имя</span><span class="sxs-lookup"><span data-stu-id="13e30-119">Name</span></span>          | <span data-ttu-id="13e30-120">Описание</span><span class="sxs-lookup"><span data-stu-id="13e30-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="13e30-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13e30-121">Authorization</span></span> | <span data-ttu-id="13e30-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="13e30-122">Bearer {token}.</span></span> <span data-ttu-id="13e30-123">Required.</span><span class="sxs-lookup"><span data-stu-id="13e30-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13e30-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="13e30-124">Request body</span></span>

<span data-ttu-id="13e30-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13e30-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13e30-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="13e30-126">Response</span></span>

<span data-ttu-id="13e30-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="13e30-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="13e30-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="13e30-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13e30-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="13e30-129">Request</span></span>

<span data-ttu-id="13e30-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13e30-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="13e30-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="13e30-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="13e30-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="13e30-132">Response</span></span>

<span data-ttu-id="13e30-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13e30-133">The following is an example of the response.</span></span>

> <span data-ttu-id="13e30-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="13e30-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="13e30-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="13e30-135">All the properties will be returned from an actual call.</span></span>

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
