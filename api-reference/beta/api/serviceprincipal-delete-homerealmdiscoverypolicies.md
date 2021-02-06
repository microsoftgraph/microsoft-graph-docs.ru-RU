---
title: Удаление типа ресурса homeRealmDiscoveryPolicy
description: Удалите homeRealmDiscoveryPolicy из servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 65c208e572962677ea8f8e4c3d75f9f55ce51b36
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133360"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="91135-103">Удаление типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="91135-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="91135-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91135-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91135-105">Удалите [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) из [servicePrincipal.](../resources/servicePrincipal.md)</span><span class="sxs-lookup"><span data-stu-id="91135-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="91135-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91135-106">Permissions</span></span>

<span data-ttu-id="91135-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91135-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91135-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91135-109">Permission type</span></span>                        | <span data-ttu-id="91135-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91135-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="91135-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91135-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91135-112">Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91135-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="91135-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91135-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91135-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91135-114">Not supported.</span></span> |
| <span data-ttu-id="91135-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91135-115">Application</span></span>                            | <span data-ttu-id="91135-116">Policy.Read.All и Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.OwnedBy, Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91135-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91135-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91135-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{servicePrincipalId}/homeRealmDiscoveryPolicies/{policyId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="91135-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91135-118">Request headers</span></span>

| <span data-ttu-id="91135-119">Имя</span><span class="sxs-lookup"><span data-stu-id="91135-119">Name</span></span>          | <span data-ttu-id="91135-120">Описание</span><span class="sxs-lookup"><span data-stu-id="91135-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="91135-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91135-121">Authorization</span></span> | <span data-ttu-id="91135-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="91135-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="91135-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91135-123">Request body</span></span>

<span data-ttu-id="91135-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91135-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91135-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="91135-125">Response</span></span>

<span data-ttu-id="91135-126">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="91135-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="91135-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="91135-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91135-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="91135-128">Request</span></span>

<span data-ttu-id="91135-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91135-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91135-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="91135-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/homeRealmDiscoveryPolicies/{policyId}/$ref
```
# <a name="c"></a>[<span data-ttu-id="91135-131">C#</span><span class="sxs-lookup"><span data-stu-id="91135-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91135-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91135-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91135-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91135-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91135-134">Java</span><span class="sxs-lookup"><span data-stu-id="91135-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="91135-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="91135-135">Response</span></span>

<span data-ttu-id="91135-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91135-136">The following is an example of the response.</span></span>

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



