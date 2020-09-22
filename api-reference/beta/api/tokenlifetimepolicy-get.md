---
title: Получение Токенлифетимеполици
description: Получение свойств и связей объекта Токенлифетимеполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 14536ede77b27ab888d3c4d845ddb75f0579e3ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062262"
---
# <a name="get-tokenlifetimepolicy"></a><span data-ttu-id="8b07d-103">Получение Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="8b07d-103">Get tokenLifetimePolicy</span></span>

<span data-ttu-id="8b07d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b07d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b07d-105">Получение свойств и связей объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8b07d-105">Retrieve the properties and relationships of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b07d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b07d-106">Permissions</span></span>

<span data-ttu-id="8b07d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b07d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b07d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b07d-109">Permission type</span></span>                        | <span data-ttu-id="8b07d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b07d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b07d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b07d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b07d-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8b07d-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8b07d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b07d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b07d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b07d-114">Not supported.</span></span> |
| <span data-ttu-id="8b07d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b07d-115">Application</span></span>                            | <span data-ttu-id="8b07d-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8b07d-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b07d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b07d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b07d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8b07d-118">Optional query parameters</span></span>

<span data-ttu-id="8b07d-119">Этот метод поддерживает `$expand` `$select` параметры запросов OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8b07d-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="8b07d-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8b07d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="8b07d-121">При использовании `$expand` Убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="8b07d-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b07d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b07d-122">Request headers</span></span>

| <span data-ttu-id="8b07d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8b07d-123">Name</span></span>      |<span data-ttu-id="8b07d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8b07d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b07d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b07d-125">Authorization</span></span> | <span data-ttu-id="8b07d-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8b07d-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b07d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b07d-127">Request body</span></span>

<span data-ttu-id="8b07d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b07d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b07d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b07d-129">Response</span></span>

<span data-ttu-id="8b07d-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b07d-130">If successful, this method returns a `200 OK` response code and the requested [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b07d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b07d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b07d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b07d-132">Request</span></span>

<span data-ttu-id="8b07d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b07d-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b07d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b07d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="8b07d-135">C#</span><span class="sxs-lookup"><span data-stu-id="8b07d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b07d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b07d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b07d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b07d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8b07d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b07d-138">Response</span></span>

<span data-ttu-id="8b07d-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b07d-139">The following is an example of the response.</span></span>

> <span data-ttu-id="8b07d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b07d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Get tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


