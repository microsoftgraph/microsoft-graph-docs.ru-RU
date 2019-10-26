---
title: 'Трустфрамеворккэйсет: Жетактивекэй'
description: Получение активного ключа в наборе ключей.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e0e45d1cb19f6591dac620569a2d48738b2089b5
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734689"
---
# <a name="trustframeworkkeyset-getactivekey"></a><span data-ttu-id="04eb3-103">Трустфрамеворккэйсет: Жетактивекэй</span><span class="sxs-lookup"><span data-stu-id="04eb3-103">trustFrameworkKeySet: getActiveKey</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04eb3-104">Получение активных в данный момент [трустфрамеворккэй](../resources/trustframeworkkey.md) в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="04eb3-104">Get the currently active [trustFrameworkKey](../resources/trustframeworkkey.md) in a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="04eb3-105">В наборе ключей одновременно активен только один ключ.</span><span class="sxs-lookup"><span data-stu-id="04eb3-105">Only one key is active in the keyset at a time.</span></span>


## <a name="permissions"></a><span data-ttu-id="04eb3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04eb3-106">Permissions</span></span>

<span data-ttu-id="04eb3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04eb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04eb3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04eb3-109">Permission type</span></span>                        | <span data-ttu-id="04eb3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04eb3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="04eb3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04eb3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="04eb3-112">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="04eb3-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |
| <span data-ttu-id="04eb3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04eb3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04eb3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04eb3-114">Not supported.</span></span> |
| <span data-ttu-id="04eb3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04eb3-115">Application</span></span>                            | <span data-ttu-id="04eb3-116">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="04eb3-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04eb3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04eb3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/getActiveKey
```

## <a name="request-headers"></a><span data-ttu-id="04eb3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04eb3-118">Request headers</span></span>

| <span data-ttu-id="04eb3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="04eb3-119">Name</span></span>          | <span data-ttu-id="04eb3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="04eb3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="04eb3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04eb3-121">Authorization</span></span> | <span data-ttu-id="04eb3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04eb3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04eb3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04eb3-124">Request body</span></span>

<span data-ttu-id="04eb3-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04eb3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04eb3-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="04eb3-126">Response</span></span>

<span data-ttu-id="04eb3-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04eb3-127">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04eb3-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="04eb3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04eb3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="04eb3-129">Request</span></span>

<span data-ttu-id="04eb3-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04eb3-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_getactivekey"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/getActiveKey
```

### <a name="response"></a><span data-ttu-id="04eb3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="04eb3-131">Response</span></span>

<span data-ttu-id="04eb3-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04eb3-132">The following is an example of the response.</span></span>

> <span data-ttu-id="04eb3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04eb3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
