---
title: Список Кэйсетс
description: Получение списка объектов трустфрамеворккэйсет.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e824e9a677c9749a1956900908a46409c969c0c7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971872"
---
# <a name="list-keysets"></a><span data-ttu-id="89c52-103">Список Кэйсетс</span><span class="sxs-lookup"><span data-stu-id="89c52-103">List keySets</span></span>

<span data-ttu-id="89c52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89c52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89c52-105">Получение списка [трустфрамеворккэйсетс](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="89c52-105">Retrieve a list of [trustFrameworkKeySets](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="89c52-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89c52-106">Permissions</span></span>

<span data-ttu-id="89c52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89c52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89c52-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89c52-109">Permission type</span></span>                        | <span data-ttu-id="89c52-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89c52-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89c52-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89c52-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="89c52-112">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="89c52-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="89c52-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89c52-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89c52-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89c52-114">Not supported.</span></span> |
| <span data-ttu-id="89c52-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="89c52-115">Application</span></span>                            | <span data-ttu-id="89c52-116">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="89c52-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89c52-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89c52-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="89c52-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89c52-118">Request headers</span></span>

| <span data-ttu-id="89c52-119">Имя</span><span class="sxs-lookup"><span data-stu-id="89c52-119">Name</span></span>      |<span data-ttu-id="89c52-120">Описание</span><span class="sxs-lookup"><span data-stu-id="89c52-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="89c52-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89c52-121">Authorization</span></span> | <span data-ttu-id="89c52-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89c52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89c52-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89c52-124">Request body</span></span>

<span data-ttu-id="89c52-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89c52-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89c52-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="89c52-126">Response</span></span>

<span data-ttu-id="89c52-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89c52-127">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89c52-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="89c52-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89c52-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="89c52-129">Request</span></span>

<span data-ttu-id="89c52-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89c52-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89c52-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="89c52-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_keysets"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets
```
# <a name="c"></a>[<span data-ttu-id="89c52-132">C#</span><span class="sxs-lookup"><span data-stu-id="89c52-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-keysets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89c52-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89c52-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-keysets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89c52-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89c52-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-keysets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89c52-135">Java</span><span class="sxs-lookup"><span data-stu-id="89c52-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-keysets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89c52-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="89c52-136">Response</span></span>

<span data-ttu-id="89c52-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89c52-137">The following is an example of the response.</span></span>

> <span data-ttu-id="89c52-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89c52-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "keys": [
        {
          "k": "k-value",
          "x5c": [
            "x5c-value"
          ],
          "x5t": "x5t-value",
          "kty": "kty-value",
          "use": "use-value",
          "exp": 99,
          "nbf": 99,
          "kid": "kid-value",
          "e": "e-value",
          "n": "n-value",
          "d": "d-value",
          "p": "p-value",
          "q": "q-value",
          "dp": "dp-value",
          "dq": "dq-value",
          "qi": "qi-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List keySets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


