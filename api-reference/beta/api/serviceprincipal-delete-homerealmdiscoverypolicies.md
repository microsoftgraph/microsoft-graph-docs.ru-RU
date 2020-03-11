---
title: Удаление типа ресурса homeRealmDiscoveryPolicy
description: Удаление объекта Хомереалмдисковериполици из servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e167a5a913347be5514de2b2820943a3512a64c
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589015"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="a17e1-103">Удаление типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="a17e1-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="a17e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a17e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a17e1-105">Удаление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) из [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="a17e1-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a17e1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a17e1-106">Permissions</span></span>

<span data-ttu-id="a17e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a17e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a17e1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a17e1-109">Permission type</span></span>                        | <span data-ttu-id="a17e1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a17e1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a17e1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a17e1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a17e1-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a17e1-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="a17e1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a17e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a17e1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a17e1-114">Not supported.</span></span> |
| <span data-ttu-id="a17e1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a17e1-115">Application</span></span>                            | <span data-ttu-id="a17e1-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a17e1-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a17e1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a17e1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="a17e1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a17e1-118">Request headers</span></span>

| <span data-ttu-id="a17e1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a17e1-119">Name</span></span>          | <span data-ttu-id="a17e1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a17e1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a17e1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a17e1-121">Authorization</span></span> | <span data-ttu-id="a17e1-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a17e1-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a17e1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a17e1-123">Request body</span></span>

<span data-ttu-id="a17e1-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a17e1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a17e1-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="a17e1-125">Response</span></span>

<span data-ttu-id="a17e1-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a17e1-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a17e1-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="a17e1-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a17e1-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a17e1-128">Request</span></span>

<span data-ttu-id="a17e1-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a17e1-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a17e1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a17e1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="a17e1-131">C#</span><span class="sxs-lookup"><span data-stu-id="a17e1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a17e1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a17e1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a17e1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a17e1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a17e1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a17e1-134">Response</span></span>

<span data-ttu-id="a17e1-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a17e1-135">The following is an example of the response.</span></span>

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
