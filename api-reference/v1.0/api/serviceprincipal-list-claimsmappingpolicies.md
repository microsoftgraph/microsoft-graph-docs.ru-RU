---
title: Список присвоенных claimsMappingPolicies
description: Список claimsMappingPolicies, которые назначены для основного службы.
localization_priority: Normal
author: paulgarn
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8282d90d6df5c44432a203c46438317bd9f15515
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132240"
---
# <a name="list-assigned-claimsmappingpolicy"></a><span data-ttu-id="e68d5-103">Список присвоенных утвержденийMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="e68d5-103">List assigned claimsMappingPolicy</span></span>

<span data-ttu-id="e68d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e68d5-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="e68d5-105">Список объектов [claimsMappingPolicy,](../resources/claimsmappingpolicy.md) которые назначены [servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="e68d5-105">List the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects that are assigned to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e68d5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e68d5-106">Permissions</span></span>

<span data-ttu-id="e68d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e68d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e68d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e68d5-109">Permission type</span></span>                        | <span data-ttu-id="e68d5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e68d5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e68d5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e68d5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e68d5-112">Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e68d5-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="e68d5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e68d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e68d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e68d5-114">Not supported.</span></span> |
| <span data-ttu-id="e68d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e68d5-115">Application</span></span>                            | <span data-ttu-id="e68d5-116">Policy.Read.All и Application.ReadWrite.OwnedBy, Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e68d5-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e68d5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e68d5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="e68d5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e68d5-118">Request headers</span></span>

| <span data-ttu-id="e68d5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e68d5-119">Name</span></span>          | <span data-ttu-id="e68d5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e68d5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e68d5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e68d5-121">Authorization</span></span> | <span data-ttu-id="e68d5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e68d5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e68d5-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e68d5-124">Request body</span></span>

<span data-ttu-id="e68d5-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e68d5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e68d5-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e68d5-126">Response</span></span>

<span data-ttu-id="e68d5-127">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [claimsMappingPolicy](../resources/claimsmappingpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e68d5-127">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e68d5-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e68d5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e68d5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e68d5-129">Request</span></span>

<span data-ttu-id="e68d5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e68d5-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e68d5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e68d5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_claimsmappingpolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="e68d5-132">C#</span><span class="sxs-lookup"><span data-stu-id="e68d5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-claimsmappingpolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e68d5-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e68d5-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-claimsmappingpolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e68d5-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e68d5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-claimsmappingpolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e68d5-135">Java</span><span class="sxs-lookup"><span data-stu-id="e68d5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-claimsmappingpolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e68d5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e68d5-136">Response</span></span>

<span data-ttu-id="e68d5-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e68d5-137">The following is an example of the response.</span></span>

> <span data-ttu-id="e68d5-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e68d5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

