---
title: 'Трустфрамеворккэйсет: Женератекэй'
description: Автоматически создает ключ и секрет в наборе ключей.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f8c3385a06c8807ce82169efb5a02f1999223cd4
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215940"
---
# <a name="trustframeworkkeyset-generatekey"></a><span data-ttu-id="5a1c6-103">Трустфрамеворккэйсет: Женератекэй</span><span class="sxs-lookup"><span data-stu-id="5a1c6-103">trustFrameworkKeySet: generateKey</span></span>

<span data-ttu-id="5a1c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a1c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a1c6-105">Автоматическое создание [трустфрамеворккэй](../resources/trustFrameworkKey.md) и секрета в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="5a1c6-105">Generate a [trustFrameworkKey](../resources/trustFrameworkKey.md) and a secret automatically in the [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="5a1c6-106">Вызывающий абонент не должен предоставлять секрет.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-106">The caller doesn't have to provide a secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a1c6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a1c6-107">Permissions</span></span>

<span data-ttu-id="5a1c6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a1c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a1c6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a1c6-110">Permission type</span></span>                        | <span data-ttu-id="5a1c6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a1c6-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5a1c6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a1c6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a1c6-113">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5a1c6-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="5a1c6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a1c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a1c6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-115">Not supported.</span></span> |
| <span data-ttu-id="5a1c6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a1c6-116">Application</span></span>                            | <span data-ttu-id="5a1c6-117">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5a1c6-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a1c6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a1c6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/generateKey
```

## <a name="request-headers"></a><span data-ttu-id="5a1c6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a1c6-119">Request headers</span></span>

| <span data-ttu-id="5a1c6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5a1c6-120">Name</span></span>          | <span data-ttu-id="5a1c6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5a1c6-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5a1c6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a1c6-122">Authorization</span></span> | <span data-ttu-id="5a1c6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a1c6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a1c6-125">Content-type</span></span>  | <span data-ttu-id="5a1c6-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a1c6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a1c6-128">Request body</span></span>

<span data-ttu-id="5a1c6-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5a1c6-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="5a1c6-130">Parameter</span></span>    | <span data-ttu-id="5a1c6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5a1c6-131">Type</span></span>        | <span data-ttu-id="5a1c6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5a1c6-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5a1c6-133">Используйте</span><span class="sxs-lookup"><span data-stu-id="5a1c6-133">use</span></span> | <span data-ttu-id="5a1c6-134">string</span><span class="sxs-lookup"><span data-stu-id="5a1c6-134">string</span></span> | <span data-ttu-id="5a1c6-135">Аналогично свойству **use** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-135">Similar to the **use** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="5a1c6-136">кти</span><span class="sxs-lookup"><span data-stu-id="5a1c6-136">kty</span></span> | <span data-ttu-id="5a1c6-137">string</span><span class="sxs-lookup"><span data-stu-id="5a1c6-137">string</span></span> | <span data-ttu-id="5a1c6-138">Аналогично свойству **КТИ** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-138">Similar to **kty** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="5a1c6-139">nbf</span><span class="sxs-lookup"><span data-stu-id="5a1c6-139">nbf</span></span> | <span data-ttu-id="5a1c6-140">int</span><span class="sxs-lookup"><span data-stu-id="5a1c6-140">int</span></span> | <span data-ttu-id="5a1c6-141">Аналогично **NBF** для свойства **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-141">Similar to **nbf** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="5a1c6-142">exp</span><span class="sxs-lookup"><span data-stu-id="5a1c6-142">exp</span></span> | <span data-ttu-id="5a1c6-143">int</span><span class="sxs-lookup"><span data-stu-id="5a1c6-143">int</span></span> | <span data-ttu-id="5a1c6-144">Аналогично свойству **exp** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-144">Similar to **exp** property of **trustFrameworkKey**.</span></span> |

## <a name="response"></a><span data-ttu-id="5a1c6-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a1c6-145">Response</span></span>

<span data-ttu-id="5a1c6-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-146">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a1c6-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="5a1c6-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a1c6-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a1c6-148">Request</span></span>

<span data-ttu-id="5a1c6-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5a1c6-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a1c6-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5a1c6-151">C#</span><span class="sxs-lookup"><span data-stu-id="5a1c6-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-generatekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a1c6-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a1c6-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-generatekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a1c6-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a1c6-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-generatekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5a1c6-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a1c6-154">Response</span></span>

<span data-ttu-id="5a1c6-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-155">The following is an example of the response.</span></span>

> <span data-ttu-id="5a1c6-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
