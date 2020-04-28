---
title: Получение подключения
description: Получение свойств и связей объекта Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 9d373e885ee7b0bd0a954d919fc6ff9e7e328fea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422273"
---
# <a name="get-connection"></a><span data-ttu-id="79d10-103">Получение подключения</span><span class="sxs-lookup"><span data-stu-id="79d10-103">Get connection</span></span>

<span data-ttu-id="79d10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79d10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79d10-105">Получение свойств и связей объекта [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="79d10-105">Retrieve the properties and relationships of an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="79d10-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79d10-106">Permissions</span></span>

<span data-ttu-id="79d10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79d10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79d10-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79d10-109">Permission type</span></span>                        | <span data-ttu-id="79d10-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79d10-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="79d10-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79d10-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="79d10-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79d10-112">Not supported.</span></span> |
| <span data-ttu-id="79d10-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79d10-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79d10-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79d10-114">Not supported.</span></span> |
| <span data-ttu-id="79d10-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79d10-115">Application</span></span>                            | <span data-ttu-id="79d10-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79d10-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79d10-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79d10-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79d10-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="79d10-118">Optional query parameters</span></span>

<span data-ttu-id="79d10-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="79d10-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79d10-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79d10-120">Request headers</span></span>

| <span data-ttu-id="79d10-121">Имя</span><span class="sxs-lookup"><span data-stu-id="79d10-121">Name</span></span>          | <span data-ttu-id="79d10-122">Описание</span><span class="sxs-lookup"><span data-stu-id="79d10-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="79d10-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79d10-123">Authorization</span></span> | <span data-ttu-id="79d10-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79d10-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79d10-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79d10-126">Request body</span></span>

<span data-ttu-id="79d10-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79d10-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79d10-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="79d10-128">Response</span></span>

<span data-ttu-id="79d10-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [екстерналконнектион](../resources/externalconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79d10-129">If successful, this method returns a `200 OK` response code and the requested [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79d10-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="79d10-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79d10-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="79d10-131">Request</span></span>

<span data-ttu-id="79d10-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79d10-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79d10-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="79d10-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="79d10-134">C#</span><span class="sxs-lookup"><span data-stu-id="79d10-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79d10-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79d10-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79d10-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79d10-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="79d10-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="79d10-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="79d10-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="79d10-138">The following is an example of the response.</span></span>

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
