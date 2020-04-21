---
title: Удаление типа ресурса claimsMappingPolicy
description: Удаление объекта Клаимсмаппингполици из servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cd159f8efd7cf0789be143034f5edce073d23398
ms.sourcegitcommit: 24092bd1e38e8adfd314dfe8dfea9b24a5c21da6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43581669"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="0000d-103">Удаление типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="0000d-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="0000d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0000d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0000d-105">Удаление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) из [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="0000d-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0000d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0000d-106">Permissions</span></span>

<span data-ttu-id="0000d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0000d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0000d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0000d-109">Permission type</span></span>                        | <span data-ttu-id="0000d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0000d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0000d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0000d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0000d-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0000d-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="0000d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0000d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0000d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0000d-114">Not supported.</span></span> |
| <span data-ttu-id="0000d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0000d-115">Application</span></span>                            | <span data-ttu-id="0000d-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0000d-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0000d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0000d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0000d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0000d-118">Request headers</span></span>

| <span data-ttu-id="0000d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0000d-119">Name</span></span>          | <span data-ttu-id="0000d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0000d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0000d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0000d-121">Authorization</span></span> | <span data-ttu-id="0000d-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="0000d-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0000d-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0000d-123">Request body</span></span>

<span data-ttu-id="0000d-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0000d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0000d-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="0000d-125">Response</span></span>

<span data-ttu-id="0000d-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0000d-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0000d-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="0000d-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0000d-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0000d-128">Request</span></span>

<span data-ttu-id="0000d-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0000d-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0000d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0000d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="0000d-131">C#</span><span class="sxs-lookup"><span data-stu-id="0000d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0000d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0000d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0000d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0000d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0000d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0000d-134">Response</span></span>

<span data-ttu-id="0000d-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0000d-135">The following is an example of the response.</span></span>

> <span data-ttu-id="0000d-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0000d-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
