---
author: JeremyKelley
description: Удаление элемента из списка.
ms.date: 09/11/2017
title: Удаление записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 39f0d032277cf38c50c51df99d4a65ac44cf8740
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415409"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="678f6-103">Удаление элемента из списка</span><span class="sxs-lookup"><span data-stu-id="678f6-103">Delete an item from a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="678f6-104">Удаление элемента из [списка][].</span><span class="sxs-lookup"><span data-stu-id="678f6-104">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="678f6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="678f6-106">Permissions</span></span>

<span data-ttu-id="678f6-107">Чтобы можно было удалить элемент, пользователь должен предоставить приложению доступ на запись к элементу, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="678f6-107">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="678f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="678f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="678f6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="678f6-110">Permission type</span></span>      | <span data-ttu-id="678f6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="678f6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="678f6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="678f6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="678f6-113">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="678f6-113">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="678f6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="678f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="678f6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="678f6-115">Not supported.</span></span>    |
|<span data-ttu-id="678f6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="678f6-116">Application</span></span> | <span data-ttu-id="678f6-117">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="678f6-117">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="678f6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="678f6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="678f6-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="678f6-119">Optional request headers</span></span>

| <span data-ttu-id="678f6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="678f6-120">Name</span></span>       | <span data-ttu-id="678f6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="678f6-121">Value</span></span> | <span data-ttu-id="678f6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="678f6-122">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="678f6-123">_if-match_</span><span class="sxs-lookup"><span data-stu-id="678f6-123">_if-match_</span></span> | <span data-ttu-id="678f6-124">etag</span><span class="sxs-lookup"><span data-stu-id="678f6-124">etag</span></span>  | <span data-ttu-id="678f6-125">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="678f6-125">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="678f6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="678f6-126">Request body</span></span>

<span data-ttu-id="678f6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="678f6-127">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="678f6-128">Пример</span><span class="sxs-lookup"><span data-stu-id="678f6-128">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="678f6-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="678f6-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="678f6-130">C#</span><span class="sxs-lookup"><span data-stu-id="678f6-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="678f6-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="678f6-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="678f6-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="678f6-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="678f6-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="678f6-133">Response</span></span>

<span data-ttu-id="678f6-134">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="678f6-134">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
