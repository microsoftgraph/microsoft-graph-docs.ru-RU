---
title: 'Трустфрамеворккэйсет: Уплоадцертификате'
description: Отправьте сертификат в набор ключей.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 726e2d98ca1002f9e3a9e3d8a7bf705550767529
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937521"
---
# <a name="trustframeworkkeyset-uploadcertificate"></a><span data-ttu-id="c3945-103">Трустфрамеворккэйсет: Уплоадцертификате</span><span class="sxs-lookup"><span data-stu-id="c3945-103">trustFrameworkKeySet: uploadCertificate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3945-104">Отправьте сертификат в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="c3945-104">Upload a certificate to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="c3945-105">Входное значение — это значение сертификата в кодировке Base-64.</span><span class="sxs-lookup"><span data-stu-id="c3945-105">The input is a base-64 encoded value of the certificate contents.</span></span> <span data-ttu-id="c3945-106">Этот метод возвращает [трустфрамеворккэй](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="c3945-106">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3945-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3945-107">Permissions</span></span>

<span data-ttu-id="c3945-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3945-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3945-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3945-110">Permission type</span></span>                        | <span data-ttu-id="c3945-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3945-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c3945-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3945-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c3945-113">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c3945-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="c3945-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3945-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3945-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3945-115">Not supported.</span></span> |
| <span data-ttu-id="c3945-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3945-116">Application</span></span>                            | <span data-ttu-id="c3945-117">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c3945-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3945-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3945-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadCertificate
```

## <a name="request-headers"></a><span data-ttu-id="c3945-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3945-119">Request headers</span></span>

| <span data-ttu-id="c3945-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c3945-120">Name</span></span>          | <span data-ttu-id="c3945-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c3945-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c3945-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3945-122">Authorization</span></span> | <span data-ttu-id="c3945-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3945-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="c3945-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3945-125">Content-type</span></span> | <span data-ttu-id="c3945-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3945-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3945-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3945-128">Request body</span></span>

<span data-ttu-id="c3945-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c3945-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c3945-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="c3945-130">Parameter</span></span>    | <span data-ttu-id="c3945-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3945-131">Type</span></span>        | <span data-ttu-id="c3945-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3945-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c3945-133">key</span><span class="sxs-lookup"><span data-stu-id="c3945-133">key</span></span>|<span data-ttu-id="c3945-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c3945-134">String</span></span>| <span data-ttu-id="c3945-135">Это поле для отправки контента сертификата.</span><span class="sxs-lookup"><span data-stu-id="c3945-135">This is the field for sending certificate content.</span></span> <span data-ttu-id="c3945-136">Значение должно представлять собой версию фактического содержимого сертификата в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="c3945-136">The value should be a base-64 encoded version of the actual certificate content.</span></span> |

## <a name="response"></a><span data-ttu-id="c3945-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3945-137">Response</span></span>

<span data-ttu-id="c3945-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3945-138">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3945-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="c3945-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3945-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3945-140">Request</span></span>

<span data-ttu-id="c3945-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3945-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c3945-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3945-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3945-143">C#</span><span class="sxs-lookup"><span data-stu-id="c3945-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3945-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3945-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3945-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3945-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c3945-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3945-146">Response</span></span>

<span data-ttu-id="c3945-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c3945-147">The following is an example of the response.</span></span>

> <span data-ttu-id="c3945-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3945-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
