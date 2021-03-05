---
title: Get tokenIssuancePolicy
description: Извлечение свойств и связей объекта tokenIssuancePolicy.
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ecfb5f435a3d8c14ba54a7a1e8c54bf60ab17bd1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449000"
---
# <a name="get-tokenissuancepolicy"></a><span data-ttu-id="5ba1f-103">Get tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="5ba1f-103">Get tokenIssuancePolicy</span></span>

<span data-ttu-id="5ba1f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ba1f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="5ba1f-105">Извлечение свойств и связей объекта [tokenIssuancePolicy.](../resources/tokenIssuancePolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5ba1f-105">Retrieve the properties and relationships of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ba1f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ba1f-106">Permissions</span></span>

<span data-ttu-id="5ba1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ba1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ba1f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ba1f-109">Permission type</span></span>                        | <span data-ttu-id="5ba1f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ba1f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5ba1f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ba1f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ba1f-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ba1f-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="5ba1f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ba1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ba1f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-114">Not supported.</span></span> |
| <span data-ttu-id="5ba1f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ba1f-115">Application</span></span>                            | <span data-ttu-id="5ba1f-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ba1f-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ba1f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ba1f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ba1f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5ba1f-118">Optional query parameters</span></span>

<span data-ttu-id="5ba1f-119">Этот метод поддерживает параметры `$expand` `$select` запроса oData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="5ba1f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5ba1f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="5ba1f-121">При использовании убедитесь, что ваше приложение запрашивает `$expand` разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ba1f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ba1f-122">Request headers</span></span>

| <span data-ttu-id="5ba1f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="5ba1f-123">Name</span></span>      |<span data-ttu-id="5ba1f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5ba1f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ba1f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ba1f-125">Authorization</span></span> | <span data-ttu-id="5ba1f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ba1f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ba1f-128">Request body</span></span>

<span data-ttu-id="5ba1f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ba1f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ba1f-130">Response</span></span>

<span data-ttu-id="5ba1f-131">В случае успешной работы этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-131">If successful, this method returns a `200 OK` response code and the requested [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ba1f-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="5ba1f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ba1f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ba1f-133">Request</span></span>

<span data-ttu-id="5ba1f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5ba1f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ba1f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenIssuancePolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancepolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="5ba1f-136">C#</span><span class="sxs-lookup"><span data-stu-id="5ba1f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ba1f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ba1f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ba1f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ba1f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ba1f-139">Java</span><span class="sxs-lookup"><span data-stu-id="5ba1f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tokenissuancepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5ba1f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ba1f-140">Response</span></span>

<span data-ttu-id="5ba1f-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-141">The following is an example of the response.</span></span>

> <span data-ttu-id="5ba1f-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
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
  "description": "Get tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

