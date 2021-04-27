---
title: Обновление trustFrameworkKeySet
description: Обновление свойств объекта **trustFrameworkKeySet.**
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c0375dbb052c061330d26120783f69d4a8327440
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053435"
---
# <a name="update-trustframeworkkeyset"></a><span data-ttu-id="9e7ba-103">Обновление trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="9e7ba-103">Update trustFrameworkKeySet</span></span>

<span data-ttu-id="9e7ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e7ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e7ba-105">Обновление свойств [trustFrameworkKeyset.](../resources/trustframeworkkeyset.md)</span><span class="sxs-lookup"><span data-stu-id="9e7ba-105">Update the properties of a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="9e7ba-106">Эта операция заменит содержимое существующего наборов ключей.</span><span class="sxs-lookup"><span data-stu-id="9e7ba-106">This operation will replace the content of an existing keyset.</span></span> <span data-ttu-id="9e7ba-107">Указание ID в полезной нагрузке запроса является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9e7ba-107">Specifying the ID in the request payload is optional.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e7ba-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e7ba-108">Permissions</span></span>

<span data-ttu-id="9e7ba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e7ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e7ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e7ba-111">Permission type</span></span>                        | <span data-ttu-id="9e7ba-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e7ba-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9e7ba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e7ba-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e7ba-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e7ba-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="9e7ba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e7ba-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e7ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e7ba-116">Not supported.</span></span> |
| <span data-ttu-id="9e7ba-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9e7ba-117">Application</span></span>                            | <span data-ttu-id="9e7ba-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e7ba-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e7ba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e7ba-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9e7ba-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e7ba-120">Request headers</span></span>

| <span data-ttu-id="9e7ba-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9e7ba-121">Name</span></span>       | <span data-ttu-id="9e7ba-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9e7ba-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9e7ba-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e7ba-123">Authorization</span></span> | <span data-ttu-id="9e7ba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e7ba-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9e7ba-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e7ba-126">Content-type</span></span>  | <span data-ttu-id="9e7ba-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e7ba-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e7ba-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e7ba-129">Request body</span></span>


| <span data-ttu-id="9e7ba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e7ba-130">Property</span></span>     | <span data-ttu-id="9e7ba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9e7ba-131">Type</span></span>        | <span data-ttu-id="9e7ba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9e7ba-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e7ba-133">клавиши</span><span class="sxs-lookup"><span data-stu-id="9e7ba-133">keys</span></span>|<span data-ttu-id="9e7ba-134">[коллекция trustFrameworkKey](../resources/trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="9e7ba-134">[trustFrameworkKey](../resources/trustframeworkkey.md) collection</span></span>| <span data-ttu-id="9e7ba-135">обновляет коллекцию Trustframeworkkeys</span><span class="sxs-lookup"><span data-stu-id="9e7ba-135">updates a collection of Trustframeworkkeys</span></span>|

## <a name="response"></a><span data-ttu-id="9e7ba-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e7ba-136">Response</span></span>

<span data-ttu-id="9e7ba-137">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект trustFrameworkKeySet](../resources/trustframeworkkeyset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9e7ba-137">If successful, this method returns a `200 OK` response code and an updated [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e7ba-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="9e7ba-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e7ba-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e7ba-139">Request</span></span>

<span data-ttu-id="9e7ba-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e7ba-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e7ba-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e7ba-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9e7ba-142">C#</span><span class="sxs-lookup"><span data-stu-id="9e7ba-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e7ba-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e7ba-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e7ba-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e7ba-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e7ba-145">Java</span><span class="sxs-lookup"><span data-stu-id="9e7ba-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-trustframeworkkeyset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9e7ba-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e7ba-146">Response</span></span>

<span data-ttu-id="9e7ba-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9e7ba-147">The following is an example of the response.</span></span>

> <span data-ttu-id="9e7ba-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9e7ba-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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


