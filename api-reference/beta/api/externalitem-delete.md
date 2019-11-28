---
title: Удаление Екстерналитем
description: Удаление Екстерналитем или Екстерналфиле.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 34a34c3913ccf4da490a79b2449e06ff45fc8512
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636815"
---
# <a name="delete-externalitem"></a><span data-ttu-id="18e53-103">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="18e53-103">Delete externalItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18e53-104">Удаление [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="18e53-104">Delete an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="18e53-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18e53-105">Permissions</span></span>

<span data-ttu-id="18e53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18e53-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18e53-108">Permission type</span></span>                        | <span data-ttu-id="18e53-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18e53-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="18e53-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18e53-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="18e53-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18e53-111">Not supported.</span></span> |
| <span data-ttu-id="18e53-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18e53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18e53-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18e53-113">Not supported.</span></span> |
| <span data-ttu-id="18e53-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="18e53-114">Application</span></span>                            | <span data-ttu-id="18e53-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18e53-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18e53-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18e53-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="18e53-117">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="18e53-117">Path parameters</span></span>

| <span data-ttu-id="18e53-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="18e53-118">Parameter</span></span>     | <span data-ttu-id="18e53-119">Тип</span><span class="sxs-lookup"><span data-stu-id="18e53-119">Type</span></span>   | <span data-ttu-id="18e53-120">Описание</span><span class="sxs-lookup"><span data-stu-id="18e53-120">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="18e53-121">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="18e53-121">connection-id</span></span> | <span data-ttu-id="18e53-122">string</span><span class="sxs-lookup"><span data-stu-id="18e53-122">string</span></span> | <span data-ttu-id="18e53-123">`id` Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="18e53-123">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="18e53-124">item-id</span><span class="sxs-lookup"><span data-stu-id="18e53-124">item-id</span></span>       | <span data-ttu-id="18e53-125">string</span><span class="sxs-lookup"><span data-stu-id="18e53-125">string</span></span> | <span data-ttu-id="18e53-126">Предоставляемое `id` разработчиком свойство [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="18e53-126">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="18e53-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18e53-127">Request headers</span></span>

| <span data-ttu-id="18e53-128">Имя</span><span class="sxs-lookup"><span data-stu-id="18e53-128">Name</span></span>          | <span data-ttu-id="18e53-129">Описание</span><span class="sxs-lookup"><span data-stu-id="18e53-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="18e53-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18e53-130">Authorization</span></span> | <span data-ttu-id="18e53-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18e53-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18e53-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18e53-133">Request body</span></span>

<span data-ttu-id="18e53-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18e53-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18e53-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="18e53-135">Response</span></span>

<span data-ttu-id="18e53-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="18e53-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18e53-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="18e53-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18e53-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="18e53-139">Request</span></span>

<span data-ttu-id="18e53-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18e53-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="18e53-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="18e53-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="18e53-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18e53-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="18e53-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="18e53-143">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="18e53-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="18e53-144">The following is an example of the response.</span></span>

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
