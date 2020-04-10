---
title: Список назначенных КлаимсмаппингполиЦиес
description: Список КлаимсмаппингполиЦиес, назначенных для servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 83bad7c305506814bdd931dcf29a4a3513625fd3
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219090"
---
# <a name="list-assigned-claimsmappingpolicy"></a><span data-ttu-id="03ee7-103">Список назначенных Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="03ee7-103">List assigned claimsMappingPolicy</span></span>

<span data-ttu-id="03ee7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03ee7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03ee7-105">Перечисление объектов [клаимсмаппингполици](../resources/claimsmappingpolicy.md) , назначенных для [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="03ee7-105">List the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="03ee7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03ee7-106">Permissions</span></span>

<span data-ttu-id="03ee7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03ee7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03ee7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03ee7-109">Permission type</span></span>                        | <span data-ttu-id="03ee7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03ee7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="03ee7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03ee7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="03ee7-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="03ee7-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="03ee7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03ee7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03ee7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03ee7-114">Not supported.</span></span> |
| <span data-ttu-id="03ee7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03ee7-115">Application</span></span>                            | <span data-ttu-id="03ee7-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="03ee7-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03ee7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03ee7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="03ee7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03ee7-118">Request headers</span></span>

| <span data-ttu-id="03ee7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="03ee7-119">Name</span></span>          | <span data-ttu-id="03ee7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="03ee7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="03ee7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="03ee7-121">Authorization</span></span> | <span data-ttu-id="03ee7-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="03ee7-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="03ee7-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03ee7-123">Request body</span></span>

<span data-ttu-id="03ee7-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03ee7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03ee7-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="03ee7-125">Response</span></span>

<span data-ttu-id="03ee7-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [клаимсмаппингполици](../resources/claimsMappingPolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03ee7-126">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsMappingPolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03ee7-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="03ee7-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03ee7-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="03ee7-128">Request</span></span>

<span data-ttu-id="03ee7-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03ee7-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="03ee7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="03ee7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_claimsmappingpolicies_on_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="03ee7-131">C#</span><span class="sxs-lookup"><span data-stu-id="03ee7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-claimsmappingpolicies-on-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03ee7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03ee7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-claimsmappingpolicies-on-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03ee7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03ee7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-claimsmappingpolicies-on-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="03ee7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="03ee7-134">Response</span></span>

<span data-ttu-id="03ee7-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03ee7-135">The following is an example of the response.</span></span>

> <span data-ttu-id="03ee7-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03ee7-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
