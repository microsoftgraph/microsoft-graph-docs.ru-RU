---
title: Подключение
description: Извлечение свойств и связей externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 5f545343bc67b20fab59d48cce21077769c2960a
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467703"
---
# <a name="get-connection"></a><span data-ttu-id="0510f-103">Подключение</span><span class="sxs-lookup"><span data-stu-id="0510f-103">Get connection</span></span>

<span data-ttu-id="0510f-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="0510f-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0510f-105">Извлечение свойств и связей [externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="0510f-105">Retrieve the properties and relationships of an [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0510f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0510f-106">Permissions</span></span>

<span data-ttu-id="0510f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0510f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0510f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0510f-109">Permission type</span></span>                        | <span data-ttu-id="0510f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0510f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0510f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0510f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0510f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0510f-112">Not supported.</span></span> |
| <span data-ttu-id="0510f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0510f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0510f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0510f-114">Not supported.</span></span> |
| <span data-ttu-id="0510f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0510f-115">Application</span></span>                            | <span data-ttu-id="0510f-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="0510f-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="0510f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0510f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0510f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0510f-118">Optional query parameters</span></span>

<span data-ttu-id="0510f-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0510f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0510f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0510f-120">Request headers</span></span>

| <span data-ttu-id="0510f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0510f-121">Name</span></span>          | <span data-ttu-id="0510f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0510f-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0510f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0510f-123">Authorization</span></span> | <span data-ttu-id="0510f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0510f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0510f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0510f-126">Request body</span></span>

<span data-ttu-id="0510f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0510f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0510f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0510f-128">Response</span></span>

<span data-ttu-id="0510f-129">В случае успешной работы этот метод возвращает код отклика и запрашиваемого `200 OK` [объекта externalConnection](../resources/externalconnectors-externalconnection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0510f-129">If successful, this method returns a `200 OK` response code and the requested [externalConnection](../resources/externalconnectors-externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0510f-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="0510f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0510f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0510f-131">Request</span></span>

<span data-ttu-id="0510f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0510f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0510f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0510f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="0510f-134">C#</span><span class="sxs-lookup"><span data-stu-id="0510f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0510f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0510f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0510f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0510f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0510f-137">Java</span><span class="sxs-lookup"><span data-stu-id="0510f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="0510f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0510f-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="0510f-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0510f-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "state": "ready",
  "configuration": {
    "authorizedAppIds": [
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
