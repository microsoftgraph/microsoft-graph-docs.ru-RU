---
title: Получение схемы
description: Получение свойств схемы для объекта Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: de4e793a224466738773f959892a31b002737f92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453767"
---
# <a name="get-schema"></a><span data-ttu-id="2ab1a-103">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="2ab1a-103">Get schema</span></span>

<span data-ttu-id="2ab1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ab1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ab1a-105">Получение свойств [схемы](../resources/schema.md) для объекта [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="2ab1a-105">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="2ab1a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ab1a-106">Permissions</span></span>

<span data-ttu-id="2ab1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ab1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ab1a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ab1a-109">Permission type</span></span>                        | <span data-ttu-id="2ab1a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ab1a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ab1a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ab1a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ab1a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ab1a-112">Not supported.</span></span> |
| <span data-ttu-id="2ab1a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ab1a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ab1a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ab1a-114">Not supported.</span></span> |
| <span data-ttu-id="2ab1a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ab1a-115">Application</span></span>                            | <span data-ttu-id="2ab1a-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ab1a-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ab1a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ab1a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ab1a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2ab1a-118">Optional query parameters</span></span>

<span data-ttu-id="2ab1a-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2ab1a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2ab1a-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2ab1a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ab1a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ab1a-121">Request headers</span></span>

| <span data-ttu-id="2ab1a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2ab1a-122">Name</span></span>          | <span data-ttu-id="2ab1a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2ab1a-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2ab1a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ab1a-124">Authorization</span></span> | <span data-ttu-id="2ab1a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ab1a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ab1a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2ab1a-127">Request body</span></span>

<span data-ttu-id="2ab1a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ab1a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ab1a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ab1a-129">Response</span></span>

<span data-ttu-id="2ab1a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [схемы](../resources/schema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ab1a-130">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ab1a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ab1a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ab1a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ab1a-132">Request</span></span>

<span data-ttu-id="2ab1a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ab1a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ab1a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ab1a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="c"></a>[<span data-ttu-id="2ab1a-135">C#</span><span class="sxs-lookup"><span data-stu-id="2ab1a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ab1a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ab1a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ab1a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ab1a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="2ab1a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ab1a-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="2ab1a-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2ab1a-139">The following is an example of the response.</span></span>

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
