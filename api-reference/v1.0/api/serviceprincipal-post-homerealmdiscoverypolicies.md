---
title: Назначение типа ресурса homeRealmDiscoveryPolicy
description: Назначьте Хомереалмдисковериполици для servicePrincipal.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 387c8a1535ed040040475ef5c0c2e9a7d6cbb258
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846346"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="0f186-103">Назначение типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="0f186-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="0f186-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f186-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="0f186-105">Назначьте [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) для [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="0f186-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f186-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f186-106">Permissions</span></span>

<span data-ttu-id="0f186-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0f186-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0f186-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f186-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f186-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f186-109">Permission type</span></span>                        | <span data-ttu-id="0f186-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f186-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0f186-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f186-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f186-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0f186-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="0f186-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f186-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f186-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f186-114">Not supported.</span></span> |
| <span data-ttu-id="0f186-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f186-115">Application</span></span>                            | <span data-ttu-id="0f186-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0f186-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f186-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f186-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0f186-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f186-118">Request headers</span></span>

| <span data-ttu-id="0f186-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0f186-119">Name</span></span>          | <span data-ttu-id="0f186-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0f186-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0f186-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f186-121">Authorization</span></span> | <span data-ttu-id="0f186-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0f186-122">Bearer {token}.</span></span> <span data-ttu-id="0f186-123">Required.</span><span class="sxs-lookup"><span data-stu-id="0f186-123">Required.</span></span> |
| <span data-ttu-id="0f186-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f186-124">Content-Type</span></span> | <span data-ttu-id="0f186-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="0f186-125">application/json.</span></span> <span data-ttu-id="0f186-126">Required.</span><span class="sxs-lookup"><span data-stu-id="0f186-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f186-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f186-127">Request body</span></span>

<span data-ttu-id="0f186-128">В тексте запроса укажите идентификатор объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) (с помощью `@odata.id` Свойства), который должен быть назначен субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="0f186-128">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="0f186-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f186-129">Response</span></span>

<span data-ttu-id="0f186-130">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="0f186-130">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="0f186-131">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="0f186-131">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0f186-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="0f186-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f186-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f186-133">Request</span></span>

<span data-ttu-id="0f186-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f186-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0f186-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f186-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_servicePrincipal"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```

### <a name="response"></a><span data-ttu-id="0f186-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f186-136">Response</span></span>

<span data-ttu-id="0f186-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0f186-137">The following is an example of the response.</span></span>

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
  "description": "Assign homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
