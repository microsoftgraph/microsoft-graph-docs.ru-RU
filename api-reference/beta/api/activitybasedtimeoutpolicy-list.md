---
title: Список АктивитибаседтимеаутполиЦиес
description: Получение списка объектов Активитибаседтимеаутполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f13fd20baa7ddb511108bed1c77e1e3cc47eb791
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983424"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="45cf4-103">Список АктивитибаседтимеаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="45cf4-103">List activityBasedTimeoutPolicies</span></span>

<span data-ttu-id="45cf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45cf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45cf4-105">Получение списка объектов [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="45cf4-105">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="45cf4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45cf4-106">Permissions</span></span>

<span data-ttu-id="45cf4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45cf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45cf4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45cf4-109">Permission type</span></span>                        | <span data-ttu-id="45cf4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45cf4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="45cf4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45cf4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="45cf4-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="45cf4-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="45cf4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45cf4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45cf4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45cf4-114">Not supported.</span></span> |
| <span data-ttu-id="45cf4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45cf4-115">Application</span></span>                            | <span data-ttu-id="45cf4-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="45cf4-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="45cf4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45cf4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45cf4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="45cf4-118">Optional query parameters</span></span>

<span data-ttu-id="45cf4-119">Этот метод поддерживает `$filter` `$select` `$top` параметры запросов OData и OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="45cf4-119">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="45cf4-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="45cf4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="45cf4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45cf4-121">Request headers</span></span>

| <span data-ttu-id="45cf4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="45cf4-122">Name</span></span>      |<span data-ttu-id="45cf4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="45cf4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="45cf4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="45cf4-124">Authorization</span></span> | <span data-ttu-id="45cf4-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="45cf4-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="45cf4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45cf4-126">Request body</span></span>

<span data-ttu-id="45cf4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45cf4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45cf4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="45cf4-128">Response</span></span>

<span data-ttu-id="45cf4-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45cf4-129">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45cf4-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="45cf4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45cf4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="45cf4-131">Request</span></span>

<span data-ttu-id="45cf4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45cf4-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45cf4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="45cf4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
```
# <a name="c"></a>[<span data-ttu-id="45cf4-134">C#</span><span class="sxs-lookup"><span data-stu-id="45cf4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45cf4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45cf4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45cf4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45cf4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45cf4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="45cf4-137">Response</span></span>

<span data-ttu-id="45cf4-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="45cf4-138">The following is an example of the response.</span></span>

> <span data-ttu-id="45cf4-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45cf4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


