---
title: Подключение
description: Извлечение свойств и связей externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: fbab97a4e09aef1722176f6b7e25dc52df8cbbea
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366872"
---
# <a name="get-connection"></a><span data-ttu-id="0638c-103">Подключение</span><span class="sxs-lookup"><span data-stu-id="0638c-103">Get connection</span></span>

<span data-ttu-id="0638c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0638c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0638c-105">Извлечение свойств и связей [externalConnection.](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="0638c-105">Retrieve the properties and relationships of an [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0638c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0638c-106">Permissions</span></span>

<span data-ttu-id="0638c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0638c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0638c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0638c-109">Permission type</span></span>                        | <span data-ttu-id="0638c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0638c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0638c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0638c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0638c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0638c-112">Not supported.</span></span> |
| <span data-ttu-id="0638c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0638c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0638c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0638c-114">Not supported.</span></span> |
| <span data-ttu-id="0638c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0638c-115">Application</span></span>                            | <span data-ttu-id="0638c-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0638c-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0638c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0638c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0638c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0638c-118">Optional query parameters</span></span>

<span data-ttu-id="0638c-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0638c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0638c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0638c-120">Request headers</span></span>

| <span data-ttu-id="0638c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0638c-121">Name</span></span>          | <span data-ttu-id="0638c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0638c-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0638c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0638c-123">Authorization</span></span> | <span data-ttu-id="0638c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0638c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0638c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0638c-126">Request body</span></span>

<span data-ttu-id="0638c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0638c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0638c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0638c-128">Response</span></span>

<span data-ttu-id="0638c-129">В случае успешной работы этот метод возвращает код отклика и запрашиваемого `200 OK` [объекта externalConnection](../resources/externalconnection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0638c-129">If successful, this method returns a `200 OK` response code and the requested [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0638c-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="0638c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0638c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0638c-131">Request</span></span>

<span data-ttu-id="0638c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0638c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0638c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0638c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="0638c-134">C#</span><span class="sxs-lookup"><span data-stu-id="0638c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0638c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0638c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0638c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0638c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0638c-137">Java</span><span class="sxs-lookup"><span data-stu-id="0638c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="0638c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0638c-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="0638c-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0638c-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "configuration": {
    "authorizedApps": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


