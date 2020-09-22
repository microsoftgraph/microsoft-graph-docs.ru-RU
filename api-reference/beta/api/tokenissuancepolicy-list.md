---
title: Список Токениссуанцеполици
description: Получение списка объектов Токениссуанцеполици.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 70b0e7875a2634f6f06cea2de9bc2bf0a10ab348
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074023"
---
# <a name="list-tokenissuancepolicy"></a><span data-ttu-id="dedd6-103">Список Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="dedd6-103">List tokenIssuancePolicy</span></span>

<span data-ttu-id="dedd6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dedd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dedd6-105">Получение списка объектов [токениссуанцеполици](../resources/tokenIssuancePolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="dedd6-105">Get a list of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="dedd6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dedd6-106">Permissions</span></span>

<span data-ttu-id="dedd6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dedd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dedd6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dedd6-109">Permission type</span></span>                        | <span data-ttu-id="dedd6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dedd6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dedd6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dedd6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dedd6-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="dedd6-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="dedd6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dedd6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dedd6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dedd6-114">Not supported.</span></span> |
| <span data-ttu-id="dedd6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dedd6-115">Application</span></span>                            | <span data-ttu-id="dedd6-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="dedd6-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="dedd6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dedd6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenIssuancePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dedd6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dedd6-118">Optional query parameters</span></span>

<span data-ttu-id="dedd6-119">Этот метод поддерживает `$expand` `$filter` параметры запросов,, `$select` и `$top` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="dedd6-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="dedd6-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dedd6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="dedd6-121">При использовании `$expand` Убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="dedd6-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dedd6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dedd6-122">Request headers</span></span>

| <span data-ttu-id="dedd6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="dedd6-123">Name</span></span>      |<span data-ttu-id="dedd6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dedd6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dedd6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dedd6-125">Authorization</span></span> | <span data-ttu-id="dedd6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dedd6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dedd6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dedd6-128">Request body</span></span>

<span data-ttu-id="dedd6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dedd6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dedd6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="dedd6-130">Response</span></span>

<span data-ttu-id="dedd6-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [токениссуанцеполици](../resources/tokenIssuancePolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dedd6-131">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dedd6-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="dedd6-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dedd6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dedd6-133">Request</span></span>

<span data-ttu-id="dedd6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dedd6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dedd6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dedd6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tokenIssuancePolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="dedd6-136">C#</span><span class="sxs-lookup"><span data-stu-id="dedd6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tokenissuancepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dedd6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dedd6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tokenissuancepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dedd6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dedd6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tokenissuancepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="dedd6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dedd6-139">Response</span></span>

<span data-ttu-id="dedd6-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dedd6-140">The following is an example of the response.</span></span>

> <span data-ttu-id="dedd6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dedd6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


