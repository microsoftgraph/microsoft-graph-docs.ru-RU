---
title: Удаление типа ресурса claimsMappingPolicy
description: Удаление объекта Клаимсмаппингполици из servicePrincipal.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc126bcd7c386ae3d1609a58a44b3ee9f8355972
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013029"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="43732-103">Удаление типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="43732-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="43732-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43732-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="43732-105">Удаление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) из [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="43732-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="43732-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43732-106">Permissions</span></span>

<span data-ttu-id="43732-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43732-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43732-109">Permission type</span></span>                        | <span data-ttu-id="43732-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43732-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="43732-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43732-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="43732-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="43732-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="43732-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43732-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43732-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43732-114">Not supported.</span></span> |
| <span data-ttu-id="43732-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43732-115">Application</span></span>                            | <span data-ttu-id="43732-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="43732-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43732-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43732-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="43732-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43732-118">Request headers</span></span>

| <span data-ttu-id="43732-119">Имя</span><span class="sxs-lookup"><span data-stu-id="43732-119">Name</span></span>          | <span data-ttu-id="43732-120">Описание</span><span class="sxs-lookup"><span data-stu-id="43732-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="43732-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43732-121">Authorization</span></span> | <span data-ttu-id="43732-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43732-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43732-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43732-124">Request body</span></span>

<span data-ttu-id="43732-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43732-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43732-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="43732-126">Response</span></span>

<span data-ttu-id="43732-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="43732-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="43732-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="43732-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43732-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="43732-129">Request</span></span>

<span data-ttu-id="43732-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43732-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="43732-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="43732-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="43732-132">C#</span><span class="sxs-lookup"><span data-stu-id="43732-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43732-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43732-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43732-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43732-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43732-135">Java</span><span class="sxs-lookup"><span data-stu-id="43732-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="43732-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="43732-136">Response</span></span>

<span data-ttu-id="43732-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="43732-137">The following is an example of the response.</span></span>

> <span data-ttu-id="43732-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43732-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

