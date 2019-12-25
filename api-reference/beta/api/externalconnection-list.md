---
title: Список подключений
description: Получение списка Екстерналконнектионс.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b6154557f075c038efbf7a0f8cc5e4331d3daef3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869796"
---
# <a name="list-connections"></a><span data-ttu-id="4921d-103">Список подключений</span><span class="sxs-lookup"><span data-stu-id="4921d-103">List connections</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4921d-104">Получение списка [екстерналконнектионс](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="4921d-104">Retrieve a list of [externalConnections](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="4921d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4921d-105">Permissions</span></span>

<span data-ttu-id="4921d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4921d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4921d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4921d-108">Permission type</span></span>                        | <span data-ttu-id="4921d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4921d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4921d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4921d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4921d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4921d-111">Not supported.</span></span> |
| <span data-ttu-id="4921d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4921d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4921d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4921d-113">Not supported.</span></span> |
| <span data-ttu-id="4921d-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="4921d-114">Application</span></span>                            | <span data-ttu-id="4921d-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4921d-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4921d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4921d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4921d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4921d-117">Optional query parameters</span></span>

<span data-ttu-id="4921d-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4921d-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4921d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4921d-119">Request headers</span></span>

| <span data-ttu-id="4921d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4921d-120">Name</span></span>          | <span data-ttu-id="4921d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4921d-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4921d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4921d-122">Authorization</span></span> | <span data-ttu-id="4921d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4921d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4921d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4921d-125">Request body</span></span>

<span data-ttu-id="4921d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4921d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4921d-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="4921d-127">Response</span></span>

<span data-ttu-id="4921d-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [екстерналконнектион](../resources/externalconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4921d-128">If successful, this method returns a `200 OK` response code and a collection of [externalConnection](../resources/externalconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4921d-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="4921d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4921d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4921d-130">Request</span></span>

<span data-ttu-id="4921d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4921d-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4921d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4921d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connections"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4921d-133">C#</span><span class="sxs-lookup"><span data-stu-id="4921d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4921d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4921d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4921d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4921d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="4921d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4921d-136">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="4921d-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4921d-137">The following is an example of the response.</span></span>

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
