---
title: Получение Активитибаседтимеаутполици
description: Получение свойств объекта Активитибаседтимеаутполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 131a07a9b7935b97d9b392a555503fe68ac4c2a8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983433"
---
# <a name="get-activitybasedtimeoutpolicy"></a><span data-ttu-id="cc57d-103">Получение Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="cc57d-103">Get activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="cc57d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc57d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc57d-105">Получение свойств объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="cc57d-105">Get the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc57d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc57d-106">Permissions</span></span>

<span data-ttu-id="cc57d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc57d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc57d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc57d-109">Permission type</span></span>                        | <span data-ttu-id="cc57d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc57d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cc57d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc57d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc57d-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="cc57d-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="cc57d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc57d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc57d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc57d-114">Not supported.</span></span> |
| <span data-ttu-id="cc57d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc57d-115">Application</span></span>                            | <span data-ttu-id="cc57d-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="cc57d-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc57d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc57d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc57d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cc57d-118">Optional query parameters</span></span>

<span data-ttu-id="cc57d-119">Этот метод поддерживает `$select` параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cc57d-119">This method supports the `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="cc57d-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cc57d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc57d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc57d-121">Request headers</span></span>

| <span data-ttu-id="cc57d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cc57d-122">Name</span></span>      |<span data-ttu-id="cc57d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cc57d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cc57d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc57d-124">Authorization</span></span> | <span data-ttu-id="cc57d-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="cc57d-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc57d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cc57d-126">Request body</span></span>

<span data-ttu-id="cc57d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc57d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc57d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc57d-128">Response</span></span>

<span data-ttu-id="cc57d-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc57d-129">If successful, this method returns a `200 OK` response code and the requested [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc57d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc57d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cc57d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc57d-131">Request</span></span>

<span data-ttu-id="cc57d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc57d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc57d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc57d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="cc57d-134">C#</span><span class="sxs-lookup"><span data-stu-id="cc57d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc57d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc57d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc57d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc57d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cc57d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc57d-137">Response</span></span>

<span data-ttu-id="cc57d-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc57d-138">The following is an example of the response.</span></span>

> <span data-ttu-id="cc57d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc57d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Get activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


