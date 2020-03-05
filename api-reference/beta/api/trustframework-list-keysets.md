---
title: Список Кэйсетс
description: Получение списка объектов трустфрамеворккэйсет.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d93da5c97be055b96f02bcddcc0a99e751084fa4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452206"
---
# <a name="list-keysets"></a><span data-ttu-id="a3a67-103">Список Кэйсетс</span><span class="sxs-lookup"><span data-stu-id="a3a67-103">List keySets</span></span>

<span data-ttu-id="a3a67-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a3a67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3a67-105">Получение списка [трустфрамеворккэйсетс](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="a3a67-105">Retrieve a list of [trustFrameworkKeySets](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a3a67-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3a67-106">Permissions</span></span>

<span data-ttu-id="a3a67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3a67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3a67-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3a67-109">Permission type</span></span>                        | <span data-ttu-id="a3a67-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3a67-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a3a67-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3a67-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3a67-112">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a3a67-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="a3a67-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3a67-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3a67-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3a67-114">Not supported.</span></span> |
| <span data-ttu-id="a3a67-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3a67-115">Application</span></span>                            | <span data-ttu-id="a3a67-116">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a3a67-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3a67-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3a67-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="a3a67-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3a67-118">Request headers</span></span>

| <span data-ttu-id="a3a67-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a3a67-119">Name</span></span>      |<span data-ttu-id="a3a67-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a3a67-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a3a67-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3a67-121">Authorization</span></span> | <span data-ttu-id="a3a67-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3a67-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3a67-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3a67-124">Request body</span></span>

<span data-ttu-id="a3a67-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3a67-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3a67-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3a67-126">Response</span></span>

<span data-ttu-id="a3a67-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3a67-127">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3a67-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a3a67-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3a67-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3a67-129">Request</span></span>

<span data-ttu-id="a3a67-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3a67-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3a67-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3a67-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_keysets"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets
```
# <a name="c"></a>[<span data-ttu-id="a3a67-132">C#</span><span class="sxs-lookup"><span data-stu-id="a3a67-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-keysets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3a67-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3a67-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-keysets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3a67-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3a67-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-keysets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a3a67-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3a67-135">Response</span></span>

<span data-ttu-id="a3a67-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a3a67-136">The following is an example of the response.</span></span>

> <span data-ttu-id="a3a67-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3a67-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
