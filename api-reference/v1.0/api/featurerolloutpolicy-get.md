---
title: Get featureRolloutPolicy
description: Извлечение свойств и связей объекта featurerolloutpolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ab2bb89809fb5f60952f8c188922bd28c1b25c93
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052385"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="37db1-103">Get featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="37db1-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="37db1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37db1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37db1-105">Извлечение свойств и связей [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="37db1-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37db1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37db1-106">Permissions</span></span>

<span data-ttu-id="37db1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37db1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37db1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37db1-109">Permission type</span></span>                        | <span data-ttu-id="37db1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37db1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37db1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37db1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37db1-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37db1-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="37db1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37db1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37db1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37db1-114">Not supported.</span></span> |
| <span data-ttu-id="37db1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37db1-115">Application</span></span>                            | <span data-ttu-id="37db1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37db1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37db1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37db1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37db1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37db1-118">Optional query parameters</span></span>

<span data-ttu-id="37db1-119">Этот метод поддерживает параметр `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="37db1-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="37db1-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="37db1-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="37db1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37db1-121">Request headers</span></span>

| <span data-ttu-id="37db1-122">Имя</span><span class="sxs-lookup"><span data-stu-id="37db1-122">Name</span></span>      |<span data-ttu-id="37db1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="37db1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37db1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37db1-124">Authorization</span></span> | <span data-ttu-id="37db1-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="37db1-125">Bearer {token}.</span></span> <span data-ttu-id="37db1-126">Обязательна</span><span class="sxs-lookup"><span data-stu-id="37db1-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="37db1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37db1-127">Request body</span></span>

<span data-ttu-id="37db1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37db1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37db1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="37db1-129">Response</span></span>

<span data-ttu-id="37db1-130">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [featureRolloutPolicy](../resources/featurerolloutpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="37db1-130">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37db1-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="37db1-131">Examples</span></span>

### <a name="example-1-get-a-feature-rollout-policy"></a><span data-ttu-id="37db1-132">Пример 1. Получить политику выкатки функций</span><span class="sxs-lookup"><span data-stu-id="37db1-132">Example 1: Get a feature rollout policy</span></span>

#### <a name="request"></a><span data-ttu-id="37db1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="37db1-133">Request</span></span>

<span data-ttu-id="37db1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37db1-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="37db1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="37db1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="37db1-136">C#</span><span class="sxs-lookup"><span data-stu-id="37db1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37db1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37db1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37db1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37db1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37db1-139">Java</span><span class="sxs-lookup"><span data-stu-id="37db1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37db1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="37db1-140">Response</span></span>

<span data-ttu-id="37db1-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="37db1-141">The following is an example of the response.</span></span>

> <span data-ttu-id="37db1-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="37db1-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="example-2-get-a-feature-rollout-policy-and-expand-appliesto"></a><span data-ttu-id="37db1-143">Пример 2. Получить политику выкатки функций и расширить appliesTo</span><span class="sxs-lookup"><span data-stu-id="37db1-143">Example 2: Get a feature rollout policy and expand appliesTo</span></span>

#### <a name="request"></a><span data-ttu-id="37db1-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="37db1-144">Request</span></span>

<span data-ttu-id="37db1-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37db1-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="37db1-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="37db1-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_expand_appliesTo"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="c"></a>[<span data-ttu-id="37db1-147">C#</span><span class="sxs-lookup"><span data-stu-id="37db1-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-expand-appliesto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37db1-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37db1-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-expand-appliesto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37db1-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37db1-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-expand-appliesto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37db1-150">Java</span><span class="sxs-lookup"><span data-stu-id="37db1-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-expand-appliesto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37db1-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="37db1-151">Response</span></span>

<span data-ttu-id="37db1-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="37db1-152">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="37db1-153">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="37db1-153">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false,
  "appliesTo": [
    {
      "id": "2441b489-4f12-4882-b039-8f6006bd66da",
      "objectType": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


