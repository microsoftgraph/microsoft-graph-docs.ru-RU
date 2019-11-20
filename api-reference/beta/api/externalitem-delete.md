---
title: Удаление Екстерналитем
description: Удаление Екстерналитем или Екстерналфиле.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6e3f76c3c12d49b73f71fbf2bc7b93f6479103e9
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747185"
---
# <a name="delete-externalitem"></a><span data-ttu-id="b49aa-103">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="b49aa-103">Delete externalItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b49aa-104">Удаление [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="b49aa-104">Delete an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="b49aa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b49aa-105">Permissions</span></span>

<span data-ttu-id="b49aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b49aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b49aa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b49aa-108">Permission type</span></span>                        | <span data-ttu-id="b49aa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b49aa-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b49aa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b49aa-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b49aa-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b49aa-111">Not supported.</span></span> |
| <span data-ttu-id="b49aa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b49aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b49aa-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b49aa-113">Not supported.</span></span> |
| <span data-ttu-id="b49aa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b49aa-114">Application</span></span>                            | <span data-ttu-id="b49aa-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b49aa-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b49aa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b49aa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="b49aa-117">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="b49aa-117">Path parameters</span></span>

| <span data-ttu-id="b49aa-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="b49aa-118">Parameter</span></span>     | <span data-ttu-id="b49aa-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b49aa-119">Type</span></span>   | <span data-ttu-id="b49aa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b49aa-120">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="b49aa-121">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="b49aa-121">connection-id</span></span> | <span data-ttu-id="b49aa-122">string</span><span class="sxs-lookup"><span data-stu-id="b49aa-122">string</span></span> | <span data-ttu-id="b49aa-123">`id` Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="b49aa-123">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="b49aa-124">item-id</span><span class="sxs-lookup"><span data-stu-id="b49aa-124">item-id</span></span>       | <span data-ttu-id="b49aa-125">string</span><span class="sxs-lookup"><span data-stu-id="b49aa-125">string</span></span> | <span data-ttu-id="b49aa-126">Предоставляемое `id` разработчиком свойство [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="b49aa-126">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b49aa-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b49aa-127">Request headers</span></span>

| <span data-ttu-id="b49aa-128">Имя</span><span class="sxs-lookup"><span data-stu-id="b49aa-128">Name</span></span>          | <span data-ttu-id="b49aa-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b49aa-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b49aa-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b49aa-130">Authorization</span></span> | <span data-ttu-id="b49aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b49aa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b49aa-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b49aa-133">Request body</span></span>

<span data-ttu-id="b49aa-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b49aa-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b49aa-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b49aa-135">Response</span></span>

<span data-ttu-id="b49aa-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b49aa-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b49aa-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="b49aa-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b49aa-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b49aa-139">Request</span></span>

<span data-ttu-id="b49aa-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b49aa-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b49aa-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b49aa-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b49aa-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b49aa-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="b49aa-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b49aa-143">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="b49aa-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b49aa-144">The following is an example of the response.</span></span>

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
