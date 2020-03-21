---
title: Удаление Екстерналитем
description: Удаление Екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 263d04ed1b254a52d9eacab19997e40cdac4dc67
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892544"
---
# <a name="delete-externalitem"></a><span data-ttu-id="0f390-103">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="0f390-103">Delete externalItem</span></span>

<span data-ttu-id="0f390-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f390-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f390-105">Удаление [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="0f390-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="0f390-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f390-106">Permissions</span></span>

<span data-ttu-id="0f390-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f390-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f390-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f390-109">Permission type</span></span>                        | <span data-ttu-id="0f390-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f390-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0f390-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f390-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f390-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f390-112">Not supported.</span></span> |
| <span data-ttu-id="0f390-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f390-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f390-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f390-114">Not supported.</span></span> |
| <span data-ttu-id="0f390-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0f390-115">Application</span></span>                            | <span data-ttu-id="0f390-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f390-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f390-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f390-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="0f390-118">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="0f390-118">Path parameters</span></span>

| <span data-ttu-id="0f390-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="0f390-119">Parameter</span></span>     | <span data-ttu-id="0f390-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0f390-120">Type</span></span>   | <span data-ttu-id="0f390-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0f390-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="0f390-122">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="0f390-122">connection-id</span></span> | <span data-ttu-id="0f390-123">string</span><span class="sxs-lookup"><span data-stu-id="0f390-123">string</span></span> | <span data-ttu-id="0f390-124">`id` Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="0f390-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="0f390-125">item-id</span><span class="sxs-lookup"><span data-stu-id="0f390-125">item-id</span></span>       | <span data-ttu-id="0f390-126">string</span><span class="sxs-lookup"><span data-stu-id="0f390-126">string</span></span> | <span data-ttu-id="0f390-127">Предоставляемое `id` разработчиком свойство [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="0f390-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0f390-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f390-128">Request headers</span></span>

| <span data-ttu-id="0f390-129">Имя</span><span class="sxs-lookup"><span data-stu-id="0f390-129">Name</span></span>          | <span data-ttu-id="0f390-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0f390-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0f390-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f390-131">Authorization</span></span> | <span data-ttu-id="0f390-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f390-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f390-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0f390-134">Request body</span></span>

<span data-ttu-id="0f390-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f390-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f390-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f390-136">Response</span></span>

<span data-ttu-id="0f390-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0f390-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0f390-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="0f390-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f390-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f390-140">Request</span></span>

<span data-ttu-id="0f390-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f390-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0f390-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f390-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="0f390-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f390-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="0f390-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f390-144">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="0f390-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0f390-145">The following is an example of the response.</span></span>

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
