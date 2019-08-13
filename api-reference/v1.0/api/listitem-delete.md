---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Удаление записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
description: Удаление элемента из списка.
doc_type: apiPageType
ms.openlocfilehash: ac07e03892476ad160f76dd49ced3b2bcb63ace6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374024"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="b0be2-103">Удаление элемента из списка</span><span class="sxs-lookup"><span data-stu-id="b0be2-103">Delete an item from a list</span></span>

<span data-ttu-id="b0be2-104">Удаление элемента из [списка][].</span><span class="sxs-lookup"><span data-stu-id="b0be2-104">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="b0be2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0be2-106">Permissions</span></span>

<span data-ttu-id="b0be2-107">Чтобы можно было удалить элемент, пользователь должен предоставить приложению доступ на запись к элементу, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="b0be2-107">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="b0be2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0be2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0be2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0be2-110">Permission type</span></span>      | <span data-ttu-id="b0be2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0be2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0be2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0be2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b0be2-113">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0be2-113">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0be2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0be2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0be2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0be2-115">Not supported.</span></span>    |
|<span data-ttu-id="b0be2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0be2-116">Application</span></span> | <span data-ttu-id="b0be2-117">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0be2-117">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0be2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0be2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="b0be2-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0be2-119">Optional request headers</span></span>

| <span data-ttu-id="b0be2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b0be2-120">Name</span></span>       | <span data-ttu-id="b0be2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b0be2-121">Value</span></span> | <span data-ttu-id="b0be2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b0be2-122">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="b0be2-123">_if-match_</span><span class="sxs-lookup"><span data-stu-id="b0be2-123">_if-match_</span></span> | <span data-ttu-id="b0be2-124">etag</span><span class="sxs-lookup"><span data-stu-id="b0be2-124">etag</span></span>  | <span data-ttu-id="b0be2-125">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="b0be2-125">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="b0be2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0be2-126">Request body</span></span>

<span data-ttu-id="b0be2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0be2-127">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="b0be2-128">Пример</span><span class="sxs-lookup"><span data-stu-id="b0be2-128">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b0be2-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0be2-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0be2-130">C#</span><span class="sxs-lookup"><span data-stu-id="b0be2-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0be2-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0be2-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0be2-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b0be2-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b0be2-133">Java</span><span class="sxs-lookup"><span data-stu-id="b0be2-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-item-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="b0be2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0be2-134">Response</span></span>

<span data-ttu-id="b0be2-135">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="b0be2-135">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
