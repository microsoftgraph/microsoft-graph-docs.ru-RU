---
title: Создание Клаимсмаппингполици
description: Создание нового Клаимсмаппингполици.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8fa07178f6c485a98353c7b5718b0b0c9173f84f
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916519"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="398d4-103">Создание Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="398d4-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="398d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="398d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="398d4-105">Создание нового объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="398d4-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="398d4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="398d4-106">Permissions</span></span>

<span data-ttu-id="398d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="398d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="398d4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="398d4-109">Permission type</span></span>                        | <span data-ttu-id="398d4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="398d4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="398d4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="398d4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="398d4-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="398d4-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="398d4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="398d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="398d4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="398d4-114">Not supported.</span></span> |
| <span data-ttu-id="398d4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="398d4-115">Application</span></span>                            | <span data-ttu-id="398d4-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="398d4-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="398d4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="398d4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="398d4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="398d4-118">Request headers</span></span>

| <span data-ttu-id="398d4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="398d4-119">Name</span></span>          | <span data-ttu-id="398d4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="398d4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="398d4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="398d4-121">Authorization</span></span> | <span data-ttu-id="398d4-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="398d4-122">Bearer {token}</span></span> |
| <span data-ttu-id="398d4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="398d4-123">Content-type</span></span> | <span data-ttu-id="398d4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="398d4-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="398d4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="398d4-125">Request body</span></span>

<span data-ttu-id="398d4-126">В тексте запроса добавьте представление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="398d4-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="398d4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="398d4-127">Response</span></span>

<span data-ttu-id="398d4-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [клаимсмаппингполици](../resources/claimsmappingpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="398d4-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="398d4-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="398d4-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="398d4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="398d4-130">Request</span></span>

<span data-ttu-id="398d4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="398d4-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="398d4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="398d4-132">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="398d4-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="398d4-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="398d4-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="398d4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="398d4-135">C#</span><span class="sxs-lookup"><span data-stu-id="398d4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="398d4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="398d4-136">Response</span></span>

<span data-ttu-id="398d4-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="398d4-137">The following is an example of the response.</span></span>

> <span data-ttu-id="398d4-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="398d4-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
