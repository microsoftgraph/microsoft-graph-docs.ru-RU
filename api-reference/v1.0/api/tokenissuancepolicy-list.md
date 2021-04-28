---
title: List tokenIssuancePolicy
description: Получите список объектов tokenIssuancePolicy.
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 693579c25c7e96ccbdfceecee44791ba23ffeefa
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054345"
---
# <a name="list-tokenissuancepolicy"></a><span data-ttu-id="ecc77-103">List tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="ecc77-103">List tokenIssuancePolicy</span></span>

<span data-ttu-id="ecc77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecc77-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ecc77-105">Получите список [объектов tokenIssuancePolicy.](../resources/tokenIssuancePolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ecc77-105">Get a list of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecc77-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecc77-106">Permissions</span></span>

<span data-ttu-id="ecc77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecc77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ecc77-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecc77-109">Permission type</span></span>                        | <span data-ttu-id="ecc77-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecc77-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ecc77-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecc77-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ecc77-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ecc77-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="ecc77-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecc77-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecc77-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecc77-114">Not supported.</span></span> |
| <span data-ttu-id="ecc77-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecc77-115">Application</span></span>                            | <span data-ttu-id="ecc77-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ecc77-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecc77-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecc77-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenIssuancePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecc77-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ecc77-118">Optional query parameters</span></span>

<span data-ttu-id="ecc77-119">Этот метод поддерживает `$expand` параметры `$filter` запросов , и `$select` OData, чтобы помочь `$top` настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="ecc77-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ecc77-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ecc77-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="ecc77-121">При использовании убедитесь, что ваше приложение запрашивает `$expand` разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="ecc77-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecc77-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecc77-122">Request headers</span></span>

| <span data-ttu-id="ecc77-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ecc77-123">Name</span></span>      |<span data-ttu-id="ecc77-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ecc77-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ecc77-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecc77-125">Authorization</span></span> | <span data-ttu-id="ecc77-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecc77-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecc77-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecc77-128">Request body</span></span>

<span data-ttu-id="ecc77-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ecc77-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecc77-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecc77-130">Response</span></span>

<span data-ttu-id="ecc77-131">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ecc77-131">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecc77-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="ecc77-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ecc77-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecc77-133">Request</span></span>

<span data-ttu-id="ecc77-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecc77-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ecc77-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecc77-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tokenIssuancePolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="ecc77-136">C#</span><span class="sxs-lookup"><span data-stu-id="ecc77-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tokenissuancepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecc77-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecc77-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tokenissuancepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecc77-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecc77-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tokenissuancepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecc77-139">Java</span><span class="sxs-lookup"><span data-stu-id="ecc77-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tokenissuancepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ecc77-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecc77-140">Response</span></span>

<span data-ttu-id="ecc77-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ecc77-141">The following is an example of the response.</span></span>

> <span data-ttu-id="ecc77-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ecc77-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
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
  "description": "List tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

