---
title: 'trustFrameworkKeySet: uploadCertificate'
description: Upload сертификат на набор ключей.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 841a99797e737b79ee9d480b14a06c90a2bc2f48
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053421"
---
# <a name="trustframeworkkeyset-uploadcertificate"></a><span data-ttu-id="d2e14-103">trustFrameworkKeySet: uploadCertificate</span><span class="sxs-lookup"><span data-stu-id="d2e14-103">trustFrameworkKeySet: uploadCertificate</span></span>

<span data-ttu-id="d2e14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2e14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2e14-105">Upload сертификат в [trustFrameworkKeyset.](../resources/trustframeworkkeyset.md)</span><span class="sxs-lookup"><span data-stu-id="d2e14-105">Upload a certificate to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="d2e14-106">Входное значение — это закодированное значение содержимого сертификата базового значения 64.</span><span class="sxs-lookup"><span data-stu-id="d2e14-106">The input is a base-64 encoded value of the certificate contents.</span></span> <span data-ttu-id="d2e14-107">Этот метод возвращает [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="d2e14-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2e14-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2e14-108">Permissions</span></span>

<span data-ttu-id="d2e14-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2e14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2e14-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2e14-111">Permission type</span></span>                        | <span data-ttu-id="d2e14-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2e14-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2e14-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2e14-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2e14-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2e14-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="d2e14-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2e14-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2e14-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2e14-116">Not supported.</span></span> |
| <span data-ttu-id="d2e14-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d2e14-117">Application</span></span>                            | <span data-ttu-id="d2e14-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2e14-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2e14-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2e14-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadCertificate
```

## <a name="request-headers"></a><span data-ttu-id="d2e14-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2e14-120">Request headers</span></span>

| <span data-ttu-id="d2e14-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d2e14-121">Name</span></span>          | <span data-ttu-id="d2e14-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d2e14-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d2e14-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2e14-123">Authorization</span></span> | <span data-ttu-id="d2e14-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2e14-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d2e14-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2e14-126">Content-type</span></span> | <span data-ttu-id="d2e14-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2e14-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2e14-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2e14-129">Request body</span></span>

<span data-ttu-id="d2e14-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d2e14-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d2e14-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="d2e14-131">Parameter</span></span>    | <span data-ttu-id="d2e14-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d2e14-132">Type</span></span>        | <span data-ttu-id="d2e14-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d2e14-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d2e14-134">key</span><span class="sxs-lookup"><span data-stu-id="d2e14-134">key</span></span>|<span data-ttu-id="d2e14-135">String</span><span class="sxs-lookup"><span data-stu-id="d2e14-135">String</span></span>| <span data-ttu-id="d2e14-136">Это поле для отправки контента сертификата.</span><span class="sxs-lookup"><span data-stu-id="d2e14-136">This is the field for sending certificate content.</span></span> <span data-ttu-id="d2e14-137">Значение должно быть кодированной версией базового-64 фактического контента сертификата.</span><span class="sxs-lookup"><span data-stu-id="d2e14-137">The value should be a base-64 encoded version of the actual certificate content.</span></span> |

## <a name="response"></a><span data-ttu-id="d2e14-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2e14-138">Response</span></span>

<span data-ttu-id="d2e14-139">В случае успеха этот метод возвращает код отклика и новый `200 OK` [объект trustFrameworkKey](../resources/trustframeworkkey.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d2e14-139">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2e14-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2e14-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2e14-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2e14-141">Request</span></span>

<span data-ttu-id="d2e14-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2e14-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2e14-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2e14-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadCertificate
Content-type: application/json

{
  "key": "key-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d2e14-144">C#</span><span class="sxs-lookup"><span data-stu-id="d2e14-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2e14-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2e14-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2e14-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2e14-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2e14-147">Java</span><span class="sxs-lookup"><span data-stu-id="d2e14-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-uploadcertificate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2e14-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2e14-148">Response</span></span>

<span data-ttu-id="d2e14-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d2e14-149">The following is an example of the response.</span></span>

> <span data-ttu-id="d2e14-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d2e14-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "kty": "oct",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


