---
author: JeremyKelley
description: Удаление элемента из списка.
ms.date: 09/11/2017
title: Удаление записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f392ec8699fb2e079446c6f72c12c844db62852c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457145"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="a8348-103">Удаление элемента из списка</span><span class="sxs-lookup"><span data-stu-id="a8348-103">Delete an item from a list</span></span>

<span data-ttu-id="a8348-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a8348-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8348-105">Удаление элемента из [списка][].</span><span class="sxs-lookup"><span data-stu-id="a8348-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="a8348-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8348-107">Permissions</span></span>

<span data-ttu-id="a8348-108">Чтобы можно было удалить элемент, пользователь должен предоставить приложению доступ на запись к элементу, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="a8348-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="a8348-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8348-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8348-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8348-111">Permission type</span></span>      | <span data-ttu-id="a8348-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8348-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8348-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8348-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a8348-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8348-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a8348-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8348-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8348-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8348-116">Not supported.</span></span>    |
|<span data-ttu-id="a8348-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8348-117">Application</span></span> | <span data-ttu-id="a8348-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8348-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8348-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8348-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="a8348-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8348-120">Optional request headers</span></span>

| <span data-ttu-id="a8348-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a8348-121">Name</span></span>       | <span data-ttu-id="a8348-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a8348-122">Value</span></span> | <span data-ttu-id="a8348-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a8348-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="a8348-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="a8348-124">_if-match_</span></span> | <span data-ttu-id="a8348-125">etag</span><span class="sxs-lookup"><span data-stu-id="a8348-125">etag</span></span>  | <span data-ttu-id="a8348-126">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="a8348-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="a8348-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8348-127">Request body</span></span>

<span data-ttu-id="a8348-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8348-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="a8348-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a8348-129">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="a8348-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8348-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="a8348-131">C#</span><span class="sxs-lookup"><span data-stu-id="a8348-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8348-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8348-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8348-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8348-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="a8348-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8348-134">Response</span></span>

<span data-ttu-id="a8348-135">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="a8348-135">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
  ]
}
-->
