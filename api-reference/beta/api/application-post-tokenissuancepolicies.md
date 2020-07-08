---
title: Назначить tokenIssuancePolicy
description: Назначьте Токениссуанцеполици приложению.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0405311f8c38afb00fc582a4f7c63a541d2f2a81
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081297"
---
# <a name="assign-tokenissuancepolicy"></a><span data-ttu-id="735b1-103">Назначить tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="735b1-103">Assign tokenIssuancePolicy</span></span>

<span data-ttu-id="735b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="735b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="735b1-105">Назначьте [токениссуанцеполици](../resources/tokenissuancepolicy.md) [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="735b1-105">Assign a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="735b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="735b1-106">Permissions</span></span>

<span data-ttu-id="735b1-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="735b1-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="735b1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="735b1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="735b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="735b1-109">Permission type</span></span>                        | <span data-ttu-id="735b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="735b1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="735b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="735b1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="735b1-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="735b1-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="735b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="735b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="735b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="735b1-114">Not supported.</span></span> |
| <span data-ttu-id="735b1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="735b1-115">Application</span></span>                            | <span data-ttu-id="735b1-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="735b1-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="735b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="735b1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenIssuancePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="735b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="735b1-118">Request headers</span></span>

| <span data-ttu-id="735b1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="735b1-119">Name</span></span>          | <span data-ttu-id="735b1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="735b1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="735b1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="735b1-121">Authorization</span></span> | <span data-ttu-id="735b1-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="735b1-122">Bearer {token}.</span></span> <span data-ttu-id="735b1-123">Required.</span><span class="sxs-lookup"><span data-stu-id="735b1-123">Required.</span></span> |
| <span data-ttu-id="735b1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="735b1-124">Content-Type</span></span> | <span data-ttu-id="735b1-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="735b1-125">application/json.</span></span> <span data-ttu-id="735b1-126">Required.</span><span class="sxs-lookup"><span data-stu-id="735b1-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="735b1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="735b1-127">Request body</span></span>

<span data-ttu-id="735b1-128">В тексте запроса укажите идентификатор объекта [токениссуанцеполици](../resources/tokenissuancepolicy.md) (с помощью `@odata.id` Свойства), который должен быть назначен приложению.</span><span class="sxs-lookup"><span data-stu-id="735b1-128">In the request body, supply the identifier of the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object (using an `@odata.id` property) that should be assigned to the application.</span></span>

## <a name="response"></a><span data-ttu-id="735b1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="735b1-129">Response</span></span>

<span data-ttu-id="735b1-130">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="735b1-130">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="735b1-131">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="735b1-131">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="735b1-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="735b1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="735b1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="735b1-133">Request</span></span>

<span data-ttu-id="735b1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="735b1-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="735b1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="735b1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenissuancepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```

### <a name="response"></a><span data-ttu-id="735b1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="735b1-136">Response</span></span>

<span data-ttu-id="735b1-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="735b1-137">The following is an example of the response.</span></span>

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
  "description": "Assign tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
