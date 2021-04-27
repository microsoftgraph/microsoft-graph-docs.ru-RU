---
title: Список присвоенных утвержденийMappingPolicies
description: Список утвержденийMappingPolicies, которые назначены службеPrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: d049d822bd7f3bac7e306724684672670917457e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051895"
---
# <a name="list-assigned-claimsmappingpolicy"></a><span data-ttu-id="f480a-103">Список присвоенных утвержденийMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="f480a-103">List assigned claimsMappingPolicy</span></span>

<span data-ttu-id="f480a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f480a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f480a-105">Список [объектов claimsMappingPolicy,](../resources/claimsmappingpolicy.md) которые назначены [службеPrincipal.](../resources/servicePrincipal.md)</span><span class="sxs-lookup"><span data-stu-id="f480a-105">List the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f480a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f480a-106">Permissions</span></span>

<span data-ttu-id="f480a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f480a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f480a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f480a-109">Permission type</span></span>                        | <span data-ttu-id="f480a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f480a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f480a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f480a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f480a-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f480a-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="f480a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f480a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f480a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f480a-114">Not supported.</span></span> |
| <span data-ttu-id="f480a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f480a-115">Application</span></span>                            | <span data-ttu-id="f480a-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f480a-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f480a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f480a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f480a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f480a-118">Request headers</span></span>

| <span data-ttu-id="f480a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f480a-119">Name</span></span>          | <span data-ttu-id="f480a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f480a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f480a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f480a-121">Authorization</span></span> | <span data-ttu-id="f480a-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f480a-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f480a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f480a-123">Request body</span></span>

<span data-ttu-id="f480a-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f480a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f480a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="f480a-125">Response</span></span>

<span data-ttu-id="f480a-126">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [claimsMappingPolicy](../resources/claimsMappingPolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f480a-126">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsMappingPolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f480a-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="f480a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f480a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="f480a-128">Request</span></span>

<span data-ttu-id="f480a-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f480a-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f480a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f480a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_claimsmappingpolicies_on_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="f480a-131">C#</span><span class="sxs-lookup"><span data-stu-id="f480a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-claimsmappingpolicies-on-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f480a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f480a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-claimsmappingpolicies-on-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f480a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f480a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-claimsmappingpolicies-on-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f480a-134">Java</span><span class="sxs-lookup"><span data-stu-id="f480a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-claimsmappingpolicies-on-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f480a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f480a-135">Response</span></span>

<span data-ttu-id="f480a-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f480a-136">The following is an example of the response.</span></span>

> <span data-ttu-id="f480a-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f480a-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
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
  "description": "List assigned claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



