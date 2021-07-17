---
title: Подключения к списку
description: Извлечение списка externalConnections.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 5237fd7450bb2c289247a1343b8fd16dba1e8ae5
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467702"
---
# <a name="list-connections"></a><span data-ttu-id="0fa85-103">Подключения к списку</span><span class="sxs-lookup"><span data-stu-id="0fa85-103">List connections</span></span>

<span data-ttu-id="0fa85-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="0fa85-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fa85-105">Извлечение списка [externalConnections](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="0fa85-105">Retrieve a list of [externalConnections](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fa85-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fa85-106">Permissions</span></span>

<span data-ttu-id="0fa85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fa85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fa85-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fa85-109">Permission type</span></span>                        | <span data-ttu-id="0fa85-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fa85-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0fa85-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fa85-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fa85-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fa85-112">Not supported.</span></span> |
| <span data-ttu-id="0fa85-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fa85-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fa85-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fa85-114">Not supported.</span></span> |
| <span data-ttu-id="0fa85-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0fa85-115">Application</span></span>                            | <span data-ttu-id="0fa85-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="0fa85-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fa85-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fa85-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fa85-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0fa85-118">Optional query parameters</span></span>

<span data-ttu-id="0fa85-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0fa85-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fa85-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fa85-120">Request headers</span></span>

| <span data-ttu-id="0fa85-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0fa85-121">Name</span></span>          | <span data-ttu-id="0fa85-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0fa85-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0fa85-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fa85-123">Authorization</span></span> | <span data-ttu-id="0fa85-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fa85-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fa85-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fa85-126">Request body</span></span>

<span data-ttu-id="0fa85-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0fa85-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fa85-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fa85-128">Response</span></span>

<span data-ttu-id="0fa85-129">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов externalConnection](../resources/externalconnectors-externalconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fa85-129">If successful, this method returns a `200 OK` response code and a collection of [externalConnection](../resources/externalconnectors-externalconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0fa85-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="0fa85-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0fa85-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fa85-131">Request</span></span>

<span data-ttu-id="0fa85-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fa85-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0fa85-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fa85-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connections"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections
```
# <a name="c"></a>[<span data-ttu-id="0fa85-134">C#</span><span class="sxs-lookup"><span data-stu-id="0fa85-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fa85-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fa85-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fa85-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fa85-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fa85-137">Java</span><span class="sxs-lookup"><span data-stu-id="0fa85-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="0fa85-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fa85-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="0fa85-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0fa85-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection",
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
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    },
    {
      "id": "contosofinance",
      "name": "Contoso Finance",
      "description": "Connection to index Contoso Finance system",
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
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
