---
title: Список назначенных ХомереалмдисковериполиЦиес
description: Список ХомереалмдисковериполиЦиес, назначенных субъекту службы.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c4e200e01ff36db17bbeb51c5d42da95c32f414c
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846354"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="5bf4e-103">Список назначенных Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="5bf4e-103">List assigned homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="5bf4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bf4e-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="5bf4e-105">Перечисление объектов [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) , назначенных для [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="5bf4e-105">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5bf4e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5bf4e-106">Permissions</span></span>

<span data-ttu-id="5bf4e-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5bf4e-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5bf4e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bf4e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5bf4e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bf4e-109">Permission type</span></span>                        | <span data-ttu-id="5bf4e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bf4e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5bf4e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bf4e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5bf4e-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5bf4e-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="5bf4e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bf4e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bf4e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bf4e-114">Not supported.</span></span> |
| <span data-ttu-id="5bf4e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bf4e-115">Application</span></span>                            | <span data-ttu-id="5bf4e-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5bf4e-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bf4e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bf4e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="5bf4e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bf4e-118">Request headers</span></span>

| <span data-ttu-id="5bf4e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5bf4e-119">Name</span></span>          | <span data-ttu-id="5bf4e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5bf4e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5bf4e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bf4e-121">Authorization</span></span> | <span data-ttu-id="5bf4e-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5bf4e-122">Bearer {token}.</span></span> <span data-ttu-id="5bf4e-123">Required.</span><span class="sxs-lookup"><span data-stu-id="5bf4e-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bf4e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5bf4e-124">Request body</span></span>

<span data-ttu-id="5bf4e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bf4e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bf4e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bf4e-126">Response</span></span>

<span data-ttu-id="5bf4e-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5bf4e-127">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5bf4e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5bf4e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5bf4e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bf4e-129">Request</span></span>

<span data-ttu-id="5bf4e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bf4e-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5bf4e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bf4e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

### <a name="response"></a><span data-ttu-id="5bf4e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bf4e-132">Response</span></span>

<span data-ttu-id="5bf4e-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5bf4e-133">The following is an example of the response.</span></span>

> <span data-ttu-id="5bf4e-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="5bf4e-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5bf4e-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5bf4e-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
