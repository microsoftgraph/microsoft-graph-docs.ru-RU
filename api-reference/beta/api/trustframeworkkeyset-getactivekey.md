---
title: 'Трустфрамеворккэйсет: Жетактивекэй'
description: Получение активного ключа в наборе ключей.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ea4e1e31812bdbdb7a8e6619280367a5ed873fc9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937549"
---
# <a name="trustframeworkkeyset-getactivekey"></a><span data-ttu-id="627b1-103">Трустфрамеворккэйсет: Жетактивекэй</span><span class="sxs-lookup"><span data-stu-id="627b1-103">trustFrameworkKeySet: getActiveKey</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="627b1-104">Получение активных в данный момент [трустфрамеворккэй](../resources/trustframeworkkey.md) в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="627b1-104">Get the currently active [trustFrameworkKey](../resources/trustframeworkkey.md) in a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="627b1-105">В наборе ключей одновременно активен только один ключ.</span><span class="sxs-lookup"><span data-stu-id="627b1-105">Only one key is active in the keyset at a time.</span></span>


## <a name="permissions"></a><span data-ttu-id="627b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="627b1-106">Permissions</span></span>

<span data-ttu-id="627b1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="627b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="627b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="627b1-109">Permission type</span></span>                        | <span data-ttu-id="627b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="627b1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="627b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="627b1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="627b1-112">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="627b1-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |
| <span data-ttu-id="627b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="627b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="627b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="627b1-114">Not supported.</span></span> |
| <span data-ttu-id="627b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="627b1-115">Application</span></span>                            | <span data-ttu-id="627b1-116">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="627b1-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="627b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="627b1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/getActiveKey
```

## <a name="request-headers"></a><span data-ttu-id="627b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="627b1-118">Request headers</span></span>

| <span data-ttu-id="627b1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="627b1-119">Name</span></span>          | <span data-ttu-id="627b1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="627b1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="627b1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="627b1-121">Authorization</span></span> | <span data-ttu-id="627b1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="627b1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="627b1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="627b1-124">Request body</span></span>

<span data-ttu-id="627b1-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="627b1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="627b1-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="627b1-126">Response</span></span>

<span data-ttu-id="627b1-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="627b1-127">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="627b1-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="627b1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="627b1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="627b1-129">Request</span></span>

<span data-ttu-id="627b1-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="627b1-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="627b1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="627b1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_getactivekey"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/getActiveKey
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="627b1-132">C#</span><span class="sxs-lookup"><span data-stu-id="627b1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-getactivekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="627b1-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="627b1-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-getactivekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="627b1-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="627b1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-getactivekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="627b1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="627b1-135">Response</span></span>

<span data-ttu-id="627b1-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="627b1-136">The following is an example of the response.</span></span>

> <span data-ttu-id="627b1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="627b1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "k": "k-value",
  "x5c": [
    "x5c-value"
  ],
  "x5t": "x5t-value",
  "kty": "kty-value",
  "use": "use-value",
  "exp": 99
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: getActiveKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
