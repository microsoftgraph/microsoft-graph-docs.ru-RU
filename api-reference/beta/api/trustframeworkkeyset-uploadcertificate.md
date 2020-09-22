---
title: 'Трустфрамеворккэйсет: Уплоадцертификате'
description: Отправьте сертификат в набор ключей.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 81b52d3757e8710d264d3280a9012f80bc32b438
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027272"
---
# <a name="trustframeworkkeyset-uploadcertificate"></a><span data-ttu-id="b3514-103">Трустфрамеворккэйсет: Уплоадцертификате</span><span class="sxs-lookup"><span data-stu-id="b3514-103">trustFrameworkKeySet: uploadCertificate</span></span>

<span data-ttu-id="b3514-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3514-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3514-105">Отправьте сертификат в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="b3514-105">Upload a certificate to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="b3514-106">Входное значение — это значение сертификата в кодировке Base-64.</span><span class="sxs-lookup"><span data-stu-id="b3514-106">The input is a base-64 encoded value of the certificate contents.</span></span> <span data-ttu-id="b3514-107">Этот метод возвращает [трустфрамеворккэй](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="b3514-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3514-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3514-108">Permissions</span></span>

<span data-ttu-id="b3514-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3514-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3514-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3514-111">Permission type</span></span>                        | <span data-ttu-id="b3514-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3514-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b3514-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3514-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3514-114">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b3514-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="b3514-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3514-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3514-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3514-116">Not supported.</span></span> |
| <span data-ttu-id="b3514-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3514-117">Application</span></span>                            | <span data-ttu-id="b3514-118">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b3514-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3514-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3514-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadCertificate
```

## <a name="request-headers"></a><span data-ttu-id="b3514-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3514-120">Request headers</span></span>

| <span data-ttu-id="b3514-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b3514-121">Name</span></span>          | <span data-ttu-id="b3514-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b3514-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b3514-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3514-123">Authorization</span></span> | <span data-ttu-id="b3514-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3514-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="b3514-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3514-126">Content-type</span></span> | <span data-ttu-id="b3514-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3514-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3514-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3514-129">Request body</span></span>

<span data-ttu-id="b3514-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b3514-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b3514-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="b3514-131">Parameter</span></span>    | <span data-ttu-id="b3514-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b3514-132">Type</span></span>        | <span data-ttu-id="b3514-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b3514-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b3514-134">key</span><span class="sxs-lookup"><span data-stu-id="b3514-134">key</span></span>|<span data-ttu-id="b3514-135">String</span><span class="sxs-lookup"><span data-stu-id="b3514-135">String</span></span>| <span data-ttu-id="b3514-136">Это поле для отправки контента сертификата.</span><span class="sxs-lookup"><span data-stu-id="b3514-136">This is the field for sending certificate content.</span></span> <span data-ttu-id="b3514-137">Значение должно представлять собой версию фактического содержимого сертификата в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="b3514-137">The value should be a base-64 encoded version of the actual certificate content.</span></span> |

## <a name="response"></a><span data-ttu-id="b3514-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3514-138">Response</span></span>

<span data-ttu-id="b3514-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3514-139">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3514-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3514-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3514-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3514-141">Request</span></span>

<span data-ttu-id="b3514-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3514-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3514-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3514-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b3514-144">C#</span><span class="sxs-lookup"><span data-stu-id="b3514-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3514-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3514-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3514-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3514-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b3514-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3514-147">Response</span></span>

<span data-ttu-id="b3514-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3514-148">The following is an example of the response.</span></span>

> <span data-ttu-id="b3514-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3514-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


