---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Удаление записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
description: Удаление элемента из списка.
doc_type: apiPageType
ms.openlocfilehash: d2d7fd332d0a79be2088c24e6704fc9975d3924e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057290"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="24f14-103">Удаление элемента из списка</span><span class="sxs-lookup"><span data-stu-id="24f14-103">Delete an item from a list</span></span>

<span data-ttu-id="24f14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24f14-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24f14-105">Удаление элемента из [списка][].</span><span class="sxs-lookup"><span data-stu-id="24f14-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="24f14-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24f14-107">Permissions</span></span>

<span data-ttu-id="24f14-108">Чтобы можно было удалить элемент, пользователь должен предоставить приложению доступ на запись к элементу, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="24f14-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="24f14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24f14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24f14-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24f14-111">Permission type</span></span>      | <span data-ttu-id="24f14-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24f14-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24f14-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24f14-113">Delegated (work or school account)</span></span> | <span data-ttu-id="24f14-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24f14-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="24f14-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24f14-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24f14-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24f14-116">Not supported.</span></span>    |
|<span data-ttu-id="24f14-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24f14-117">Application</span></span> | <span data-ttu-id="24f14-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24f14-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24f14-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24f14-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="24f14-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24f14-120">Optional request headers</span></span>

| <span data-ttu-id="24f14-121">Имя</span><span class="sxs-lookup"><span data-stu-id="24f14-121">Name</span></span>       | <span data-ttu-id="24f14-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24f14-122">Value</span></span> | <span data-ttu-id="24f14-123">Описание</span><span class="sxs-lookup"><span data-stu-id="24f14-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="24f14-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="24f14-124">_if-match_</span></span> | <span data-ttu-id="24f14-125">etag</span><span class="sxs-lookup"><span data-stu-id="24f14-125">etag</span></span>  | <span data-ttu-id="24f14-126">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="24f14-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="24f14-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24f14-127">Request body</span></span>

<span data-ttu-id="24f14-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24f14-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="24f14-129">Пример</span><span class="sxs-lookup"><span data-stu-id="24f14-129">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="24f14-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="24f14-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="24f14-131">C#</span><span class="sxs-lookup"><span data-stu-id="24f14-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24f14-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24f14-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24f14-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24f14-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="24f14-134">Java</span><span class="sxs-lookup"><span data-stu-id="24f14-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-item-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="24f14-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="24f14-135">Response</span></span>

<span data-ttu-id="24f14-136">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="24f14-136">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
  ]
} -->

