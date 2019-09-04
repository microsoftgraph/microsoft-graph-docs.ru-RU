---
title: Список ФеатурероллаутполиЦиес
description: Получение списка объектов Феатурероллаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbc8c04ea5f0a50782e1ab09fc13ceedb8b3471f
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719607"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="e1180-103">Список ФеатурероллаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="e1180-103">List featureRolloutPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1180-104">Получение списка объектов [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e1180-104">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1180-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1180-105">Permissions</span></span>

<span data-ttu-id="e1180-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1180-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1180-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1180-108">Permission type</span></span>                        | <span data-ttu-id="e1180-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1180-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e1180-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1180-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1180-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1180-111">Policy.Read.All</span></span> |
| <span data-ttu-id="e1180-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1180-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1180-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1180-113">Not supported.</span></span> |
| <span data-ttu-id="e1180-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1180-114">Application</span></span>                            | <span data-ttu-id="e1180-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1180-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1180-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1180-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1180-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e1180-117">Optional query parameters</span></span>

<span data-ttu-id="e1180-118">Этот метод поддерживает следующие параметры `$count`запроса OData для настройки отклика:, `$expand` `$filter` `$orderby` `$select`,,,, `$skip`,. `$top`</span><span class="sxs-lookup"><span data-stu-id="e1180-118">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="e1180-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e1180-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1180-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1180-120">Request headers</span></span>

| <span data-ttu-id="e1180-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e1180-121">Name</span></span>      |<span data-ttu-id="e1180-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e1180-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e1180-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1180-123">Authorization</span></span> | <span data-ttu-id="e1180-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e1180-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1180-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1180-125">Request body</span></span>

<span data-ttu-id="e1180-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1180-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1180-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1180-127">Response</span></span>

<span data-ttu-id="e1180-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1180-128">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1180-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="e1180-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1180-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1180-130">Request</span></span>

<span data-ttu-id="e1180-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1180-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e1180-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1180-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1180-133">C#</span><span class="sxs-lookup"><span data-stu-id="e1180-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1180-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1180-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1180-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e1180-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1180-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1180-136">Response</span></span>

<span data-ttu-id="e1180-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1180-137">The following is an example of the response.</span></span>

> <span data-ttu-id="e1180-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1180-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
