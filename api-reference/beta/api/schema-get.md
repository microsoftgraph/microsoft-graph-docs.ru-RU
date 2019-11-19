---
title: Получение схемы
description: Получение свойств схемы для объекта Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: da42ecae79e7e0a81a77edf510a082bb8d3990c2
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703723"
---
# <a name="get-schema"></a><span data-ttu-id="218aa-103">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="218aa-103">Get schema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="218aa-104">Получение свойств [схемы](../resources/schema.md) для объекта [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="218aa-104">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="218aa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="218aa-105">Permissions</span></span>

<span data-ttu-id="218aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="218aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="218aa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="218aa-108">Permission type</span></span>                        | <span data-ttu-id="218aa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="218aa-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="218aa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="218aa-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="218aa-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="218aa-111">Not supported.</span></span> |
| <span data-ttu-id="218aa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="218aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="218aa-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="218aa-113">Not supported.</span></span> |
| <span data-ttu-id="218aa-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="218aa-114">Application</span></span>                            | <span data-ttu-id="218aa-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="218aa-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="218aa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="218aa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="218aa-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="218aa-117">Optional query parameters</span></span>

<span data-ttu-id="218aa-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="218aa-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="218aa-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="218aa-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="218aa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="218aa-120">Request headers</span></span>

| <span data-ttu-id="218aa-121">Имя</span><span class="sxs-lookup"><span data-stu-id="218aa-121">Name</span></span>          | <span data-ttu-id="218aa-122">Описание</span><span class="sxs-lookup"><span data-stu-id="218aa-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="218aa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="218aa-123">Authorization</span></span> | <span data-ttu-id="218aa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="218aa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="218aa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="218aa-126">Request body</span></span>

<span data-ttu-id="218aa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="218aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="218aa-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="218aa-128">Response</span></span>

<span data-ttu-id="218aa-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [схемы](../resources/schema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="218aa-129">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="218aa-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="218aa-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="218aa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="218aa-131">Request</span></span>

<span data-ttu-id="218aa-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="218aa-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="218aa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="218aa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="218aa-134">C#</span><span class="sxs-lookup"><span data-stu-id="218aa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="218aa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="218aa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="218aa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="218aa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="218aa-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="218aa-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="218aa-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="218aa-138">The following is an example of the response.</span></span>

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
      "name": "title",
      "type": "String",
      "isSearchable": true,
      "isRetrievable": true
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": true,
      "isRetrievable": true
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
