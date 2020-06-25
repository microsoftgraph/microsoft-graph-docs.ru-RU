---
title: Список назначенных ХомереалмдисковериполиЦиес
description: Список ХомереалмдисковериполиЦиес, назначенных субъекту службы.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 91754e1d67d9d88ff7d165638f1bc1d143580cf0
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863595"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="b3c27-103">Список назначенных Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="b3c27-103">List assigned homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="b3c27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3c27-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="b3c27-105">Перечисление объектов [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) , назначенных для [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="b3c27-105">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3c27-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3c27-106">Permissions</span></span>

<span data-ttu-id="b3c27-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b3c27-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b3c27-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3c27-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3c27-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3c27-109">Permission type</span></span>                        | <span data-ttu-id="b3c27-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3c27-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b3c27-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3c27-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3c27-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b3c27-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="b3c27-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3c27-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3c27-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3c27-114">Not supported.</span></span> |
| <span data-ttu-id="b3c27-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b3c27-115">Application</span></span>                            | <span data-ttu-id="b3c27-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b3c27-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3c27-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3c27-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="b3c27-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3c27-118">Request headers</span></span>

| <span data-ttu-id="b3c27-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b3c27-119">Name</span></span>          | <span data-ttu-id="b3c27-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b3c27-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b3c27-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3c27-121">Authorization</span></span> | <span data-ttu-id="b3c27-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b3c27-122">Bearer {token}.</span></span> <span data-ttu-id="b3c27-123">Required.</span><span class="sxs-lookup"><span data-stu-id="b3c27-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3c27-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3c27-124">Request body</span></span>

<span data-ttu-id="b3c27-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3c27-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3c27-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3c27-126">Response</span></span>

<span data-ttu-id="b3c27-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3c27-127">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3c27-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3c27-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3c27-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3c27-129">Request</span></span>

<span data-ttu-id="b3c27-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3c27-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b3c27-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3c27-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="b3c27-132">C#</span><span class="sxs-lookup"><span data-stu-id="b3c27-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-homerealmdiscoverypolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3c27-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3c27-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-homerealmdiscoverypolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3c27-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3c27-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-homerealmdiscoverypolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3c27-135">Java</span><span class="sxs-lookup"><span data-stu-id="b3c27-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-homerealmdiscoverypolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b3c27-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3c27-136">Response</span></span>

<span data-ttu-id="b3c27-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3c27-137">The following is an example of the response.</span></span>

> <span data-ttu-id="b3c27-138">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="b3c27-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b3c27-139">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b3c27-139">All the properties will be returned from an actual call.</span></span>

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
