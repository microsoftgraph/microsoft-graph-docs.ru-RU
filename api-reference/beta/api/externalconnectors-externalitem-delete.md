---
title: Удаление externalItem
description: Удаление externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 26b556a71f6eda6ee2860fc897eb14d58ae9a249
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467002"
---
# <a name="delete-externalitem"></a><span data-ttu-id="11677-103">Удаление externalItem</span><span class="sxs-lookup"><span data-stu-id="11677-103">Delete externalItem</span></span>

<span data-ttu-id="11677-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="11677-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11677-105">Удаление [externalitem](../resources/externalconnectors-externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="11677-105">Delete an [externalitem](../resources/externalconnectors-externalitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="11677-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11677-106">Permissions</span></span>

<span data-ttu-id="11677-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11677-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11677-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11677-109">Permission type</span></span>                        | <span data-ttu-id="11677-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11677-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="11677-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11677-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11677-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11677-112">Not supported.</span></span> |
| <span data-ttu-id="11677-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11677-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11677-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11677-114">Not supported.</span></span> |
| <span data-ttu-id="11677-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="11677-115">Application</span></span>                            | <span data-ttu-id="11677-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11677-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11677-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11677-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="11677-118">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="11677-118">Path parameters</span></span>

| <span data-ttu-id="11677-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="11677-119">Parameter</span></span>     | <span data-ttu-id="11677-120">Тип</span><span class="sxs-lookup"><span data-stu-id="11677-120">Type</span></span>   | <span data-ttu-id="11677-121">Описание</span><span class="sxs-lookup"><span data-stu-id="11677-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="11677-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="11677-122">connection-id</span></span> | <span data-ttu-id="11677-123">String</span><span class="sxs-lookup"><span data-stu-id="11677-123">string</span></span> | <span data-ttu-id="11677-124">`id`Свойствосодержащего [externalConnection](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="11677-124">The `id` property of the containing [externalConnection](../resources/externalconnectors-externalconnection.md)</span></span> |
| <span data-ttu-id="11677-125">item-id</span><span class="sxs-lookup"><span data-stu-id="11677-125">item-id</span></span>       | <span data-ttu-id="11677-126">String</span><span class="sxs-lookup"><span data-stu-id="11677-126">string</span></span> | <span data-ttu-id="11677-127">Свойство `id` [externalItem,](../resources/externalconnectors-externalitem.md)предоставленное разработчиком.</span><span class="sxs-lookup"><span data-stu-id="11677-127">The developer-provided `id` property of the [externalItem](../resources/externalconnectors-externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="11677-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11677-128">Request headers</span></span>

| <span data-ttu-id="11677-129">Имя</span><span class="sxs-lookup"><span data-stu-id="11677-129">Name</span></span>          | <span data-ttu-id="11677-130">Описание</span><span class="sxs-lookup"><span data-stu-id="11677-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="11677-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11677-131">Authorization</span></span> | <span data-ttu-id="11677-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11677-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11677-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11677-134">Request body</span></span>

<span data-ttu-id="11677-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11677-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11677-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="11677-136">Response</span></span>

<span data-ttu-id="11677-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="11677-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11677-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="11677-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11677-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="11677-140">Request</span></span>

<span data-ttu-id="11677-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11677-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11677-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="11677-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="11677-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11677-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="11677-144">C#</span><span class="sxs-lookup"><span data-stu-id="11677-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11677-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11677-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11677-146">Java</span><span class="sxs-lookup"><span data-stu-id="11677-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="11677-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="11677-147">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="11677-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="11677-148">The following is an example of the response.</span></span>

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


