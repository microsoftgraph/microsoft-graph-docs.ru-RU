---
title: 'Трустфрамеворккэйсет: Уплоадцертификате'
description: Отправьте сертификат в набор ключей.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0342565ca8c7e652118c525a3c51c4700840d718
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215905"
---
# <a name="trustframeworkkeyset-uploadcertificate"></a><span data-ttu-id="8526a-103">Трустфрамеворккэйсет: Уплоадцертификате</span><span class="sxs-lookup"><span data-stu-id="8526a-103">trustFrameworkKeySet: uploadCertificate</span></span>

<span data-ttu-id="8526a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8526a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8526a-105">Отправьте сертификат в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="8526a-105">Upload a certificate to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="8526a-106">Входное значение — это значение сертификата в кодировке Base-64.</span><span class="sxs-lookup"><span data-stu-id="8526a-106">The input is a base-64 encoded value of the certificate contents.</span></span> <span data-ttu-id="8526a-107">Этот метод возвращает [трустфрамеворккэй](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="8526a-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8526a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8526a-108">Permissions</span></span>

<span data-ttu-id="8526a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8526a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8526a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8526a-111">Permission type</span></span>                        | <span data-ttu-id="8526a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8526a-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8526a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8526a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8526a-114">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8526a-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="8526a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8526a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8526a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8526a-116">Not supported.</span></span> |
| <span data-ttu-id="8526a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8526a-117">Application</span></span>                            | <span data-ttu-id="8526a-118">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8526a-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8526a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8526a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadCertificate
```

## <a name="request-headers"></a><span data-ttu-id="8526a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8526a-120">Request headers</span></span>

| <span data-ttu-id="8526a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8526a-121">Name</span></span>          | <span data-ttu-id="8526a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8526a-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8526a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8526a-123">Authorization</span></span> | <span data-ttu-id="8526a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8526a-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="8526a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8526a-126">Content-type</span></span> | <span data-ttu-id="8526a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8526a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8526a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8526a-129">Request body</span></span>

<span data-ttu-id="8526a-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8526a-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8526a-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="8526a-131">Parameter</span></span>    | <span data-ttu-id="8526a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8526a-132">Type</span></span>        | <span data-ttu-id="8526a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8526a-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8526a-134">key</span><span class="sxs-lookup"><span data-stu-id="8526a-134">key</span></span>|<span data-ttu-id="8526a-135">Строка</span><span class="sxs-lookup"><span data-stu-id="8526a-135">String</span></span>| <span data-ttu-id="8526a-136">Это поле для отправки контента сертификата.</span><span class="sxs-lookup"><span data-stu-id="8526a-136">This is the field for sending certificate content.</span></span> <span data-ttu-id="8526a-137">Значение должно представлять собой версию фактического содержимого сертификата в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="8526a-137">The value should be a base-64 encoded version of the actual certificate content.</span></span> |

## <a name="response"></a><span data-ttu-id="8526a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8526a-138">Response</span></span>

<span data-ttu-id="8526a-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8526a-139">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8526a-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="8526a-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8526a-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8526a-141">Request</span></span>

<span data-ttu-id="8526a-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8526a-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8526a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8526a-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8526a-144">C#</span><span class="sxs-lookup"><span data-stu-id="8526a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8526a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8526a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8526a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8526a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8526a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8526a-147">Response</span></span>

<span data-ttu-id="8526a-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8526a-148">The following is an example of the response.</span></span>

> <span data-ttu-id="8526a-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8526a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
