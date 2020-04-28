---
title: Список подключений
description: Получение списка Екстерналконнектионс.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c47d2e58bed88748e6b05e3099bc1d2d930bbb9f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422259"
---
# <a name="list-connections"></a><span data-ttu-id="cfcfd-103">Список подключений</span><span class="sxs-lookup"><span data-stu-id="cfcfd-103">List connections</span></span>

<span data-ttu-id="cfcfd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfcfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfcfd-105">Получение списка [екстерналконнектионс](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="cfcfd-105">Retrieve a list of [externalConnections](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="cfcfd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfcfd-106">Permissions</span></span>

<span data-ttu-id="cfcfd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfcfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cfcfd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfcfd-109">Permission type</span></span>                        | <span data-ttu-id="cfcfd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfcfd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cfcfd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfcfd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cfcfd-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfcfd-112">Not supported.</span></span> |
| <span data-ttu-id="cfcfd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfcfd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfcfd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfcfd-114">Not supported.</span></span> |
| <span data-ttu-id="cfcfd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfcfd-115">Application</span></span>                            | <span data-ttu-id="cfcfd-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfcfd-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfcfd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfcfd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cfcfd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cfcfd-118">Optional query parameters</span></span>

<span data-ttu-id="cfcfd-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cfcfd-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfcfd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfcfd-120">Request headers</span></span>

| <span data-ttu-id="cfcfd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cfcfd-121">Name</span></span>          | <span data-ttu-id="cfcfd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cfcfd-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cfcfd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cfcfd-123">Authorization</span></span> | <span data-ttu-id="cfcfd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfcfd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfcfd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cfcfd-126">Request body</span></span>

<span data-ttu-id="cfcfd-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cfcfd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfcfd-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="cfcfd-128">Response</span></span>

<span data-ttu-id="cfcfd-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [екстерналконнектион](../resources/externalconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cfcfd-129">If successful, this method returns a `200 OK` response code and a collection of [externalConnection](../resources/externalconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfcfd-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="cfcfd-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cfcfd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfcfd-131">Request</span></span>

<span data-ttu-id="cfcfd-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfcfd-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfcfd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfcfd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connections"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections
```
# <a name="c"></a>[<span data-ttu-id="cfcfd-134">C#</span><span class="sxs-lookup"><span data-stu-id="cfcfd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfcfd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfcfd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfcfd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfcfd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="cfcfd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfcfd-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="cfcfd-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cfcfd-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contosohr",
      "name": "Contoso HR",
      "description": "Connection to index Contoso HR system",
      "configuration": {
        "authorizedApps": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    },
    {
      "id": "contosofinance",
      "name": "Contoso Finance",
      "description": "Connection to index Contoso Finance system",
      "configuration": {
        "authorizedApps": [
          "fbdc7d4e-07f4-4143-8258-e5a2fcebeadb"
        ]
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
