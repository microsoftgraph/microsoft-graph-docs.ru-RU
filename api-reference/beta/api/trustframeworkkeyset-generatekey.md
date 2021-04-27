---
title: 'trustFrameworkKeySet: generateKey'
description: Создание ключа и секрета автоматически в наборе ключей.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2dd481634a9b42a9cf40d2d507e06c95b225b0c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053442"
---
# <a name="trustframeworkkeyset-generatekey"></a><span data-ttu-id="7aaf9-103">trustFrameworkKeySet: generateKey</span><span class="sxs-lookup"><span data-stu-id="7aaf9-103">trustFrameworkKeySet: generateKey</span></span>

<span data-ttu-id="7aaf9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aaf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aaf9-105">Создание [trustFrameworkKey](../resources/trustFrameworkKey.md) и секрет автоматически в [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="7aaf9-105">Generate a [trustFrameworkKey](../resources/trustFrameworkKey.md) and a secret automatically in the [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="7aaf9-106">Вызываемая не должна предоставлять секрет.</span><span class="sxs-lookup"><span data-stu-id="7aaf9-106">The caller doesn't have to provide a secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aaf9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7aaf9-107">Permissions</span></span>

<span data-ttu-id="7aaf9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aaf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7aaf9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7aaf9-110">Permission type</span></span>                        | <span data-ttu-id="7aaf9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7aaf9-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7aaf9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7aaf9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7aaf9-113">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aaf9-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="7aaf9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7aaf9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aaf9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aaf9-115">Not supported.</span></span> |
| <span data-ttu-id="7aaf9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7aaf9-116">Application</span></span>                            | <span data-ttu-id="7aaf9-117">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aaf9-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aaf9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aaf9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/generateKey
```

## <a name="request-headers"></a><span data-ttu-id="7aaf9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7aaf9-119">Request headers</span></span>

| <span data-ttu-id="7aaf9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7aaf9-120">Name</span></span>          | <span data-ttu-id="7aaf9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7aaf9-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7aaf9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7aaf9-122">Authorization</span></span> | <span data-ttu-id="7aaf9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7aaf9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7aaf9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7aaf9-125">Content-type</span></span>  | <span data-ttu-id="7aaf9-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7aaf9-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aaf9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7aaf9-128">Request body</span></span>

<span data-ttu-id="7aaf9-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7aaf9-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7aaf9-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="7aaf9-130">Parameter</span></span>    | <span data-ttu-id="7aaf9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7aaf9-131">Type</span></span>        | <span data-ttu-id="7aaf9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7aaf9-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7aaf9-133">использование</span><span class="sxs-lookup"><span data-stu-id="7aaf9-133">use</span></span> | <span data-ttu-id="7aaf9-134">String</span><span class="sxs-lookup"><span data-stu-id="7aaf9-134">string</span></span> | <span data-ttu-id="7aaf9-135">Аналогично **свойству использования** **trustFrameworkKey.**</span><span class="sxs-lookup"><span data-stu-id="7aaf9-135">Similar to the **use** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="7aaf9-136">kty</span><span class="sxs-lookup"><span data-stu-id="7aaf9-136">kty</span></span> | <span data-ttu-id="7aaf9-137">String</span><span class="sxs-lookup"><span data-stu-id="7aaf9-137">string</span></span> | <span data-ttu-id="7aaf9-138">Аналогично **свойству kty** **trustFrameworkKey.**</span><span class="sxs-lookup"><span data-stu-id="7aaf9-138">Similar to **kty** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="7aaf9-139">nbf</span><span class="sxs-lookup"><span data-stu-id="7aaf9-139">nbf</span></span> | <span data-ttu-id="7aaf9-140">int</span><span class="sxs-lookup"><span data-stu-id="7aaf9-140">int</span></span> | <span data-ttu-id="7aaf9-141">Аналогично **свойству nbf** **trustFrameworkKey.**</span><span class="sxs-lookup"><span data-stu-id="7aaf9-141">Similar to **nbf** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="7aaf9-142">exp</span><span class="sxs-lookup"><span data-stu-id="7aaf9-142">exp</span></span> | <span data-ttu-id="7aaf9-143">int</span><span class="sxs-lookup"><span data-stu-id="7aaf9-143">int</span></span> | <span data-ttu-id="7aaf9-144">Аналогично **свойству exp** **trustFrameworkKey.**</span><span class="sxs-lookup"><span data-stu-id="7aaf9-144">Similar to **exp** property of **trustFrameworkKey**.</span></span> |

## <a name="response"></a><span data-ttu-id="7aaf9-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aaf9-145">Response</span></span>

<span data-ttu-id="7aaf9-146">В случае успеха этот метод возвращает код отклика и новый `200 OK` [объект trustFrameworkKey](../resources/trustframeworkkey.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7aaf9-146">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7aaf9-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="7aaf9-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7aaf9-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="7aaf9-148">Request</span></span>

<span data-ttu-id="7aaf9-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7aaf9-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7aaf9-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="7aaf9-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_generatekey"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/generateKey
Content-type: application/json

{
  "use": "sig",
  "kty": "RSA",
  "nbf": 1508969811,
  "exp": 1508969811
}
```
# <a name="c"></a>[<span data-ttu-id="7aaf9-151">C#</span><span class="sxs-lookup"><span data-stu-id="7aaf9-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-generatekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7aaf9-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7aaf9-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-generatekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7aaf9-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7aaf9-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-generatekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7aaf9-154">Java</span><span class="sxs-lookup"><span data-stu-id="7aaf9-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-generatekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7aaf9-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aaf9-155">Response</span></span>

<span data-ttu-id="7aaf9-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7aaf9-156">The following is an example of the response.</span></span>

> <span data-ttu-id="7aaf9-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7aaf9-157">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.trustFrameworkKey",
    "k": null,
    "x5c": [],
    "kty": "RSA",
    "use": "sig",
    "exp": 1908969811,
    "nbf": 1908969811,
    "kid": "Gaid7K8sO8RavMX9fzHir_Wg0femGhbY9b-B4rVIxbE",
    "e": "AQAB",
    "n": "rd54s6",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: generateKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


