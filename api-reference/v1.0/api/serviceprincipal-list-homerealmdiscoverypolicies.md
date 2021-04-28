---
title: Список, присвоенный homeRealmDiscoveryPolicies
description: Список homeRealmDiscoveryPolicies, которые назначены директору службы.
localization_priority: Normal
author: hpsin
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 56c7e23c6bca817b5b35a3ec1646c479d20e972d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054443"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="a868d-103">Список, присвоенный homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="a868d-103">List assigned homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="a868d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a868d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="a868d-105">Список [объектов homeRealmDiscoveryPolicy,](../resources/homerealmdiscoverypolicy.md) которые назначены [службеPrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="a868d-105">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a868d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a868d-106">Permissions</span></span>

<span data-ttu-id="a868d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a868d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a868d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a868d-109">Permission type</span></span>                        | <span data-ttu-id="a868d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a868d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a868d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a868d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a868d-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a868d-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="a868d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a868d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a868d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a868d-114">Not supported.</span></span> |
| <span data-ttu-id="a868d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a868d-115">Application</span></span>                            | <span data-ttu-id="a868d-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a868d-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a868d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a868d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="a868d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a868d-118">Request headers</span></span>

| <span data-ttu-id="a868d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a868d-119">Name</span></span>          | <span data-ttu-id="a868d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a868d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a868d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a868d-121">Authorization</span></span> | <span data-ttu-id="a868d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a868d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a868d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a868d-124">Request body</span></span>

<span data-ttu-id="a868d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a868d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a868d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a868d-126">Response</span></span>

<span data-ttu-id="a868d-127">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a868d-127">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a868d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a868d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a868d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a868d-129">Request</span></span>

<span data-ttu-id="a868d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a868d-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a868d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a868d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="a868d-132">C#</span><span class="sxs-lookup"><span data-stu-id="a868d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-homerealmdiscoverypolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a868d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a868d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-homerealmdiscoverypolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a868d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a868d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-homerealmdiscoverypolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a868d-135">Java</span><span class="sxs-lookup"><span data-stu-id="a868d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-homerealmdiscoverypolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a868d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a868d-136">Response</span></span>

<span data-ttu-id="a868d-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a868d-137">The following is an example of the response.</span></span>

> <span data-ttu-id="a868d-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a868d-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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

