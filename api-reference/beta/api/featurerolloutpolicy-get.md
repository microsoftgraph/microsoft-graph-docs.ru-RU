---
title: Get featureRolloutPolicy
description: Извлечение свойств и связей объекта featurerolloutpolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5cd9830833ed06febf4b1b66b77d3ca4f72c52f8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436136"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="90319-103">Get featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="90319-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="90319-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90319-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90319-105">Извлечение свойств и связей [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="90319-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90319-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90319-106">Permissions</span></span>

<span data-ttu-id="90319-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90319-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90319-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90319-109">Permission type</span></span>                        | <span data-ttu-id="90319-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90319-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90319-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90319-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90319-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="90319-112">Policy.Read.All</span></span> |
| <span data-ttu-id="90319-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90319-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90319-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90319-114">Not supported.</span></span> |
| <span data-ttu-id="90319-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90319-115">Application</span></span>                            | <span data-ttu-id="90319-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90319-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90319-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90319-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90319-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="90319-118">Optional query parameters</span></span>

<span data-ttu-id="90319-119">Этот метод поддерживает параметр `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="90319-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="90319-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="90319-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="90319-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90319-121">Request headers</span></span>

| <span data-ttu-id="90319-122">Имя</span><span class="sxs-lookup"><span data-stu-id="90319-122">Name</span></span>      |<span data-ttu-id="90319-123">Описание</span><span class="sxs-lookup"><span data-stu-id="90319-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90319-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90319-124">Authorization</span></span> | <span data-ttu-id="90319-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="90319-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="90319-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90319-126">Request body</span></span>

<span data-ttu-id="90319-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90319-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90319-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="90319-128">Response</span></span>

<span data-ttu-id="90319-129">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [featureRolloutPolicy](../resources/featurerolloutpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="90319-129">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90319-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="90319-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90319-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="90319-131">Request</span></span>

<span data-ttu-id="90319-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90319-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90319-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="90319-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="90319-134">C#</span><span class="sxs-lookup"><span data-stu-id="90319-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90319-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90319-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90319-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90319-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90319-137">Java</span><span class="sxs-lookup"><span data-stu-id="90319-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="90319-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="90319-138">Response</span></span>

<span data-ttu-id="90319-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90319-139">The following is an example of the response.</span></span>

> <span data-ttu-id="90319-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90319-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="request"></a><span data-ttu-id="90319-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="90319-142">Request</span></span>

<span data-ttu-id="90319-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90319-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90319-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="90319-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="c"></a>[<span data-ttu-id="90319-145">C#</span><span class="sxs-lookup"><span data-stu-id="90319-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90319-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90319-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90319-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90319-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90319-148">Java</span><span class="sxs-lookup"><span data-stu-id="90319-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="90319-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="90319-149">Response</span></span>

<span data-ttu-id="90319-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90319-150">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="90319-151">Объект отклика, показанный здесь, может быть сокращен для чтения.</span><span class="sxs-lookup"><span data-stu-id="90319-151">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="90319-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90319-152">All the properties will be returned from an actual call.</span></span>

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


