---
title: Получение схемы
description: Получение свойств схемы для объекта Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: dbaba2bc54bf2b28c95584826f8baa83c803894b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014156"
---
# <a name="get-schema"></a><span data-ttu-id="f9140-103">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="f9140-103">Get schema</span></span>

<span data-ttu-id="f9140-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9140-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9140-105">Получение свойств [схемы](../resources/schema.md) для объекта [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f9140-105">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="f9140-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9140-106">Permissions</span></span>

<span data-ttu-id="f9140-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9140-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9140-109">Permission type</span></span>                        | <span data-ttu-id="f9140-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9140-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f9140-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9140-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9140-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9140-112">Not supported.</span></span> |
| <span data-ttu-id="f9140-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9140-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9140-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9140-114">Not supported.</span></span> |
| <span data-ttu-id="f9140-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9140-115">Application</span></span>                            | <span data-ttu-id="f9140-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9140-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9140-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9140-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9140-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9140-118">Optional query parameters</span></span>

<span data-ttu-id="f9140-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f9140-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f9140-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f9140-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9140-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9140-121">Request headers</span></span>

| <span data-ttu-id="f9140-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f9140-122">Name</span></span>          | <span data-ttu-id="f9140-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f9140-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f9140-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9140-124">Authorization</span></span> | <span data-ttu-id="f9140-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9140-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9140-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9140-127">Request body</span></span>

<span data-ttu-id="f9140-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9140-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9140-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9140-129">Response</span></span>

<span data-ttu-id="f9140-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [схемы](../resources/schema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9140-130">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9140-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f9140-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9140-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9140-132">Request</span></span>

<span data-ttu-id="f9140-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9140-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9140-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9140-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="c"></a>[<span data-ttu-id="f9140-135">C#</span><span class="sxs-lookup"><span data-stu-id="f9140-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9140-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9140-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9140-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9140-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="f9140-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9140-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f9140-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f9140-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schema"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": true,
      "isRetrievable": true,
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": true,
      "isRetrievable": true,
      "isRefinable": true,
      "isSearchable": false
    },
    {
      "name": "assignee",
      "type": "String",
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


