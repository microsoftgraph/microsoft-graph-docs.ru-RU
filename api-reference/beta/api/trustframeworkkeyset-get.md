---
title: Получение Трустфрамеворккэйсет
description: Получение свойств и связей объекта трустфрамеворккэйсет.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e70f0cf3e7eaae0add9da7ded068b8c3517529bc
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734684"
---
# <a name="get-trustframeworkkeyset"></a><span data-ttu-id="f862d-103">Получение Трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="f862d-103">Get trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f862d-104">Получение свойств и связей для объекта [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="f862d-104">Retrieve the properties and associations for a [Trustframeworkkeyset](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f862d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f862d-105">Permissions</span></span>

<span data-ttu-id="f862d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f862d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f862d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f862d-108">Permission type</span></span>                        | <span data-ttu-id="f862d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f862d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f862d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f862d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f862d-111">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f862d-111">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="f862d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f862d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f862d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f862d-113">Not supported.</span></span> |
| <span data-ttu-id="f862d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f862d-114">Application</span></span>                            | <span data-ttu-id="f862d-115">Трустфрамеворккэйсет. Read. ALL, Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f862d-115">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f862d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f862d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f862d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f862d-117">Request headers</span></span>

| <span data-ttu-id="f862d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f862d-118">Name</span></span>      |<span data-ttu-id="f862d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f862d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f862d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f862d-120">Authorization</span></span> | <span data-ttu-id="f862d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f862d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f862d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f862d-123">Request body</span></span>

<span data-ttu-id="f862d-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f862d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f862d-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="f862d-125">Response</span></span>

<span data-ttu-id="f862d-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f862d-126">If successful, this method returns a `200 OK` response code and the requested [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f862d-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="f862d-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f862d-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="f862d-128">Request</span></span>

<span data-ttu-id="f862d-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f862d-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_trustframeworkkeyset"
}-->

```http
GET https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```

### <a name="response"></a><span data-ttu-id="f862d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f862d-130">Response</span></span>

<span data-ttu-id="f862d-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f862d-131">The following is an example of the response.</span></span>

> <span data-ttu-id="f862d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f862d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Get trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->