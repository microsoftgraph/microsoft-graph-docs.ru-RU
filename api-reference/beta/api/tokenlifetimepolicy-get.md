---
title: Get tokenLifetimePolicy
description: Извлечение свойств и связей объекта tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 00698245935b714ce6afb2fc400133d3c2c5b447
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443383"
---
# <a name="get-tokenlifetimepolicy"></a><span data-ttu-id="3834e-103">Get tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="3834e-103">Get tokenLifetimePolicy</span></span>

<span data-ttu-id="3834e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3834e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3834e-105">Извлечение свойств и связей объекта [tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3834e-105">Retrieve the properties and relationships of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3834e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3834e-106">Permissions</span></span>

<span data-ttu-id="3834e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3834e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3834e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3834e-109">Permission type</span></span>                        | <span data-ttu-id="3834e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3834e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3834e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3834e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3834e-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3834e-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="3834e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3834e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3834e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3834e-114">Not supported.</span></span> |
| <span data-ttu-id="3834e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3834e-115">Application</span></span>                            | <span data-ttu-id="3834e-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3834e-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="3834e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3834e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3834e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3834e-118">Optional query parameters</span></span>

<span data-ttu-id="3834e-119">Этот метод поддерживает параметры `$expand` `$select` запроса oData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3834e-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="3834e-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3834e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="3834e-121">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="3834e-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3834e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3834e-122">Request headers</span></span>

| <span data-ttu-id="3834e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3834e-123">Name</span></span>      |<span data-ttu-id="3834e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3834e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3834e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3834e-125">Authorization</span></span> | <span data-ttu-id="3834e-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="3834e-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3834e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3834e-127">Request body</span></span>

<span data-ttu-id="3834e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3834e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3834e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3834e-129">Response</span></span>

<span data-ttu-id="3834e-130">В случае успешной работы этот метод возвращает код отклика и запрашиваемого `200 OK` [объекта tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3834e-130">If successful, this method returns a `200 OK` response code and the requested [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3834e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="3834e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3834e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3834e-132">Request</span></span>

<span data-ttu-id="3834e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3834e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3834e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3834e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="3834e-135">C#</span><span class="sxs-lookup"><span data-stu-id="3834e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3834e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3834e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3834e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3834e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3834e-138">Java</span><span class="sxs-lookup"><span data-stu-id="3834e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tokenlifetimepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3834e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3834e-139">Response</span></span>

<span data-ttu-id="3834e-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3834e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="3834e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3834e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


