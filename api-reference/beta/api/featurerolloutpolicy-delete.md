---
title: Удаление featureRolloutPolicy
description: Удаление объекта featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fc776712a60dd4beaafb2e9ca38391fdf73a0c10
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508924"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="1f32f-103">Удаление featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="1f32f-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="1f32f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f32f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f32f-105">Удаление [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1f32f-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f32f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f32f-106">Permissions</span></span>

<span data-ttu-id="1f32f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f32f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f32f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f32f-109">Permission type</span></span>                        | <span data-ttu-id="1f32f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f32f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1f32f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f32f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f32f-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f32f-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="1f32f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f32f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f32f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f32f-114">Not supported.</span></span> |
| <span data-ttu-id="1f32f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f32f-115">Application</span></span>                            | <span data-ttu-id="1f32f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f32f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f32f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f32f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1f32f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f32f-118">Request headers</span></span>

| <span data-ttu-id="1f32f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1f32f-119">Name</span></span>          | <span data-ttu-id="1f32f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1f32f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1f32f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f32f-121">Authorization</span></span> | <span data-ttu-id="1f32f-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="1f32f-122">Bearer {token}.</span></span> <span data-ttu-id="1f32f-123">Обязательна</span><span class="sxs-lookup"><span data-stu-id="1f32f-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f32f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f32f-124">Request body</span></span>

<span data-ttu-id="1f32f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f32f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f32f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f32f-126">Response</span></span>

<span data-ttu-id="1f32f-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1f32f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f32f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="1f32f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f32f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f32f-130">Request</span></span>

<span data-ttu-id="1f32f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f32f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f32f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f32f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy_policies"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="1f32f-133">C#</span><span class="sxs-lookup"><span data-stu-id="1f32f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-featurerolloutpolicy-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f32f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f32f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-featurerolloutpolicy-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f32f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f32f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-featurerolloutpolicy-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f32f-136">Java</span><span class="sxs-lookup"><span data-stu-id="1f32f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-featurerolloutpolicy-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f32f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f32f-137">Response</span></span>

<span data-ttu-id="1f32f-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1f32f-138">The following is an example of the response.</span></span>

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
  "description": "Delete featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


