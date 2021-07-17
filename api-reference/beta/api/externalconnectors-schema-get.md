---
title: Получение схемы
description: Извлечение свойств схемы для externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: e8efc13fe7cb96b0a820f80974710f5086f1349d
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466999"
---
# <a name="get-schema"></a><span data-ttu-id="01019-103">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="01019-103">Get schema</span></span>

<span data-ttu-id="01019-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="01019-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01019-105">Извлечение свойств [схемы](../resources/externalconnectors-schema.md) для [externalConnection](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="01019-105">Retrieve the properties of a [schema](../resources/externalconnectors-schema.md) for an [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="01019-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01019-106">Permissions</span></span>

<span data-ttu-id="01019-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01019-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01019-109">Permission type</span></span>                        | <span data-ttu-id="01019-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01019-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="01019-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01019-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="01019-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01019-112">Not supported.</span></span> |
| <span data-ttu-id="01019-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01019-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01019-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01019-114">Not supported.</span></span> |
| <span data-ttu-id="01019-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="01019-115">Application</span></span>                            | <span data-ttu-id="01019-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="01019-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="01019-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01019-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01019-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01019-118">Optional query parameters</span></span>

<span data-ttu-id="01019-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="01019-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="01019-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="01019-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="01019-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01019-121">Request headers</span></span>

| <span data-ttu-id="01019-122">Имя</span><span class="sxs-lookup"><span data-stu-id="01019-122">Name</span></span>          | <span data-ttu-id="01019-123">Описание</span><span class="sxs-lookup"><span data-stu-id="01019-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="01019-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01019-124">Authorization</span></span> | <span data-ttu-id="01019-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01019-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01019-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01019-127">Request body</span></span>

<span data-ttu-id="01019-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01019-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01019-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="01019-129">Response</span></span>

<span data-ttu-id="01019-130">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [схемы](../resources/externalconnectors-schema.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="01019-130">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/externalconnectors-schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01019-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="01019-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="01019-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="01019-132">Request</span></span>

<span data-ttu-id="01019-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01019-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01019-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="01019-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="c"></a>[<span data-ttu-id="01019-135">C#</span><span class="sxs-lookup"><span data-stu-id="01019-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01019-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01019-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01019-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01019-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01019-138">Java</span><span class="sxs-lookup"><span data-stu-id="01019-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="01019-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="01019-139">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="01019-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="01019-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.schema"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "string",
      "isSearchable": true,
      "isRetrievable": true,
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "string",
      "isQueryable": true,
      "isRetrievable": true,
      "isRefinable": true,
      "isSearchable": false
    },
    {
      "name": "assignee",
      "type": "string",
      "isRetrievable": true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


