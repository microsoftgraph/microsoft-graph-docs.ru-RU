---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Удаление записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
description: Удаление элемента из списка.
doc_type: apiPageType
ms.openlocfilehash: 9f87510a1b5a773f49ad3a9bb265391647de3ce3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023155"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="bf9c4-103">Удаление элемента из списка</span><span class="sxs-lookup"><span data-stu-id="bf9c4-103">Delete an item from a list</span></span>

<span data-ttu-id="bf9c4-104">Удаление элемента из [списка][].</span><span class="sxs-lookup"><span data-stu-id="bf9c4-104">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="bf9c4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf9c4-106">Permissions</span></span>

<span data-ttu-id="bf9c4-107">Чтобы можно было удалить элемент, пользователь должен предоставить приложению доступ на запись к элементу, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="bf9c4-107">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="bf9c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf9c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf9c4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf9c4-110">Permission type</span></span>      | <span data-ttu-id="bf9c4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf9c4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf9c4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf9c4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bf9c4-113">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf9c4-113">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bf9c4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf9c4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf9c4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9c4-115">Not supported.</span></span>    |
|<span data-ttu-id="bf9c4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf9c4-116">Application</span></span> | <span data-ttu-id="bf9c4-117">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf9c4-117">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf9c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf9c4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="bf9c4-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf9c4-119">Optional request headers</span></span>

| <span data-ttu-id="bf9c4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bf9c4-120">Name</span></span>       | <span data-ttu-id="bf9c4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bf9c4-121">Value</span></span> | <span data-ttu-id="bf9c4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bf9c4-122">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="bf9c4-123">_if-match_</span><span class="sxs-lookup"><span data-stu-id="bf9c4-123">_if-match_</span></span> | <span data-ttu-id="bf9c4-124">etag</span><span class="sxs-lookup"><span data-stu-id="bf9c4-124">etag</span></span>  | <span data-ttu-id="bf9c4-125">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="bf9c4-125">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="bf9c4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bf9c4-126">Request body</span></span>

<span data-ttu-id="bf9c4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf9c4-127">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="bf9c4-128">Пример</span><span class="sxs-lookup"><span data-stu-id="bf9c4-128">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bf9c4-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf9c4-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bf9c4-130">C#</span><span class="sxs-lookup"><span data-stu-id="bf9c4-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf9c4-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="bf9c4-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bf9c4-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bf9c4-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bf9c4-133">Java</span><span class="sxs-lookup"><span data-stu-id="bf9c4-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-item-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="bf9c4-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf9c4-134">Response</span></span>

<span data-ttu-id="bf9c4-135">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="bf9c4-135">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
