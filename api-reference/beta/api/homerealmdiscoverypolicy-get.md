---
title: Получение Хомереалмдисковериполици
description: Получение свойств и связей объекта Хомереалмдисковериполици.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 569ecd0c645f5472d52916cb787ffd1b82371b6a
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916536"
---
# <a name="get-homerealmdiscoverypolicy"></a><span data-ttu-id="5a28f-103">Получение Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="5a28f-103">Get homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="5a28f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a28f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a28f-105">Получение свойств и связей объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="5a28f-105">Retrieve the properties and relationships of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a28f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a28f-106">Permissions</span></span>

<span data-ttu-id="5a28f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a28f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a28f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a28f-109">Permission type</span></span>                        | <span data-ttu-id="5a28f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a28f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5a28f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a28f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a28f-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5a28f-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="5a28f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a28f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a28f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a28f-114">Not supported.</span></span> |
| <span data-ttu-id="5a28f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a28f-115">Application</span></span>                            | <span data-ttu-id="5a28f-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5a28f-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a28f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a28f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a28f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5a28f-118">Optional query parameters</span></span>

<span data-ttu-id="5a28f-119">Этот метод поддерживает параметры `$expand` запросов `$select` OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5a28f-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="5a28f-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5a28f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="5a28f-121">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="5a28f-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a28f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a28f-122">Request headers</span></span>

| <span data-ttu-id="5a28f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="5a28f-123">Name</span></span>      |<span data-ttu-id="5a28f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5a28f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a28f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a28f-125">Authorization</span></span> | <span data-ttu-id="5a28f-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="5a28f-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a28f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a28f-127">Request body</span></span>

<span data-ttu-id="5a28f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a28f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a28f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a28f-129">Response</span></span>

<span data-ttu-id="5a28f-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a28f-130">If successful, this method returns a `200 OK` response code and the requested [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a28f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5a28f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a28f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a28f-132">Request</span></span>

<span data-ttu-id="5a28f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a28f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5a28f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a28f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="5a28f-135">C#</span><span class="sxs-lookup"><span data-stu-id="5a28f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a28f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a28f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a28f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a28f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5a28f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a28f-138">Response</span></span>

<span data-ttu-id="5a28f-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5a28f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="5a28f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a28f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
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
  "description": "Get homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
