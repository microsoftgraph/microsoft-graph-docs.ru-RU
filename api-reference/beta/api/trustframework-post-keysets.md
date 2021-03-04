---
title: Создание trustFrameworkKeySet
description: Создайте новый **объект trustFrameworkKeySet.**
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c4295de0e6a6e361a28932fa4755b35aca80b64b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444986"
---
# <a name="create-trustframeworkkeyset"></a><span data-ttu-id="89deb-103">Создание trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="89deb-103">Create trustFrameworkKeySet</span></span>

<span data-ttu-id="89deb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89deb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89deb-105">Создание нового [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="89deb-105">Create a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="89deb-106">В запросе на создание ожидается ID **trustFrameworkKeySet;** однако службой она может быть изменена.</span><span class="sxs-lookup"><span data-stu-id="89deb-106">The ID of the **trustFrameworkKeySet** is expected in the create request; however, it can be modified by the service.</span></span> <span data-ttu-id="89deb-107">Измененный ID будет доступен в ответе и в загоне расположения.</span><span class="sxs-lookup"><span data-stu-id="89deb-107">The modified ID will be available in the response and in the location header.</span></span>

## <a name="permissions"></a><span data-ttu-id="89deb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89deb-108">Permissions</span></span>

<span data-ttu-id="89deb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89deb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89deb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89deb-111">Permission type</span></span>                        | <span data-ttu-id="89deb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89deb-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89deb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89deb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="89deb-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89deb-114">TrustFrameworkKeySet.ReadWrite.All</span></span>   |
| <span data-ttu-id="89deb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89deb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89deb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89deb-116">Not supported.</span></span> |
| <span data-ttu-id="89deb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="89deb-117">Application</span></span>                            | <span data-ttu-id="89deb-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89deb-118">TrustFrameworkKeySet.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="89deb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89deb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="89deb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89deb-120">Request headers</span></span>

| <span data-ttu-id="89deb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="89deb-121">Name</span></span>          | <span data-ttu-id="89deb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="89deb-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="89deb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89deb-123">Authorization</span></span> | <span data-ttu-id="89deb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89deb-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="89deb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89deb-126">Content-type</span></span> | <span data-ttu-id="89deb-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89deb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89deb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89deb-129">Request body</span></span>

<span data-ttu-id="89deb-130">В теле запроса подарйте JSON представление объекта [trustFrameworkKeySet.](../resources/trustframeworkkeyset.md)</span><span class="sxs-lookup"><span data-stu-id="89deb-130">In the request body, supply a JSON representation of a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="89deb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="89deb-131">Response</span></span>

<span data-ttu-id="89deb-132">В случае успешной работы этот метод возвращает код отклика, заголовку расположения для вновь созданного объекта и новый объект `201 Created` [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="89deb-132">If successful, this method returns a `201 Created` response code, a location header for the newly created object, and a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89deb-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="89deb-133">Examples</span></span>

### <a name="example-1-create-an-empty-keyset"></a><span data-ttu-id="89deb-134">Пример 1. Создание пустого наборов ключей</span><span class="sxs-lookup"><span data-stu-id="89deb-134">Example 1: Create an empty keyset</span></span>
<span data-ttu-id="89deb-135">Это одна из самых полезных операций.</span><span class="sxs-lookup"><span data-stu-id="89deb-135">This is one of the most useful operations.</span></span> <span data-ttu-id="89deb-136">Сначала создается пустой набор ключей.</span><span class="sxs-lookup"><span data-stu-id="89deb-136">First, you create an empty keyset.</span></span> <span data-ttu-id="89deb-137">Затем в новом наборе ключей можно создать ключ, загрузить секрет вручную и загрузить сертификат или ключ PKCS12.</span><span class="sxs-lookup"><span data-stu-id="89deb-137">Then, in the new keyset, you can generate a key, upload a manual secret, and upload a certificate or a PKCS12 key.</span></span> 

#### <a name="request"></a><span data-ttu-id="89deb-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="89deb-138">Request</span></span>

<span data-ttu-id="89deb-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89deb-139">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89deb-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="89deb-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_trustframework1"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets
Content-type: application/json

{
  "id": "keyset1"  
}
```
# <a name="c"></a>[<span data-ttu-id="89deb-141">C#</span><span class="sxs-lookup"><span data-stu-id="89deb-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-trustframeworkkeyset-from-trustframework-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89deb-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89deb-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-trustframeworkkeyset-from-trustframework-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89deb-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89deb-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-trustframeworkkeyset-from-trustframework-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89deb-144">Java</span><span class="sxs-lookup"><span data-stu-id="89deb-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-trustframeworkkeyset-from-trustframework-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89deb-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="89deb-145">Response</span></span>

<span data-ttu-id="89deb-146">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89deb-146">The following example shows the response.</span></span>

> <span data-ttu-id="89deb-p106">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89deb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Location: /trustFramework/keySets('B2C_1A_keyset1')

{
  "id": "B2C_1A_keyset1",
  "keys": []
}
```

### <a name="example-2-create-a-keyset-with-a-key"></a><span data-ttu-id="89deb-149">Пример 2. Создание наборов ключей с ключом</span><span class="sxs-lookup"><span data-stu-id="89deb-149">Example 2: Create a keyset with a key</span></span>

<span data-ttu-id="89deb-150">Это расширенный сценарий, в котором необходимо знать формат ключа JSON Web Key, совместимый с [RFC 7517.](https://tools.ietf.org/html/rfc7517#section-5)</span><span class="sxs-lookup"><span data-stu-id="89deb-150">This is an advanced scenario where you need to know the [RFC 7517](https://tools.ietf.org/html/rfc7517#section-5) compliant JSON Web Key format of the key.</span></span>

#### <a name="request"></a><span data-ttu-id="89deb-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="89deb-151">Request</span></span>

<span data-ttu-id="89deb-152">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89deb-152">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_trustframework"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets
Content-type: application/json

{
  "id": "keyset1",
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

#### <a name="response"></a><span data-ttu-id="89deb-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="89deb-153">Response</span></span>

<span data-ttu-id="89deb-154">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89deb-154">The following example shows the response.</span></span>

> <span data-ttu-id="89deb-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89deb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Location: /trustFramework/keySets('B2C_1A_keyset1')

{
  "id": "B2C_1A_keyset1",
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
  "description": "Create trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


