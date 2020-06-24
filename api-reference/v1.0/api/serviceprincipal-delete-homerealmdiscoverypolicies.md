---
title: Удаление типа ресурса homeRealmDiscoveryPolicy
description: Удаление объекта Хомереалмдисковериполици из servicePrincipal.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b8c5f152f8e44f31b0016b480019fb36d132d953
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846317"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="60c0e-103">Удаление типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="60c0e-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="60c0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60c0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60c0e-105">Удаление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) из [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="60c0e-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="60c0e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60c0e-106">Permissions</span></span>

<span data-ttu-id="60c0e-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="60c0e-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="60c0e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60c0e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60c0e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60c0e-109">Permission type</span></span>                        | <span data-ttu-id="60c0e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60c0e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="60c0e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60c0e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="60c0e-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="60c0e-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="60c0e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60c0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60c0e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60c0e-114">Not supported.</span></span> |
| <span data-ttu-id="60c0e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60c0e-115">Application</span></span>                            | <span data-ttu-id="60c0e-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="60c0e-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60c0e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60c0e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="60c0e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60c0e-118">Request headers</span></span>

| <span data-ttu-id="60c0e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="60c0e-119">Name</span></span>          | <span data-ttu-id="60c0e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="60c0e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="60c0e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60c0e-121">Authorization</span></span> | <span data-ttu-id="60c0e-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="60c0e-122">Bearer {token}.</span></span> <span data-ttu-id="60c0e-123">Required.</span><span class="sxs-lookup"><span data-stu-id="60c0e-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60c0e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="60c0e-124">Request body</span></span>

<span data-ttu-id="60c0e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60c0e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60c0e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="60c0e-126">Response</span></span>

<span data-ttu-id="60c0e-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="60c0e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="60c0e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="60c0e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60c0e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="60c0e-129">Request</span></span>

<span data-ttu-id="60c0e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60c0e-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="60c0e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="60c0e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="60c0e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="60c0e-132">Response</span></span>

<span data-ttu-id="60c0e-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="60c0e-133">The following is an example of the response.</span></span>

> <span data-ttu-id="60c0e-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="60c0e-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="60c0e-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="60c0e-135">All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
