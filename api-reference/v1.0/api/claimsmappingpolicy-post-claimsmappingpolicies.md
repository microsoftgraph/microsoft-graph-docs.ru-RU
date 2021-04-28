---
title: Создание claimsMappingPolicy
description: Создание новых утвержденийMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f0f22d941c5d7f5ed1e3691e461d6cda25d5b31f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051552"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="62c68-103">Создание claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="62c68-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="62c68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62c68-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62c68-105">Создайте новый [объект claimsMappingPolicy.](../resources/claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="62c68-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="62c68-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62c68-106">Permissions</span></span>

<span data-ttu-id="62c68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62c68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62c68-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62c68-109">Permission type</span></span>                        | <span data-ttu-id="62c68-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62c68-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="62c68-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62c68-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="62c68-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="62c68-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="62c68-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62c68-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62c68-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62c68-114">Not supported.</span></span> |
| <span data-ttu-id="62c68-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62c68-115">Application</span></span>                            | <span data-ttu-id="62c68-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="62c68-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="62c68-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62c68-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="62c68-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62c68-118">Request headers</span></span>

| <span data-ttu-id="62c68-119">Имя</span><span class="sxs-lookup"><span data-stu-id="62c68-119">Name</span></span>          | <span data-ttu-id="62c68-120">Описание</span><span class="sxs-lookup"><span data-stu-id="62c68-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="62c68-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62c68-121">Authorization</span></span> | <span data-ttu-id="62c68-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="62c68-122">Bearer {token}</span></span> |
| <span data-ttu-id="62c68-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62c68-123">Content-type</span></span> | <span data-ttu-id="62c68-124">application/json</span><span class="sxs-lookup"><span data-stu-id="62c68-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="62c68-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62c68-125">Request body</span></span>

<span data-ttu-id="62c68-126">В теле запроса поставляем представление JSON объекта [claimsMappingPolicy.](../resources/claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="62c68-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="62c68-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="62c68-127">Response</span></span>

<span data-ttu-id="62c68-128">В случае успеха этот метод возвращает код ответа и новый объект `201 Created` [claimsMappingPolicy](../resources/claimsmappingpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="62c68-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62c68-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="62c68-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62c68-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="62c68-130">Request</span></span>

<span data-ttu-id="62c68-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62c68-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="62c68-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="62c68-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_claimsmappingpolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="62c68-133">C#</span><span class="sxs-lookup"><span data-stu-id="62c68-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62c68-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62c68-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62c68-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62c68-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62c68-136">Java</span><span class="sxs-lookup"><span data-stu-id="62c68-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-claimsmappingpolicy-from-claimsmappingpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="62c68-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="62c68-137">Response</span></span>

<span data-ttu-id="62c68-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="62c68-138">The following is an example of the response.</span></span>

> <span data-ttu-id="62c68-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62c68-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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

