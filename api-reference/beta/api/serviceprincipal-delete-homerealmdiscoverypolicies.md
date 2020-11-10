---
title: Удаление типа ресурса homeRealmDiscoveryPolicy
description: Удаление объекта Хомереалмдисковериполици из servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aa704fcd0bd997fe2880183ebc03bf75c3ebf0a3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969668"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="10a75-103">Удаление типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="10a75-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="10a75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10a75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10a75-105">Удаление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) из [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="10a75-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="10a75-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10a75-106">Permissions</span></span>

<span data-ttu-id="10a75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10a75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10a75-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10a75-109">Permission type</span></span>                        | <span data-ttu-id="10a75-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10a75-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="10a75-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10a75-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10a75-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="10a75-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="10a75-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10a75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10a75-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10a75-114">Not supported.</span></span> |
| <span data-ttu-id="10a75-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="10a75-115">Application</span></span>                            | <span data-ttu-id="10a75-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="10a75-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10a75-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10a75-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{servicePrincipalId}/homeRealmDiscoveryPolicies/{policyId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="10a75-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10a75-118">Request headers</span></span>

| <span data-ttu-id="10a75-119">Имя</span><span class="sxs-lookup"><span data-stu-id="10a75-119">Name</span></span>          | <span data-ttu-id="10a75-120">Описание</span><span class="sxs-lookup"><span data-stu-id="10a75-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="10a75-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10a75-121">Authorization</span></span> | <span data-ttu-id="10a75-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="10a75-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="10a75-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10a75-123">Request body</span></span>

<span data-ttu-id="10a75-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10a75-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10a75-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="10a75-125">Response</span></span>

<span data-ttu-id="10a75-126">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="10a75-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="10a75-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="10a75-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10a75-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="10a75-128">Request</span></span>

<span data-ttu-id="10a75-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10a75-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10a75-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="10a75-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/homeRealmDiscoveryPolicies/{policyId}/$ref
```
# <a name="c"></a>[<span data-ttu-id="10a75-131">C#</span><span class="sxs-lookup"><span data-stu-id="10a75-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10a75-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10a75-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10a75-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10a75-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10a75-134">Java</span><span class="sxs-lookup"><span data-stu-id="10a75-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10a75-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="10a75-135">Response</span></span>

<span data-ttu-id="10a75-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="10a75-136">The following is an example of the response.</span></span>

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


