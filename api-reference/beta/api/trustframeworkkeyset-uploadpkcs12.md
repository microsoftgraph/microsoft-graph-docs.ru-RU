---
title: 'trustFrameworkKeySet: uploadPkcs12'
description: Upload клавишу формата PKCS 12 (PFX) в набор ключей.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 520508293c6336e5c5c1e715eeb4f02de9209b4e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053428"
---
# <a name="trustframeworkkeyset-uploadpkcs12"></a><span data-ttu-id="87813-103">trustFrameworkKeySet: uploadPkcs12</span><span class="sxs-lookup"><span data-stu-id="87813-103">trustFrameworkKeySet: uploadPkcs12</span></span>

<span data-ttu-id="87813-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87813-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87813-105">Upload PKCS12 формата (PFX) в [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="87813-105">Upload a PKCS12 format key (PFX) to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="87813-106">Входное значение — это закодированное значение содержимого сертификата Pfx.</span><span class="sxs-lookup"><span data-stu-id="87813-106">The input is a base-64 encoded value of the Pfx certificate contents.</span></span> <span data-ttu-id="87813-107">Этот метод возвращает [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="87813-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="87813-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87813-108">Permissions</span></span>

<span data-ttu-id="87813-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87813-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87813-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87813-111">Permission type</span></span>                        | <span data-ttu-id="87813-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87813-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="87813-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87813-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="87813-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87813-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="87813-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87813-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87813-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87813-116">Not supported.</span></span> |
| <span data-ttu-id="87813-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="87813-117">Application</span></span>                            | <span data-ttu-id="87813-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87813-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87813-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87813-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadPkcs12
```

## <a name="request-headers"></a><span data-ttu-id="87813-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87813-120">Request headers</span></span>

| <span data-ttu-id="87813-121">Имя</span><span class="sxs-lookup"><span data-stu-id="87813-121">Name</span></span>          | <span data-ttu-id="87813-122">Описание</span><span class="sxs-lookup"><span data-stu-id="87813-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="87813-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87813-123">Authorization</span></span> | <span data-ttu-id="87813-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87813-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87813-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="87813-126">Content-type</span></span>  | <span data-ttu-id="87813-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87813-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87813-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87813-129">Request body</span></span>

<span data-ttu-id="87813-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="87813-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="87813-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="87813-131">Parameter</span></span>    | <span data-ttu-id="87813-132">Тип</span><span class="sxs-lookup"><span data-stu-id="87813-132">Type</span></span>        | <span data-ttu-id="87813-133">Описание</span><span class="sxs-lookup"><span data-stu-id="87813-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87813-134">key</span><span class="sxs-lookup"><span data-stu-id="87813-134">key</span></span>|<span data-ttu-id="87813-135">String</span><span class="sxs-lookup"><span data-stu-id="87813-135">String</span></span>|<span data-ttu-id="87813-136">Это поле для отправки контента pfx.</span><span class="sxs-lookup"><span data-stu-id="87813-136">This is the field for sending pfx content.</span></span> <span data-ttu-id="87813-137">Значение должно быть кодированной версией базового-64 фактического контента сертификата.</span><span class="sxs-lookup"><span data-stu-id="87813-137">The value should be a base-64 encoded version of the actual certificate content.</span></span>|
|<span data-ttu-id="87813-138">password</span><span class="sxs-lookup"><span data-stu-id="87813-138">password</span></span>|<span data-ttu-id="87813-139">Строка</span><span class="sxs-lookup"><span data-stu-id="87813-139">String</span></span>|<span data-ttu-id="87813-140">Это поле для отправки пароля контенту PFX.</span><span class="sxs-lookup"><span data-stu-id="87813-140">This is the field for sending the password to PFX content.</span></span>|

## <a name="response"></a><span data-ttu-id="87813-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="87813-141">Response</span></span>

<span data-ttu-id="87813-142">В случае успеха этот метод возвращает код отклика и новый `200 OK` [объект trustFrameworkKey](../resources/trustframeworkkey.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="87813-142">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87813-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="87813-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="87813-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="87813-144">Request</span></span>

<span data-ttu-id="87813-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87813-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87813-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="87813-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadpkcs12"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadPkcs12
Content-type: application/json

{
  "key": "Base64-encoded-pfx-content",
  "password": "password-value"
}
```
# <a name="c"></a>[<span data-ttu-id="87813-147">C#</span><span class="sxs-lookup"><span data-stu-id="87813-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadpkcs12-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87813-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87813-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadpkcs12-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87813-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87813-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadpkcs12-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87813-150">Java</span><span class="sxs-lookup"><span data-stu-id="87813-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-uploadpkcs12-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="87813-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="87813-151">Response</span></span>

<span data-ttu-id="87813-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="87813-152">The following is an example of the response.</span></span>

> <span data-ttu-id="87813-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="87813-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "kid": "kid-value",
    "use": "sig",
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadPkcs12",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


