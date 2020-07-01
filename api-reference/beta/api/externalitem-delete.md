---
title: Удаление Екстерналитем
description: Удаление Екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: be19c8ddb584ca17e6eac346996239a0c90c6738
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990001"
---
# <a name="delete-externalitem"></a><span data-ttu-id="928ae-103">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="928ae-103">Delete externalItem</span></span>

<span data-ttu-id="928ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="928ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="928ae-105">Удаление [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="928ae-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="928ae-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="928ae-106">Permissions</span></span>

<span data-ttu-id="928ae-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="928ae-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="928ae-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="928ae-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="928ae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="928ae-109">Permission type</span></span>                        | <span data-ttu-id="928ae-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="928ae-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="928ae-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="928ae-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="928ae-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="928ae-112">Not supported.</span></span> |
| <span data-ttu-id="928ae-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="928ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="928ae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="928ae-114">Not supported.</span></span> |
| <span data-ttu-id="928ae-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="928ae-115">Application</span></span>                            | <span data-ttu-id="928ae-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="928ae-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="928ae-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="928ae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="928ae-118">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="928ae-118">Path parameters</span></span>

| <span data-ttu-id="928ae-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="928ae-119">Parameter</span></span>     | <span data-ttu-id="928ae-120">Тип</span><span class="sxs-lookup"><span data-stu-id="928ae-120">Type</span></span>   | <span data-ttu-id="928ae-121">Описание</span><span class="sxs-lookup"><span data-stu-id="928ae-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="928ae-122">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="928ae-122">connection-id</span></span> | <span data-ttu-id="928ae-123">string</span><span class="sxs-lookup"><span data-stu-id="928ae-123">string</span></span> | <span data-ttu-id="928ae-124">`id`Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="928ae-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="928ae-125">item-id</span><span class="sxs-lookup"><span data-stu-id="928ae-125">item-id</span></span>       | <span data-ttu-id="928ae-126">string</span><span class="sxs-lookup"><span data-stu-id="928ae-126">string</span></span> | <span data-ttu-id="928ae-127">Предоставляемое разработчиком `id` свойство [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="928ae-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="928ae-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="928ae-128">Request headers</span></span>

| <span data-ttu-id="928ae-129">Имя</span><span class="sxs-lookup"><span data-stu-id="928ae-129">Name</span></span>          | <span data-ttu-id="928ae-130">Описание</span><span class="sxs-lookup"><span data-stu-id="928ae-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="928ae-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="928ae-131">Authorization</span></span> | <span data-ttu-id="928ae-132">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="928ae-132">Bearer {token}.</span></span> <span data-ttu-id="928ae-133">Required.</span><span class="sxs-lookup"><span data-stu-id="928ae-133">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="928ae-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="928ae-134">Request body</span></span>

<span data-ttu-id="928ae-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="928ae-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="928ae-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="928ae-136">Response</span></span>

<span data-ttu-id="928ae-137">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="928ae-137">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="928ae-138">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="928ae-138">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="928ae-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="928ae-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="928ae-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="928ae-140">Request</span></span>

<span data-ttu-id="928ae-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="928ae-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="928ae-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="928ae-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="928ae-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="928ae-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="928ae-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="928ae-144">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="928ae-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="928ae-145">The following is an example of the response.</span></span>

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
