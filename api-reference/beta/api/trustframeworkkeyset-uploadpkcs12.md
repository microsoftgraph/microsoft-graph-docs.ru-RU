---
title: 'Трустфрамеворккэйсет: uploadPkcs12'
description: Отправьте ключ формата PKCS 12 (PFX) в набор ключей.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64d5b2d2c10194156a1b577437d1e7a90773b80a
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219013"
---
# <a name="trustframeworkkeyset-uploadpkcs12"></a><span data-ttu-id="e3d9e-103">Трустфрамеворккэйсет: uploadPkcs12</span><span class="sxs-lookup"><span data-stu-id="e3d9e-103">trustFrameworkKeySet: uploadPkcs12</span></span>

<span data-ttu-id="e3d9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3d9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3d9e-105">Отправьте ключ формата PKCS12 (PFX) в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="e3d9e-105">Upload a PKCS12 format key (PFX) to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="e3d9e-106">Входные данные — это значение, закодированное как Base-64, для контента сертификата pfx.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-106">The input is a base-64 encoded value of the Pfx certificate contents.</span></span> <span data-ttu-id="e3d9e-107">Этот метод возвращает [трустфрамеворккэй](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="e3d9e-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3d9e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3d9e-108">Permissions</span></span>

<span data-ttu-id="e3d9e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3d9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3d9e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3d9e-111">Permission type</span></span>                        | <span data-ttu-id="e3d9e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3d9e-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e3d9e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3d9e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3d9e-114">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e3d9e-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="e3d9e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3d9e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3d9e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-116">Not supported.</span></span> |
| <span data-ttu-id="e3d9e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3d9e-117">Application</span></span>                            | <span data-ttu-id="e3d9e-118">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e3d9e-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3d9e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3d9e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadPkcs12
```

## <a name="request-headers"></a><span data-ttu-id="e3d9e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3d9e-120">Request headers</span></span>

| <span data-ttu-id="e3d9e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e3d9e-121">Name</span></span>          | <span data-ttu-id="e3d9e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e3d9e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e3d9e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3d9e-123">Authorization</span></span> | <span data-ttu-id="e3d9e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e3d9e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3d9e-126">Content-type</span></span>  | <span data-ttu-id="e3d9e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3d9e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3d9e-129">Request body</span></span>

<span data-ttu-id="e3d9e-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e3d9e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="e3d9e-131">Parameter</span></span>    | <span data-ttu-id="e3d9e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e3d9e-132">Type</span></span>        | <span data-ttu-id="e3d9e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e3d9e-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e3d9e-134">key</span><span class="sxs-lookup"><span data-stu-id="e3d9e-134">key</span></span>|<span data-ttu-id="e3d9e-135">String</span><span class="sxs-lookup"><span data-stu-id="e3d9e-135">String</span></span>|<span data-ttu-id="e3d9e-136">Это поле для отправки PFX-содержимого.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-136">This is the field for sending pfx content.</span></span> <span data-ttu-id="e3d9e-137">Значение должно представлять собой версию фактического содержимого сертификата в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-137">The value should be a base-64 encoded version of the actual certificate content.</span></span>|
|<span data-ttu-id="e3d9e-138">password</span><span class="sxs-lookup"><span data-stu-id="e3d9e-138">password</span></span>|<span data-ttu-id="e3d9e-139">Строка</span><span class="sxs-lookup"><span data-stu-id="e3d9e-139">String</span></span>|<span data-ttu-id="e3d9e-140">Это поле для отправки пароля в PFX-контент.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-140">This is the field for sending the password to PFX content.</span></span>|

## <a name="response"></a><span data-ttu-id="e3d9e-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3d9e-141">Response</span></span>

<span data-ttu-id="e3d9e-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-142">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3d9e-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3d9e-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3d9e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3d9e-144">Request</span></span>

<span data-ttu-id="e3d9e-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3d9e-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3d9e-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e3d9e-147">C#</span><span class="sxs-lookup"><span data-stu-id="e3d9e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadpkcs12-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3d9e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3d9e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadpkcs12-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3d9e-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3d9e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadpkcs12-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e3d9e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3d9e-150">Response</span></span>

<span data-ttu-id="e3d9e-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-151">The following is an example of the response.</span></span>

> <span data-ttu-id="e3d9e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3d9e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
