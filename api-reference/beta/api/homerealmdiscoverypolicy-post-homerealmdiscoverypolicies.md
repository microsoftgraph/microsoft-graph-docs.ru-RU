---
title: Создание Хомереалмдисковериполици
description: Создание нового Хомереалмдисковериполици.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f28e5922c7742ced5e9b66aecb69813d4da59ca
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964739"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="10a51-103">Создание Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="10a51-103">Create homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="10a51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10a51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10a51-105">Создание нового объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="10a51-105">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="10a51-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10a51-106">Permissions</span></span>

<span data-ttu-id="10a51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10a51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10a51-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10a51-109">Permission type</span></span>                        | <span data-ttu-id="10a51-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10a51-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="10a51-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10a51-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10a51-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="10a51-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="10a51-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10a51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10a51-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10a51-114">Not supported.</span></span> |
| <span data-ttu-id="10a51-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="10a51-115">Application</span></span>                            | <span data-ttu-id="10a51-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="10a51-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="10a51-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10a51-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="10a51-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10a51-118">Request headers</span></span>

| <span data-ttu-id="10a51-119">Имя</span><span class="sxs-lookup"><span data-stu-id="10a51-119">Name</span></span>          | <span data-ttu-id="10a51-120">Описание</span><span class="sxs-lookup"><span data-stu-id="10a51-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="10a51-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10a51-121">Authorization</span></span> | <span data-ttu-id="10a51-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="10a51-122">Bearer {token}</span></span> |
| <span data-ttu-id="10a51-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10a51-123">Content-type</span></span> | <span data-ttu-id="10a51-124">application/json</span><span class="sxs-lookup"><span data-stu-id="10a51-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="10a51-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10a51-125">Request body</span></span>

<span data-ttu-id="10a51-126">В тексте запроса добавьте представление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10a51-126">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="10a51-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="10a51-127">Response</span></span>

<span data-ttu-id="10a51-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10a51-128">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10a51-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="10a51-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10a51-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="10a51-130">Request</span></span>

<span data-ttu-id="10a51-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10a51-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10a51-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="10a51-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_homerealmdiscoverypolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="10a51-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10a51-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10a51-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10a51-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="10a51-135">C#</span><span class="sxs-lookup"><span data-stu-id="10a51-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10a51-136">Java</span><span class="sxs-lookup"><span data-stu-id="10a51-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10a51-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="10a51-137">Response</span></span>

<span data-ttu-id="10a51-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10a51-138">The following is an example of the response.</span></span>

> <span data-ttu-id="10a51-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10a51-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
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
  "description": "Create homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


