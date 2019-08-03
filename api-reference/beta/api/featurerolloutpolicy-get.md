---
title: Получение Феатурероллаутполици
description: Получение свойств и связей объекта феатурероллаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 58f2145ad897c142b09f0a26edad8e362f1778bf
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172865"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="84887-103">Получение Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="84887-103">Get featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84887-104">Получение свойств и связей объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="84887-104">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84887-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84887-105">Permissions</span></span>

<span data-ttu-id="84887-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84887-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84887-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84887-108">Permission type</span></span>                        | <span data-ttu-id="84887-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84887-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="84887-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84887-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="84887-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="84887-111">Policy.Read.All</span></span> |
| <span data-ttu-id="84887-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84887-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84887-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84887-113">Not supported.</span></span> |
| <span data-ttu-id="84887-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84887-114">Application</span></span>                            | <span data-ttu-id="84887-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84887-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84887-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84887-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84887-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84887-117">Optional query parameters</span></span>

<span data-ttu-id="84887-118">Этот метод поддерживает параметр `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="84887-118">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="84887-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="84887-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="84887-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84887-120">Request headers</span></span>

| <span data-ttu-id="84887-121">Имя</span><span class="sxs-lookup"><span data-stu-id="84887-121">Name</span></span>      |<span data-ttu-id="84887-122">Описание</span><span class="sxs-lookup"><span data-stu-id="84887-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84887-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84887-123">Authorization</span></span> | <span data-ttu-id="84887-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="84887-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="84887-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84887-125">Request body</span></span>

<span data-ttu-id="84887-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84887-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84887-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="84887-127">Response</span></span>

<span data-ttu-id="84887-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84887-128">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84887-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="84887-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84887-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="84887-130">Request</span></span>

<span data-ttu-id="84887-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84887-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="84887-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="84887-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84887-133">C#</span><span class="sxs-lookup"><span data-stu-id="84887-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84887-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="84887-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84887-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="84887-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="84887-136">Java</span><span class="sxs-lookup"><span data-stu-id="84887-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="84887-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="84887-137">Response</span></span>

<span data-ttu-id="84887-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84887-138">The following is an example of the response.</span></span>

> <span data-ttu-id="84887-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84887-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="request"></a><span data-ttu-id="84887-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="84887-141">Request</span></span>

<span data-ttu-id="84887-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84887-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="84887-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="84887-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84887-144">C#</span><span class="sxs-lookup"><span data-stu-id="84887-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84887-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="84887-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84887-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="84887-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="84887-147">Java</span><span class="sxs-lookup"><span data-stu-id="84887-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="84887-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="84887-148">Response</span></span>

<span data-ttu-id="84887-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="84887-149">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="84887-150">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="84887-150">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="84887-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84887-151">All the properties will be returned from an actual call.</span></span>

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
