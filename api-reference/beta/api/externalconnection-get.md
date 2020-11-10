---
title: Получение подключения
description: Получение свойств и связей объекта Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c32f04e7f373e8955e794d5ce9e4f62a477936cd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965656"
---
# <a name="get-connection"></a><span data-ttu-id="d1262-103">Получение подключения</span><span class="sxs-lookup"><span data-stu-id="d1262-103">Get connection</span></span>

<span data-ttu-id="d1262-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1262-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1262-105">Получение свойств и связей объекта [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="d1262-105">Retrieve the properties and relationships of an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="d1262-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1262-106">Permissions</span></span>

<span data-ttu-id="d1262-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1262-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1262-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1262-109">Permission type</span></span>                        | <span data-ttu-id="d1262-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1262-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d1262-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1262-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1262-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1262-112">Not supported.</span></span> |
| <span data-ttu-id="d1262-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1262-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1262-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1262-114">Not supported.</span></span> |
| <span data-ttu-id="d1262-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d1262-115">Application</span></span>                            | <span data-ttu-id="d1262-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1262-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1262-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1262-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1262-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1262-118">Optional query parameters</span></span>

<span data-ttu-id="d1262-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d1262-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1262-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1262-120">Request headers</span></span>

| <span data-ttu-id="d1262-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d1262-121">Name</span></span>          | <span data-ttu-id="d1262-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d1262-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d1262-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1262-123">Authorization</span></span> | <span data-ttu-id="d1262-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1262-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1262-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1262-126">Request body</span></span>

<span data-ttu-id="d1262-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1262-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1262-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1262-128">Response</span></span>

<span data-ttu-id="d1262-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [екстерналконнектион](../resources/externalconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1262-129">If successful, this method returns a `200 OK` response code and the requested [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1262-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="d1262-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1262-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1262-131">Request</span></span>

<span data-ttu-id="d1262-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1262-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1262-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1262-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="d1262-134">C#</span><span class="sxs-lookup"><span data-stu-id="d1262-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1262-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1262-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1262-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1262-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1262-137">Java</span><span class="sxs-lookup"><span data-stu-id="d1262-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="d1262-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1262-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d1262-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d1262-139">The following is an example of the response.</span></span>

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


