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
# <a name="delete-externalitem"></a><span data-ttu-id="57475-103">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="57475-103">Delete externalItem</span></span>

<span data-ttu-id="57475-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57475-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57475-105">Удаление [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="57475-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="57475-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57475-106">Permissions</span></span>

<span data-ttu-id="57475-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57475-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57475-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57475-109">Permission type</span></span>                        | <span data-ttu-id="57475-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57475-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="57475-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57475-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="57475-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57475-112">Not supported.</span></span> |
| <span data-ttu-id="57475-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57475-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57475-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57475-114">Not supported.</span></span> |
| <span data-ttu-id="57475-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57475-115">Application</span></span>                            | <span data-ttu-id="57475-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57475-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57475-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57475-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="57475-118">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="57475-118">Path parameters</span></span>

| <span data-ttu-id="57475-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="57475-119">Parameter</span></span>     | <span data-ttu-id="57475-120">Тип</span><span class="sxs-lookup"><span data-stu-id="57475-120">Type</span></span>   | <span data-ttu-id="57475-121">Описание</span><span class="sxs-lookup"><span data-stu-id="57475-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="57475-122">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="57475-122">connection-id</span></span> | <span data-ttu-id="57475-123">string</span><span class="sxs-lookup"><span data-stu-id="57475-123">string</span></span> | <span data-ttu-id="57475-124">`id`Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="57475-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="57475-125">item-id</span><span class="sxs-lookup"><span data-stu-id="57475-125">item-id</span></span>       | <span data-ttu-id="57475-126">string</span><span class="sxs-lookup"><span data-stu-id="57475-126">string</span></span> | <span data-ttu-id="57475-127">Предоставляемое разработчиком `id` свойство [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="57475-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="57475-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57475-128">Request headers</span></span>

| <span data-ttu-id="57475-129">Имя</span><span class="sxs-lookup"><span data-stu-id="57475-129">Name</span></span>          | <span data-ttu-id="57475-130">Описание</span><span class="sxs-lookup"><span data-stu-id="57475-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="57475-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57475-131">Authorization</span></span> | <span data-ttu-id="57475-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57475-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57475-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57475-134">Request body</span></span>

<span data-ttu-id="57475-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57475-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57475-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="57475-136">Response</span></span>

<span data-ttu-id="57475-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="57475-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57475-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="57475-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57475-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="57475-140">Request</span></span>

<span data-ttu-id="57475-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57475-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57475-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="57475-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="57475-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57475-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="57475-144">C#</span><span class="sxs-lookup"><span data-stu-id="57475-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57475-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57475-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="57475-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="57475-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="57475-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="57475-147">The following is an example of the response.</span></span>

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
