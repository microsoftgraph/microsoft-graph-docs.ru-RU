---
title: Получение Феатурероллаутполици
description: Получение свойств и связей объекта феатурероллаутполици.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6fdf941383d8f64e690899b80044300c3d69d684
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181121"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="0caf7-103">Получение Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="0caf7-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="0caf7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0caf7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0caf7-105">Получение свойств и связей объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0caf7-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0caf7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0caf7-106">Permissions</span></span>

<span data-ttu-id="0caf7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0caf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0caf7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0caf7-109">Permission type</span></span>                        | <span data-ttu-id="0caf7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0caf7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0caf7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0caf7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0caf7-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="0caf7-112">Policy.Read.All</span></span> |
| <span data-ttu-id="0caf7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0caf7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0caf7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0caf7-114">Not supported.</span></span> |
| <span data-ttu-id="0caf7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0caf7-115">Application</span></span>                            | <span data-ttu-id="0caf7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0caf7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0caf7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0caf7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0caf7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0caf7-118">Optional query parameters</span></span>

<span data-ttu-id="0caf7-119">Этот метод поддерживает параметр `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0caf7-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="0caf7-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0caf7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0caf7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0caf7-121">Request headers</span></span>

| <span data-ttu-id="0caf7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0caf7-122">Name</span></span>      |<span data-ttu-id="0caf7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0caf7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0caf7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0caf7-124">Authorization</span></span> | <span data-ttu-id="0caf7-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0caf7-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0caf7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0caf7-126">Request body</span></span>

<span data-ttu-id="0caf7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0caf7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0caf7-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0caf7-128">Response</span></span>

<span data-ttu-id="0caf7-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0caf7-129">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0caf7-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="0caf7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0caf7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0caf7-131">Request</span></span>

<span data-ttu-id="0caf7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0caf7-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0caf7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0caf7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="0caf7-134">C#</span><span class="sxs-lookup"><span data-stu-id="0caf7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0caf7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0caf7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0caf7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0caf7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0caf7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0caf7-137">Response</span></span>

<span data-ttu-id="0caf7-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0caf7-138">The following is an example of the response.</span></span>

> <span data-ttu-id="0caf7-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0caf7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="request"></a><span data-ttu-id="0caf7-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0caf7-141">Request</span></span>

<span data-ttu-id="0caf7-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0caf7-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0caf7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0caf7-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="c"></a>[<span data-ttu-id="0caf7-144">C#</span><span class="sxs-lookup"><span data-stu-id="0caf7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0caf7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0caf7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0caf7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0caf7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0caf7-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0caf7-147">Response</span></span>

<span data-ttu-id="0caf7-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0caf7-148">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="0caf7-149">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0caf7-149">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0caf7-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0caf7-150">All the properties will be returned from an actual call.</span></span>

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
