---
title: Список АктивитибаседтимеаутполиЦиес
description: Получение списка объектов Активитибаседтимеаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9191e911f1e7a91d8423aca7b7feb1c9ace6c8a9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441841"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="994ed-103">Список АктивитибаседтимеаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="994ed-103">List activityBasedTimeoutPolicies</span></span>

<span data-ttu-id="994ed-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="994ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="994ed-105">Получение списка объектов [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="994ed-105">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="994ed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="994ed-106">Permissions</span></span>

<span data-ttu-id="994ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="994ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="994ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="994ed-109">Permission type</span></span>                        | <span data-ttu-id="994ed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="994ed-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="994ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="994ed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="994ed-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="994ed-112">Policy.Read.All</span></span> |
| <span data-ttu-id="994ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="994ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="994ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="994ed-114">Not supported.</span></span> |
| <span data-ttu-id="994ed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="994ed-115">Application</span></span>                            | <span data-ttu-id="994ed-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="994ed-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="994ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="994ed-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="994ed-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="994ed-118">Optional query parameters</span></span>

<span data-ttu-id="994ed-119">Этот метод поддерживает `$filter`параметры запросов `$select` OData `$top` и OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="994ed-119">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="994ed-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="994ed-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="994ed-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="994ed-121">Request headers</span></span>

| <span data-ttu-id="994ed-122">Имя</span><span class="sxs-lookup"><span data-stu-id="994ed-122">Name</span></span>      |<span data-ttu-id="994ed-123">Описание</span><span class="sxs-lookup"><span data-stu-id="994ed-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="994ed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="994ed-124">Authorization</span></span> | <span data-ttu-id="994ed-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="994ed-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="994ed-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="994ed-126">Request body</span></span>

<span data-ttu-id="994ed-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="994ed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="994ed-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="994ed-128">Response</span></span>

<span data-ttu-id="994ed-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="994ed-129">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="994ed-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="994ed-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="994ed-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="994ed-131">Request</span></span>

<span data-ttu-id="994ed-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="994ed-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="994ed-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="994ed-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
```
# <a name="c"></a>[<span data-ttu-id="994ed-134">C#</span><span class="sxs-lookup"><span data-stu-id="994ed-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="994ed-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="994ed-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="994ed-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="994ed-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="994ed-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="994ed-137">Response</span></span>

<span data-ttu-id="994ed-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="994ed-138">The following is an example of the response.</span></span>

> <span data-ttu-id="994ed-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="994ed-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List activityBasedTimeoutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
