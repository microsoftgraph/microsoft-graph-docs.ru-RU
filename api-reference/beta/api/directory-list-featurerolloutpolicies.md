---
title: Функция ListRolloutPolicies
description: Извлечение списка объектов featureRolloutPolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b594b19d420ec794001851132457824691794c9c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436990"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="06e11-103">Функция ListRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="06e11-103">List featureRolloutPolicies</span></span>

<span data-ttu-id="06e11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06e11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06e11-105">Извлечение списка [объектов featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06e11-105">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="06e11-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06e11-106">Permissions</span></span>

<span data-ttu-id="06e11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06e11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06e11-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06e11-109">Permission type</span></span>                        | <span data-ttu-id="06e11-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06e11-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06e11-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06e11-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="06e11-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="06e11-112">Policy.Read.All</span></span> |
| <span data-ttu-id="06e11-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06e11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06e11-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06e11-114">Not supported.</span></span> |
| <span data-ttu-id="06e11-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06e11-115">Application</span></span>                            | <span data-ttu-id="06e11-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06e11-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06e11-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06e11-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06e11-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06e11-118">Optional query parameters</span></span>

<span data-ttu-id="06e11-119">Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ: `$count` , , , , , , `$expand` `$filter` `$orderby` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="06e11-119">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="06e11-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="06e11-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="06e11-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06e11-121">Request headers</span></span>

| <span data-ttu-id="06e11-122">Имя</span><span class="sxs-lookup"><span data-stu-id="06e11-122">Name</span></span>      |<span data-ttu-id="06e11-123">Описание</span><span class="sxs-lookup"><span data-stu-id="06e11-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06e11-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06e11-124">Authorization</span></span> | <span data-ttu-id="06e11-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="06e11-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="06e11-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06e11-126">Request body</span></span>

<span data-ttu-id="06e11-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06e11-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06e11-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="06e11-128">Response</span></span>

<span data-ttu-id="06e11-129">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [featureRolloutPolicy](../resources/featurerolloutpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="06e11-129">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06e11-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="06e11-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06e11-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="06e11-131">Request</span></span>

<span data-ttu-id="06e11-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06e11-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="06e11-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="06e11-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies
```
# <a name="c"></a>[<span data-ttu-id="06e11-134">C#</span><span class="sxs-lookup"><span data-stu-id="06e11-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06e11-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06e11-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06e11-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06e11-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06e11-137">Java</span><span class="sxs-lookup"><span data-stu-id="06e11-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06e11-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="06e11-138">Response</span></span>

<span data-ttu-id="06e11-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="06e11-139">The following is an example of the response.</span></span>

> <span data-ttu-id="06e11-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06e11-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
      "displayName": "PassthroughAuthentication rollout policy",
      "description": "PassthroughAuthentication rollout policy",
      "feature": "passthroughAuthentication",
      "isEnabled": true,
      "isAppliedToOrganization": false
    },
    {
      "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
      "displayName": "SeamlessSso rollout policy",
      "description": "SeamlessSso rollout policy",
      "feature": "seamlessSso",
      "isEnabled": true,
      "isAppliedToOrganization": false
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List featureRolloutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


