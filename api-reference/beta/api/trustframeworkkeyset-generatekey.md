---
title: 'Трустфрамеворккэйсет: Женератекэй'
description: Автоматически создает ключ и секрет в наборе ключей.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f82f6b17aa6155d8d49e02a4a3112f010c6279c2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937578"
---
# <a name="trustframeworkkeyset-generatekey"></a><span data-ttu-id="aee66-103">Трустфрамеворккэйсет: Женератекэй</span><span class="sxs-lookup"><span data-stu-id="aee66-103">trustFrameworkKeySet: generateKey</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aee66-104">Автоматическое создание [трустфрамеворккэй](../resources/trustFrameworkKey.md) и секрета в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="aee66-104">Generate a [trustFrameworkKey](../resources/trustFrameworkKey.md) and a secret automatically in the [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="aee66-105">Вызывающий абонент не должен предоставлять секрет.</span><span class="sxs-lookup"><span data-stu-id="aee66-105">The caller doesn't have to provide a secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="aee66-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aee66-106">Permissions</span></span>

<span data-ttu-id="aee66-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aee66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aee66-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aee66-109">Permission type</span></span>                        | <span data-ttu-id="aee66-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aee66-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aee66-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aee66-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aee66-112">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="aee66-112">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="aee66-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aee66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aee66-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aee66-114">Not supported.</span></span> |
| <span data-ttu-id="aee66-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aee66-115">Application</span></span>                            | <span data-ttu-id="aee66-116">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="aee66-116">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aee66-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aee66-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/generateKey
```

## <a name="request-headers"></a><span data-ttu-id="aee66-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aee66-118">Request headers</span></span>

| <span data-ttu-id="aee66-119">Имя</span><span class="sxs-lookup"><span data-stu-id="aee66-119">Name</span></span>          | <span data-ttu-id="aee66-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aee66-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="aee66-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aee66-121">Authorization</span></span> | <span data-ttu-id="aee66-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aee66-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aee66-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aee66-124">Content-type</span></span>  | <span data-ttu-id="aee66-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aee66-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aee66-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aee66-127">Request body</span></span>

<span data-ttu-id="aee66-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="aee66-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aee66-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="aee66-129">Parameter</span></span>    | <span data-ttu-id="aee66-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aee66-130">Type</span></span>        | <span data-ttu-id="aee66-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aee66-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="aee66-132">Используйте</span><span class="sxs-lookup"><span data-stu-id="aee66-132">use</span></span> | <span data-ttu-id="aee66-133">string</span><span class="sxs-lookup"><span data-stu-id="aee66-133">string</span></span> | <span data-ttu-id="aee66-134">Аналогично свойству **use** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="aee66-134">Similar to the **use** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="aee66-135">кти</span><span class="sxs-lookup"><span data-stu-id="aee66-135">kty</span></span> | <span data-ttu-id="aee66-136">string</span><span class="sxs-lookup"><span data-stu-id="aee66-136">string</span></span> | <span data-ttu-id="aee66-137">Аналогично свойству **КТИ** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="aee66-137">Similar to **kty** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="aee66-138">nbf</span><span class="sxs-lookup"><span data-stu-id="aee66-138">nbf</span></span> | <span data-ttu-id="aee66-139">int</span><span class="sxs-lookup"><span data-stu-id="aee66-139">int</span></span> | <span data-ttu-id="aee66-140">Аналогично **NBF** для свойства **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="aee66-140">Similar to **nbf** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="aee66-141">exp</span><span class="sxs-lookup"><span data-stu-id="aee66-141">exp</span></span> | <span data-ttu-id="aee66-142">int</span><span class="sxs-lookup"><span data-stu-id="aee66-142">int</span></span> | <span data-ttu-id="aee66-143">Аналогично свойству **exp** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="aee66-143">Similar to **exp** property of **trustFrameworkKey**.</span></span> |

## <a name="response"></a><span data-ttu-id="aee66-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="aee66-144">Response</span></span>

<span data-ttu-id="aee66-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aee66-145">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aee66-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="aee66-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aee66-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="aee66-147">Request</span></span>

<span data-ttu-id="aee66-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aee66-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="aee66-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="aee66-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="aee66-150">C#</span><span class="sxs-lookup"><span data-stu-id="aee66-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-generatekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aee66-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aee66-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-generatekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aee66-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aee66-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-generatekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aee66-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="aee66-153">Response</span></span>

<span data-ttu-id="aee66-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aee66-154">The following is an example of the response.</span></span>

> <span data-ttu-id="aee66-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aee66-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
