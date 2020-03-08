---
title: Список назначенных КлаимсмаппингполиЦиес
description: Список КлаимсмаппингполиЦиес, назначенных для servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 33146ef8033643fc136f6e4d16d54a63ce92a470
ms.sourcegitcommit: 435d80cfa71574c06d24780c591d4303a5cd9636
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2020
ms.locfileid: "42562747"
---
# <a name="list-assigned-claimsmappingpolicy"></a><span data-ttu-id="2bcf4-103">Список назначенных Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="2bcf4-103">List assigned claimsMappingPolicy</span></span>

<span data-ttu-id="2bcf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bcf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bcf4-105">Перечисление объектов [клаимсмаппингполици](../resources/claimsmappingpolicy.md) , назначенных для [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="2bcf4-105">List the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2bcf4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2bcf4-106">Permissions</span></span>

<span data-ttu-id="2bcf4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bcf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2bcf4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bcf4-109">Permission type</span></span>                        | <span data-ttu-id="2bcf4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bcf4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2bcf4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bcf4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2bcf4-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2bcf4-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="2bcf4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bcf4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bcf4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bcf4-114">Not supported.</span></span> |
| <span data-ttu-id="2bcf4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2bcf4-115">Application</span></span>                            | <span data-ttu-id="2bcf4-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2bcf4-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bcf4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bcf4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="2bcf4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2bcf4-118">Request headers</span></span>

| <span data-ttu-id="2bcf4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2bcf4-119">Name</span></span>          | <span data-ttu-id="2bcf4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2bcf4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2bcf4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bcf4-121">Authorization</span></span> | <span data-ttu-id="2bcf4-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="2bcf4-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2bcf4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2bcf4-123">Request body</span></span>

<span data-ttu-id="2bcf4-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2bcf4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bcf4-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="2bcf4-125">Response</span></span>

<span data-ttu-id="2bcf4-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [клаимсмаппингполици](../resources/claimsMappingPolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2bcf4-126">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsMappingPolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2bcf4-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="2bcf4-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2bcf4-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bcf4-128">Request</span></span>

<span data-ttu-id="2bcf4-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2bcf4-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2bcf4-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bcf4-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_claimsmappingpolicies_on_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="2bcf4-131">C#</span><span class="sxs-lookup"><span data-stu-id="2bcf4-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-claimsmappingpolicies-on-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2bcf4-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bcf4-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-claimsmappingpolicies-on-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2bcf4-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2bcf4-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-claimsmappingpolicies-on-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2bcf4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bcf4-134">Response</span></span>

<span data-ttu-id="2bcf4-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2bcf4-135">The following is an example of the response.</span></span>

> <span data-ttu-id="2bcf4-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2bcf4-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
