---
title: Обновление Трустфрамеворккэйсет
description: Обновление свойств объекта **трустфрамеворккэйсет** .
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f78bde00aee45dedc6d55d765aead8331605f0f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938237"
---
# <a name="update-trustframeworkkeyset"></a><span data-ttu-id="20dfe-103">Обновление Трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="20dfe-103">Update trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20dfe-104">Обновление свойств объекта [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="20dfe-104">Update the properties of a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="20dfe-105">Эта операция заменит содержимое существующего набора ключей.</span><span class="sxs-lookup"><span data-stu-id="20dfe-105">This operation will replace the content of an existing keyset.</span></span> <span data-ttu-id="20dfe-106">Указывать идентификатор в полезных данных запроса необязательно.</span><span class="sxs-lookup"><span data-stu-id="20dfe-106">Specifying the ID in the request payload is optional.</span></span>

## <a name="permissions"></a><span data-ttu-id="20dfe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20dfe-107">Permissions</span></span>

<span data-ttu-id="20dfe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20dfe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20dfe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20dfe-110">Permission type</span></span>                        | <span data-ttu-id="20dfe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20dfe-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="20dfe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20dfe-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="20dfe-113">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="20dfe-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="20dfe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20dfe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20dfe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20dfe-115">Not supported.</span></span> |
| <span data-ttu-id="20dfe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20dfe-116">Application</span></span>                            | <span data-ttu-id="20dfe-117">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="20dfe-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20dfe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20dfe-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="20dfe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20dfe-119">Request headers</span></span>

| <span data-ttu-id="20dfe-120">Имя</span><span class="sxs-lookup"><span data-stu-id="20dfe-120">Name</span></span>       | <span data-ttu-id="20dfe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="20dfe-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="20dfe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20dfe-122">Authorization</span></span> | <span data-ttu-id="20dfe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20dfe-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20dfe-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20dfe-125">Content-type</span></span>  | <span data-ttu-id="20dfe-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20dfe-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20dfe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20dfe-128">Request body</span></span>


| <span data-ttu-id="20dfe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="20dfe-129">Property</span></span>     | <span data-ttu-id="20dfe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="20dfe-130">Type</span></span>        | <span data-ttu-id="20dfe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="20dfe-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20dfe-132">переключен</span><span class="sxs-lookup"><span data-stu-id="20dfe-132">keys</span></span>|<span data-ttu-id="20dfe-133">Коллекция [трустфрамеворккэй](../resources/trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="20dfe-133">[trustFrameworkKey](../resources/trustframeworkkey.md) collection</span></span>| <span data-ttu-id="20dfe-134">Обновляет коллекцию Трустфрамеворккэйс</span><span class="sxs-lookup"><span data-stu-id="20dfe-134">updates a collection of Trustframeworkkeys</span></span>|

## <a name="response"></a><span data-ttu-id="20dfe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="20dfe-135">Response</span></span>

<span data-ttu-id="20dfe-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20dfe-136">If successful, this method returns a `200 OK` response code and an updated [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20dfe-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="20dfe-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20dfe-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="20dfe-138">Request</span></span>

<span data-ttu-id="20dfe-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20dfe-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="20dfe-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="20dfe-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_trustframeworkkeyset"
}-->

```http
PUT https://graph.microsoft.com/beta/trustFramework/keySets/{id}
Content-type: application/json

{
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
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="20dfe-141">C#</span><span class="sxs-lookup"><span data-stu-id="20dfe-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20dfe-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20dfe-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20dfe-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20dfe-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20dfe-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="20dfe-144">Response</span></span>

<span data-ttu-id="20dfe-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="20dfe-145">The following is an example of the response.</span></span>

> <span data-ttu-id="20dfe-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20dfe-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update trustframeworkkeyset",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
