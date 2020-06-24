---
title: Удаление типа ресурса claimsMappingPolicy
description: Удаление объекта Клаимсмаппингполици из servicePrincipal.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8dbbd82aa324ccb4edbb61c613d84122213990ec
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846314"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="fb232-103">Удаление типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="fb232-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="fb232-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb232-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb232-105">Удаление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) из [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="fb232-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb232-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb232-106">Permissions</span></span>

<span data-ttu-id="fb232-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fb232-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fb232-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb232-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb232-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb232-109">Permission type</span></span>                        | <span data-ttu-id="fb232-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb232-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fb232-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb232-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb232-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fb232-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="fb232-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb232-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb232-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb232-114">Not supported.</span></span> |
| <span data-ttu-id="fb232-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb232-115">Application</span></span>                            | <span data-ttu-id="fb232-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fb232-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb232-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb232-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="fb232-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb232-118">Request headers</span></span>

| <span data-ttu-id="fb232-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fb232-119">Name</span></span>          | <span data-ttu-id="fb232-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fb232-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fb232-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb232-121">Authorization</span></span> | <span data-ttu-id="fb232-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="fb232-122">Bearer {token}.</span></span> <span data-ttu-id="fb232-123">Required.</span><span class="sxs-lookup"><span data-stu-id="fb232-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb232-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fb232-124">Request body</span></span>

<span data-ttu-id="fb232-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb232-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb232-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb232-126">Response</span></span>

<span data-ttu-id="fb232-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fb232-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fb232-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="fb232-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb232-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb232-129">Request</span></span>

<span data-ttu-id="fb232-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb232-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fb232-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb232-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="fb232-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb232-132">Response</span></span>

<span data-ttu-id="fb232-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fb232-133">The following is an example of the response.</span></span>

> <span data-ttu-id="fb232-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="fb232-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fb232-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fb232-135">All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
