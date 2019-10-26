---
title: Обновление Трустфрамеворккэйсет
description: Обновление свойств объекта **трустфрамеворккэйсет** .
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3de58ada2a4dd91042785366566b8f1ca2c907dc
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734680"
---
# <a name="update-trustframeworkkeyset"></a><span data-ttu-id="bdf4d-103">Обновление Трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="bdf4d-103">Update trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdf4d-104">Обновление свойств объекта [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="bdf4d-104">Update the properties of a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="bdf4d-105">Эта операция заменит содержимое существующего набора ключей.</span><span class="sxs-lookup"><span data-stu-id="bdf4d-105">This operation will replace the content of an existing keyset.</span></span> <span data-ttu-id="bdf4d-106">Указывать идентификатор в полезных данных запроса необязательно.</span><span class="sxs-lookup"><span data-stu-id="bdf4d-106">Specifying the ID in the request payload is optional.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdf4d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdf4d-107">Permissions</span></span>

<span data-ttu-id="bdf4d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdf4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdf4d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdf4d-110">Permission type</span></span>                        | <span data-ttu-id="bdf4d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdf4d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bdf4d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdf4d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdf4d-113">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bdf4d-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="bdf4d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdf4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdf4d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdf4d-115">Not supported.</span></span> |
| <span data-ttu-id="bdf4d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdf4d-116">Application</span></span>                            | <span data-ttu-id="bdf4d-117">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bdf4d-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdf4d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdf4d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bdf4d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdf4d-119">Request headers</span></span>

| <span data-ttu-id="bdf4d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bdf4d-120">Name</span></span>       | <span data-ttu-id="bdf4d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf4d-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bdf4d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdf4d-122">Authorization</span></span> | <span data-ttu-id="bdf4d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdf4d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bdf4d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bdf4d-125">Content-type</span></span>  | <span data-ttu-id="bdf4d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdf4d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdf4d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdf4d-128">Request body</span></span>


| <span data-ttu-id="bdf4d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdf4d-129">Property</span></span>     | <span data-ttu-id="bdf4d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bdf4d-130">Type</span></span>        | <span data-ttu-id="bdf4d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf4d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bdf4d-132">переключен</span><span class="sxs-lookup"><span data-stu-id="bdf4d-132">keys</span></span>|<span data-ttu-id="bdf4d-133">Коллекция [трустфрамеворккэй](../resources/trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="bdf4d-133">[trustFrameworkKey](../resources/trustframeworkkey.md) collection</span></span>| <span data-ttu-id="bdf4d-134">Обновляет коллекцию Трустфрамеворккэйс</span><span class="sxs-lookup"><span data-stu-id="bdf4d-134">updates a collection of Trustframeworkkeys</span></span>|

## <a name="response"></a><span data-ttu-id="bdf4d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdf4d-135">Response</span></span>

<span data-ttu-id="bdf4d-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdf4d-136">If successful, this method returns a `200 OK` response code and an updated [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bdf4d-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="bdf4d-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bdf4d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdf4d-138">Request</span></span>

<span data-ttu-id="bdf4d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdf4d-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_trustframeworkkeyset"
}-->

```http
PUT https://graph.microsoft.com/beta/trustFramework/keySets/{id}
Content-type: application/json

{
  "keys": [
    {
      "k": "k-value",
      "x5c": [
        "x5c-value"
      ],
      "x5t": "x5t-value",
      "kty": "kty-value",
      "use": "use-value",
      "exp": 99,
      "nbf": 99,
      "kid": "kid-value",
      "e": "e-value",
      "n": "n-value",
      "d": "d-value",
      "p": "p-value",
      "q": "q-value",
      "dp": "dp-value",
      "dq": "dq-value",
      "qi": "qi-value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="bdf4d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdf4d-140">Response</span></span>

<span data-ttu-id="bdf4d-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bdf4d-141">The following is an example of the response.</span></span>

> <span data-ttu-id="bdf4d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdf4d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "keys": [
    {
      "k": "k-value",
      "x5c": [
        "x5c-value"
      ],
      "x5t": "x5t-value",
      "kty": "kty-value",
      "use": "use-value",
      "exp": 99,
      "nbf": 99,
      "kid": "kid-value",
      "e": "e-value",
      "n": "n-value",
      "d": "d-value",
      "p": "p-value",
      "q": "q-value",
      "dp": "dp-value",
      "dq": "dq-value",
      "qi": "qi-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update trustframeworkkeyset",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
