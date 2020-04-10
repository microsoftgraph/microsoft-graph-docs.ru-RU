---
title: Создание Трустфрамеворккэйсет
description: Создание нового объекта **трустфрамеворккэйсет** .
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 934a3c7bbcd0e76bc41eac0294e0660ea9da3ccc
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215961"
---
# <a name="create-trustframeworkkeyset"></a><span data-ttu-id="4182a-103">Создание Трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="4182a-103">Create trustFrameworkKeySet</span></span>

<span data-ttu-id="4182a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4182a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4182a-105">Создание нового [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="4182a-105">Create a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="4182a-106">В запросе на создание должен быть указан идентификатор **трустфрамеворккэйсет** ; Тем не менее, она может быть изменена службой.</span><span class="sxs-lookup"><span data-stu-id="4182a-106">The ID of the **trustFrameworkKeySet** is expected in the create request; however, it can be modified by the service.</span></span> <span data-ttu-id="4182a-107">Измененный идентификатор будет доступен в ответе и в заголовке Location.</span><span class="sxs-lookup"><span data-stu-id="4182a-107">The modified ID will be available in the response and in the location header.</span></span>

## <a name="permissions"></a><span data-ttu-id="4182a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4182a-108">Permissions</span></span>

<span data-ttu-id="4182a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4182a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4182a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4182a-111">Permission type</span></span>                        | <span data-ttu-id="4182a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4182a-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4182a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4182a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4182a-114">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4182a-114">TrustFrameworkKeySet.ReadWrite.All</span></span>   |
| <span data-ttu-id="4182a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4182a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4182a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4182a-116">Not supported.</span></span> |
| <span data-ttu-id="4182a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4182a-117">Application</span></span>                            | <span data-ttu-id="4182a-118">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4182a-118">TrustFrameworkKeySet.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="4182a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4182a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="4182a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4182a-120">Request headers</span></span>

| <span data-ttu-id="4182a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4182a-121">Name</span></span>          | <span data-ttu-id="4182a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4182a-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4182a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4182a-123">Authorization</span></span> | <span data-ttu-id="4182a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4182a-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="4182a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4182a-126">Content-type</span></span> | <span data-ttu-id="4182a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4182a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4182a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4182a-129">Request body</span></span>

<span data-ttu-id="4182a-130">В тексте запроса добавьте представление объекта [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4182a-130">In the request body, supply a JSON representation of a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4182a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4182a-131">Response</span></span>

<span data-ttu-id="4182a-132">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, заголовок расположения для нового объекта и новый объект [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4182a-132">If successful, this method returns a `201 Created` response code, a location header for the newly created object, and a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4182a-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="4182a-133">Examples</span></span>

### <a name="example-1-create-an-empty-keyset"></a><span data-ttu-id="4182a-134">Пример 1: создание пустого набора ключей</span><span class="sxs-lookup"><span data-stu-id="4182a-134">Example 1: Create an empty keyset</span></span>
<span data-ttu-id="4182a-135">Это одна из наиболее эффективных операций.</span><span class="sxs-lookup"><span data-stu-id="4182a-135">This is one of the most useful operations.</span></span> <span data-ttu-id="4182a-136">Сначала необходимо создать пустой набор ключей.</span><span class="sxs-lookup"><span data-stu-id="4182a-136">First, you create an empty keyset.</span></span> <span data-ttu-id="4182a-137">Затем в новом наборе ключей можно создать ключ, отправить секрет вручную и отправить сертификат или ключ PKCS12.</span><span class="sxs-lookup"><span data-stu-id="4182a-137">Then, in the new keyset, you can generate a key, upload a manual secret, and upload a certificate or a PKCS12 key.</span></span> 

#### <a name="request"></a><span data-ttu-id="4182a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="4182a-138">Request</span></span>

<span data-ttu-id="4182a-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4182a-139">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4182a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="4182a-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4182a-141">C#</span><span class="sxs-lookup"><span data-stu-id="4182a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-trustframeworkkeyset-from-trustframework-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4182a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4182a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-trustframeworkkeyset-from-trustframework-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4182a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4182a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-trustframeworkkeyset-from-trustframework-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4182a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4182a-144">Response</span></span>

<span data-ttu-id="4182a-145">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4182a-145">The following example shows the response.</span></span>

> <span data-ttu-id="4182a-p106">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4182a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-keyset-with-a-key"></a><span data-ttu-id="4182a-148">Пример 2: создание набора ключей с ключом</span><span class="sxs-lookup"><span data-stu-id="4182a-148">Example 2: Create a keyset with a key</span></span>

<span data-ttu-id="4182a-149">Это расширенный сценарий, в котором необходимо знать формат ключа JSON, совместимый с [RFC 7517](https://tools.ietf.org/html/rfc7517#section-5) , для ключа.</span><span class="sxs-lookup"><span data-stu-id="4182a-149">This is an advanced scenario where you need to know the [RFC 7517](https://tools.ietf.org/html/rfc7517#section-5) compliant JSON Web Key format of the key.</span></span>

#### <a name="request"></a><span data-ttu-id="4182a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="4182a-150">Request</span></span>

<span data-ttu-id="4182a-151">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4182a-151">The following example shows the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="4182a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="4182a-152">Response</span></span>

<span data-ttu-id="4182a-153">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4182a-153">The following example shows the response.</span></span>

> <span data-ttu-id="4182a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4182a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
