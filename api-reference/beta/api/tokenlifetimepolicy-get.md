---
title: Get tokenLifetimePolicy
description: Извлечение свойств и связей объекта tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ed80eaa28738dd367ba7762e1fabf4f28adf29e6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051783"
---
# <a name="get-tokenlifetimepolicy"></a><span data-ttu-id="2a927-103">Get tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="2a927-103">Get tokenLifetimePolicy</span></span>

<span data-ttu-id="2a927-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a927-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a927-105">Извлечение свойств и связей объекта [tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2a927-105">Retrieve the properties and relationships of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a927-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a927-106">Permissions</span></span>

<span data-ttu-id="2a927-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a927-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a927-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a927-109">Permission type</span></span>                        | <span data-ttu-id="2a927-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a927-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2a927-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a927-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a927-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a927-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="2a927-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a927-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a927-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a927-114">Not supported.</span></span> |
| <span data-ttu-id="2a927-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2a927-115">Application</span></span>                            | <span data-ttu-id="2a927-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a927-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a927-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a927-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a927-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2a927-118">Optional query parameters</span></span>

<span data-ttu-id="2a927-119">Этот метод поддерживает параметры `$expand` `$select` запроса oData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2a927-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="2a927-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2a927-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="2a927-121">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="2a927-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a927-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a927-122">Request headers</span></span>

| <span data-ttu-id="2a927-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2a927-123">Name</span></span>      |<span data-ttu-id="2a927-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2a927-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2a927-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a927-125">Authorization</span></span> | <span data-ttu-id="2a927-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="2a927-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a927-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a927-127">Request body</span></span>

<span data-ttu-id="2a927-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a927-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a927-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a927-129">Response</span></span>

<span data-ttu-id="2a927-130">В случае успешной работы этот метод возвращает код отклика и запрашиваемого `200 OK` [объекта tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2a927-130">If successful, this method returns a `200 OK` response code and the requested [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a927-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a927-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a927-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a927-132">Request</span></span>

<span data-ttu-id="2a927-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a927-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a927-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a927-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="2a927-135">C#</span><span class="sxs-lookup"><span data-stu-id="2a927-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a927-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a927-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a927-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a927-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a927-138">Java</span><span class="sxs-lookup"><span data-stu-id="2a927-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tokenlifetimepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2a927-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a927-139">Response</span></span>

<span data-ttu-id="2a927-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2a927-140">The following is an example of the response.</span></span>

> <span data-ttu-id="2a927-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2a927-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


