---
title: Перечисление типов ресурсов tokenLifetimePolicy
description: Получите список объектов tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3d1566bf122d0400e979789049e7cbec1a45622c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439991"
---
# <a name="list-tokenlifetimepolicies"></a><span data-ttu-id="8c66c-103">Перечисление типов ресурсов tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="8c66c-103">List tokenLifetimePolicies</span></span>

<span data-ttu-id="8c66c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c66c-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="8c66c-105">Получите список [объектов tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c66c-105">Get a list of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c66c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c66c-106">Permissions</span></span>

<span data-ttu-id="8c66c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c66c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c66c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c66c-109">Permission type</span></span>                        | <span data-ttu-id="8c66c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c66c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8c66c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c66c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c66c-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c66c-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8c66c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c66c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c66c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c66c-114">Not supported.</span></span> |
| <span data-ttu-id="8c66c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c66c-115">Application</span></span>                            | <span data-ttu-id="8c66c-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c66c-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c66c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c66c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenLifetimePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c66c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c66c-118">Optional query parameters</span></span>

<span data-ttu-id="8c66c-119">Этот метод поддерживает параметры `$expand` `$filter` запроса `$select` OData и OData для настройки `$top` ответа.</span><span class="sxs-lookup"><span data-stu-id="8c66c-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="8c66c-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8c66c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="8c66c-121">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="8c66c-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c66c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c66c-122">Request headers</span></span>

| <span data-ttu-id="8c66c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8c66c-123">Name</span></span>      |<span data-ttu-id="8c66c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8c66c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c66c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c66c-125">Authorization</span></span> | <span data-ttu-id="8c66c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c66c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c66c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c66c-128">Request body</span></span>

<span data-ttu-id="8c66c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c66c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c66c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c66c-130">Response</span></span>

<span data-ttu-id="8c66c-131">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` [объектов tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8c66c-131">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c66c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c66c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c66c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c66c-133">Request</span></span>

<span data-ttu-id="8c66c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c66c-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8c66c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c66c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="8c66c-136">C#</span><span class="sxs-lookup"><span data-stu-id="8c66c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c66c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c66c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c66c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c66c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c66c-139">Java</span><span class="sxs-lookup"><span data-stu-id="8c66c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tokenlifetimepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c66c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c66c-140">Response</span></span>

<span data-ttu-id="8c66c-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c66c-141">The following is an example of the response.</span></span>

> <span data-ttu-id="8c66c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c66c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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
  "description": "List tokenLifetimePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

