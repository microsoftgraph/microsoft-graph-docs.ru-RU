---
title: 'Трустфрамеворккэйсет: Жетактивекэй'
description: Получение активного ключа в наборе ключей.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: db234801ed4f4a1f1599d249d95f17b92a1f8afb
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215891"
---
# <a name="trustframeworkkeyset-getactivekey"></a><span data-ttu-id="49511-103">Трустфрамеворккэйсет: Жетактивекэй</span><span class="sxs-lookup"><span data-stu-id="49511-103">trustFrameworkKeySet: getActiveKey</span></span>

<span data-ttu-id="49511-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49511-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49511-105">Получение активных в данный момент [трустфрамеворккэй](../resources/trustframeworkkey.md) в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="49511-105">Get the currently active [trustFrameworkKey](../resources/trustframeworkkey.md) in a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="49511-106">В наборе ключей одновременно активен только один ключ.</span><span class="sxs-lookup"><span data-stu-id="49511-106">Only one key is active in the keyset at a time.</span></span>


## <a name="permissions"></a><span data-ttu-id="49511-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49511-107">Permissions</span></span>

<span data-ttu-id="49511-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49511-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49511-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49511-110">Permission type</span></span>                        | <span data-ttu-id="49511-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49511-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="49511-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49511-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="49511-113">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="49511-113">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |
| <span data-ttu-id="49511-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49511-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49511-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49511-115">Not supported.</span></span> |
| <span data-ttu-id="49511-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49511-116">Application</span></span>                            | <span data-ttu-id="49511-117">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="49511-117">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49511-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49511-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/getActiveKey
```

## <a name="request-headers"></a><span data-ttu-id="49511-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49511-119">Request headers</span></span>

| <span data-ttu-id="49511-120">Имя</span><span class="sxs-lookup"><span data-stu-id="49511-120">Name</span></span>          | <span data-ttu-id="49511-121">Описание</span><span class="sxs-lookup"><span data-stu-id="49511-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="49511-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49511-122">Authorization</span></span> | <span data-ttu-id="49511-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49511-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49511-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49511-125">Request body</span></span>

<span data-ttu-id="49511-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49511-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49511-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="49511-127">Response</span></span>

<span data-ttu-id="49511-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49511-128">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49511-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="49511-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49511-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="49511-130">Request</span></span>

<span data-ttu-id="49511-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49511-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49511-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="49511-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_getactivekey"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/getActiveKey
```
# <a name="c"></a>[<span data-ttu-id="49511-133">C#</span><span class="sxs-lookup"><span data-stu-id="49511-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-getactivekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49511-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49511-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-getactivekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49511-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49511-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-getactivekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49511-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="49511-136">Response</span></span>

<span data-ttu-id="49511-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49511-137">The following is an example of the response.</span></span>

> <span data-ttu-id="49511-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49511-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
