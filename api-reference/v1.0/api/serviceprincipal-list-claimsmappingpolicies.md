---
title: Список присвоенных утвержденийMappingPolicies
description: Список утвержденийMappingPolicies, которые назначены директору службы.
localization_priority: Normal
author: paulgarn
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 0f6c5d3b0b9217bef4394f9595a72980a973173e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034908"
---
# <a name="list-assigned-claimsmappingpolicy"></a><span data-ttu-id="5d2f8-103">Список присвоенных утвержденийMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="5d2f8-103">List assigned claimsMappingPolicy</span></span>

<span data-ttu-id="5d2f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d2f8-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="5d2f8-105">Список [объектов claimsMappingPolicy,](../resources/claimsmappingpolicy.md) которые назначены [службеPrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="5d2f8-105">List the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects that are assigned to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d2f8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d2f8-106">Permissions</span></span>

<span data-ttu-id="5d2f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d2f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d2f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d2f8-109">Permission type</span></span>                        | <span data-ttu-id="5d2f8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d2f8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5d2f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d2f8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d2f8-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d2f8-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="5d2f8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d2f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d2f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d2f8-114">Not supported.</span></span> |
| <span data-ttu-id="5d2f8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d2f8-115">Application</span></span>                            | <span data-ttu-id="5d2f8-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d2f8-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d2f8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d2f8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="5d2f8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d2f8-118">Request headers</span></span>

| <span data-ttu-id="5d2f8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5d2f8-119">Name</span></span>          | <span data-ttu-id="5d2f8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5d2f8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5d2f8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d2f8-121">Authorization</span></span> | <span data-ttu-id="5d2f8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d2f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d2f8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d2f8-124">Request body</span></span>

<span data-ttu-id="5d2f8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d2f8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d2f8-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d2f8-126">Response</span></span>

<span data-ttu-id="5d2f8-127">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [claimsMappingPolicy](../resources/claimsmappingpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5d2f8-127">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d2f8-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5d2f8-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d2f8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d2f8-129">Request</span></span>

<span data-ttu-id="5d2f8-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d2f8-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5d2f8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d2f8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_claimsmappingpolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="5d2f8-132">C#</span><span class="sxs-lookup"><span data-stu-id="5d2f8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-claimsmappingpolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d2f8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d2f8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-claimsmappingpolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d2f8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d2f8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-claimsmappingpolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d2f8-135">Java</span><span class="sxs-lookup"><span data-stu-id="5d2f8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-claimsmappingpolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d2f8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d2f8-136">Response</span></span>

<span data-ttu-id="5d2f8-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5d2f8-137">The following is an example of the response.</span></span>

> <span data-ttu-id="5d2f8-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5d2f8-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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

