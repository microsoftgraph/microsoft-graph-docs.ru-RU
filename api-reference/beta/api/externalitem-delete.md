---
title: Удаление Екстерналитем
description: Удаление Екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: f9abe39baa29ba247994d4ea6ff8c30bd7f28f72
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006802"
---
# <a name="delete-externalitem"></a><span data-ttu-id="d9ea1-103">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="d9ea1-103">Delete externalItem</span></span>

<span data-ttu-id="d9ea1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9ea1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9ea1-105">Удаление [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="d9ea1-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="d9ea1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9ea1-106">Permissions</span></span>

<span data-ttu-id="d9ea1-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d9ea1-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d9ea1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9ea1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9ea1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9ea1-109">Permission type</span></span>                        | <span data-ttu-id="d9ea1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9ea1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d9ea1-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9ea1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9ea1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9ea1-112">Not supported.</span></span> |
| <span data-ttu-id="d9ea1-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9ea1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9ea1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9ea1-114">Not supported.</span></span> |
| <span data-ttu-id="d9ea1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9ea1-115">Application</span></span>                            | <span data-ttu-id="d9ea1-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9ea1-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9ea1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9ea1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="d9ea1-118">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="d9ea1-118">Path parameters</span></span>

| <span data-ttu-id="d9ea1-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="d9ea1-119">Parameter</span></span>     | <span data-ttu-id="d9ea1-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d9ea1-120">Type</span></span>   | <span data-ttu-id="d9ea1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d9ea1-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="d9ea1-122">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="d9ea1-122">connection-id</span></span> | <span data-ttu-id="d9ea1-123">string</span><span class="sxs-lookup"><span data-stu-id="d9ea1-123">string</span></span> | <span data-ttu-id="d9ea1-124">`id`Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="d9ea1-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="d9ea1-125">item-id</span><span class="sxs-lookup"><span data-stu-id="d9ea1-125">item-id</span></span>       | <span data-ttu-id="d9ea1-126">string</span><span class="sxs-lookup"><span data-stu-id="d9ea1-126">string</span></span> | <span data-ttu-id="d9ea1-127">Предоставляемое разработчиком `id` свойство [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="d9ea1-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d9ea1-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9ea1-128">Request headers</span></span>

| <span data-ttu-id="d9ea1-129">Имя</span><span class="sxs-lookup"><span data-stu-id="d9ea1-129">Name</span></span>          | <span data-ttu-id="d9ea1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d9ea1-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d9ea1-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9ea1-131">Authorization</span></span> | <span data-ttu-id="d9ea1-132">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="d9ea1-132">Bearer {token}.</span></span> <span data-ttu-id="d9ea1-133">Required.</span><span class="sxs-lookup"><span data-stu-id="d9ea1-133">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9ea1-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9ea1-134">Request body</span></span>

<span data-ttu-id="d9ea1-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9ea1-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9ea1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9ea1-136">Response</span></span>

<span data-ttu-id="d9ea1-137">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="d9ea1-137">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="d9ea1-138">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="d9ea1-138">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9ea1-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="d9ea1-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9ea1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9ea1-140">Request</span></span>

<span data-ttu-id="d9ea1-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9ea1-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9ea1-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9ea1-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="d9ea1-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9ea1-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d9ea1-144">C#</span><span class="sxs-lookup"><span data-stu-id="d9ea1-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9ea1-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9ea1-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="d9ea1-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9ea1-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d9ea1-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d9ea1-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
