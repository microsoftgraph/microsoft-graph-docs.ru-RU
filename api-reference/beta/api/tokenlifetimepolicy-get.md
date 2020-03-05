---
title: Получение Токенлифетимеполици
description: Получение свойств и связей объекта Токенлифетимеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0bbd72ebddb221bc7bc82e1676180048e57d9994
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452227"
---
# <a name="get-tokenlifetimepolicy"></a><span data-ttu-id="33efb-103">Получение Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="33efb-103">Get tokenLifetimePolicy</span></span>

<span data-ttu-id="33efb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="33efb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33efb-105">Получение свойств и связей объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="33efb-105">Retrieve the properties and relationships of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="33efb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33efb-106">Permissions</span></span>

<span data-ttu-id="33efb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33efb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33efb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33efb-109">Permission type</span></span>                        | <span data-ttu-id="33efb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33efb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="33efb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33efb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="33efb-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="33efb-112">Policy.Read.All</span></span> |
| <span data-ttu-id="33efb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33efb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33efb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33efb-114">Not supported.</span></span> |
| <span data-ttu-id="33efb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33efb-115">Application</span></span>                            | <span data-ttu-id="33efb-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="33efb-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33efb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33efb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33efb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="33efb-118">Optional query parameters</span></span>

<span data-ttu-id="33efb-119">Этот метод поддерживает параметры `$expand` запросов `$select` OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="33efb-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="33efb-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="33efb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="33efb-121">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="33efb-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33efb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33efb-122">Request headers</span></span>

| <span data-ttu-id="33efb-123">Имя</span><span class="sxs-lookup"><span data-stu-id="33efb-123">Name</span></span>      |<span data-ttu-id="33efb-124">Описание</span><span class="sxs-lookup"><span data-stu-id="33efb-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="33efb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="33efb-125">Authorization</span></span> | <span data-ttu-id="33efb-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="33efb-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="33efb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33efb-127">Request body</span></span>

<span data-ttu-id="33efb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33efb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33efb-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="33efb-129">Response</span></span>

<span data-ttu-id="33efb-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33efb-130">If successful, this method returns a `200 OK` response code and the requested [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33efb-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="33efb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="33efb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="33efb-132">Request</span></span>

<span data-ttu-id="33efb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33efb-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="33efb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="33efb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="33efb-135">C#</span><span class="sxs-lookup"><span data-stu-id="33efb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33efb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33efb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33efb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33efb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="33efb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="33efb-138">Response</span></span>

<span data-ttu-id="33efb-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33efb-139">The following is an example of the response.</span></span>

> <span data-ttu-id="33efb-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33efb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
