---
title: 'Трустфрамеворккэйсет: Женератекэй'
description: Автоматически создает ключ и секрет в наборе ключей.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5915bcf514c96ddea2c7e3ce2df2653e38b4cb7d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981700"
---
# <a name="trustframeworkkeyset-generatekey"></a><span data-ttu-id="53322-103">Трустфрамеворккэйсет: Женератекэй</span><span class="sxs-lookup"><span data-stu-id="53322-103">trustFrameworkKeySet: generateKey</span></span>

<span data-ttu-id="53322-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53322-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53322-105">Автоматическое создание [трустфрамеворккэй](../resources/trustFrameworkKey.md) и секрета в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="53322-105">Generate a [trustFrameworkKey](../resources/trustFrameworkKey.md) and a secret automatically in the [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="53322-106">Вызывающий абонент не должен предоставлять секрет.</span><span class="sxs-lookup"><span data-stu-id="53322-106">The caller doesn't have to provide a secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="53322-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53322-107">Permissions</span></span>

<span data-ttu-id="53322-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53322-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53322-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53322-110">Permission type</span></span>                        | <span data-ttu-id="53322-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53322-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="53322-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53322-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="53322-113">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="53322-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="53322-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53322-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53322-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53322-115">Not supported.</span></span> |
| <span data-ttu-id="53322-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="53322-116">Application</span></span>                            | <span data-ttu-id="53322-117">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="53322-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53322-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53322-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/generateKey
```

## <a name="request-headers"></a><span data-ttu-id="53322-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53322-119">Request headers</span></span>

| <span data-ttu-id="53322-120">Имя</span><span class="sxs-lookup"><span data-stu-id="53322-120">Name</span></span>          | <span data-ttu-id="53322-121">Описание</span><span class="sxs-lookup"><span data-stu-id="53322-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="53322-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53322-122">Authorization</span></span> | <span data-ttu-id="53322-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53322-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53322-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53322-125">Content-type</span></span>  | <span data-ttu-id="53322-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53322-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53322-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53322-128">Request body</span></span>

<span data-ttu-id="53322-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="53322-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53322-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="53322-130">Parameter</span></span>    | <span data-ttu-id="53322-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53322-131">Type</span></span>        | <span data-ttu-id="53322-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53322-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="53322-133">Используйте</span><span class="sxs-lookup"><span data-stu-id="53322-133">use</span></span> | <span data-ttu-id="53322-134">string</span><span class="sxs-lookup"><span data-stu-id="53322-134">string</span></span> | <span data-ttu-id="53322-135">Аналогично свойству **use** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="53322-135">Similar to the **use** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="53322-136">кти</span><span class="sxs-lookup"><span data-stu-id="53322-136">kty</span></span> | <span data-ttu-id="53322-137">string</span><span class="sxs-lookup"><span data-stu-id="53322-137">string</span></span> | <span data-ttu-id="53322-138">Аналогично свойству **КТИ** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="53322-138">Similar to **kty** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="53322-139">nbf</span><span class="sxs-lookup"><span data-stu-id="53322-139">nbf</span></span> | <span data-ttu-id="53322-140">int</span><span class="sxs-lookup"><span data-stu-id="53322-140">int</span></span> | <span data-ttu-id="53322-141">Аналогично **NBF** для свойства **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="53322-141">Similar to **nbf** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="53322-142">exp</span><span class="sxs-lookup"><span data-stu-id="53322-142">exp</span></span> | <span data-ttu-id="53322-143">int</span><span class="sxs-lookup"><span data-stu-id="53322-143">int</span></span> | <span data-ttu-id="53322-144">Аналогично свойству **exp** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="53322-144">Similar to **exp** property of **trustFrameworkKey**.</span></span> |

## <a name="response"></a><span data-ttu-id="53322-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="53322-145">Response</span></span>

<span data-ttu-id="53322-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53322-146">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53322-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="53322-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53322-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="53322-148">Request</span></span>

<span data-ttu-id="53322-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53322-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53322-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="53322-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="53322-151">C#</span><span class="sxs-lookup"><span data-stu-id="53322-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-generatekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53322-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53322-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-generatekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53322-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53322-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-generatekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53322-154">Java</span><span class="sxs-lookup"><span data-stu-id="53322-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-generatekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53322-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="53322-155">Response</span></span>

<span data-ttu-id="53322-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53322-156">The following is an example of the response.</span></span>

> <span data-ttu-id="53322-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53322-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


