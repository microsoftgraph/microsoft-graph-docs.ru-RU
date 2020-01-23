---
title: Создание Клаимсмаппингполици
description: Создание нового Клаимсмаппингполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: badb0bc304d4fa41a4826e7b166308dd80e148c3
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476352"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="aade9-103">Создание Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="aade9-103">Create claimsMappingPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aade9-104">Создание нового объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="aade9-104">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aade9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aade9-105">Permissions</span></span>

<span data-ttu-id="aade9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aade9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aade9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aade9-108">Permission type</span></span>                        | <span data-ttu-id="aade9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aade9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aade9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aade9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="aade9-111">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="aade9-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="aade9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aade9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aade9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aade9-113">Not supported.</span></span> |
| <span data-ttu-id="aade9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aade9-114">Application</span></span>                            | <span data-ttu-id="aade9-115">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="aade9-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="aade9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aade9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="aade9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aade9-117">Request headers</span></span>

| <span data-ttu-id="aade9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="aade9-118">Name</span></span>          | <span data-ttu-id="aade9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="aade9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="aade9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aade9-120">Authorization</span></span> | <span data-ttu-id="aade9-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="aade9-121">Bearer {token}</span></span> |
| <span data-ttu-id="aade9-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aade9-122">Content-type</span></span> | <span data-ttu-id="aade9-123">application/json</span><span class="sxs-lookup"><span data-stu-id="aade9-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="aade9-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aade9-124">Request body</span></span>

<span data-ttu-id="aade9-125">В тексте запроса добавьте представление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aade9-125">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aade9-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="aade9-126">Response</span></span>

<span data-ttu-id="aade9-127">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [клаимсмаппингполици](../resources/claimsmappingpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aade9-127">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aade9-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="aade9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aade9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="aade9-129">Request</span></span>

<span data-ttu-id="aade9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aade9-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="aade9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="aade9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_claimsmappingpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/claimsMappingPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aade9-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aade9-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aade9-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aade9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aade9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aade9-134">Response</span></span>

<span data-ttu-id="aade9-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aade9-135">The following is an example of the response.</span></span>

> <span data-ttu-id="aade9-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aade9-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
