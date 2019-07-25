---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Удаление записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e597e171782a0170e378aec051f12e753970a928
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880279"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="a9be0-102">Удаление элемента из списка</span><span class="sxs-lookup"><span data-stu-id="a9be0-102">Delete an item from a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9be0-103">Удаление элемента из [списка][].</span><span class="sxs-lookup"><span data-stu-id="a9be0-103">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="a9be0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9be0-105">Permissions</span></span>

<span data-ttu-id="a9be0-106">Чтобы можно было удалить элемент, пользователь должен предоставить приложению доступ на запись к элементу, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="a9be0-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="a9be0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9be0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9be0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9be0-109">Permission type</span></span>      | <span data-ttu-id="a9be0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9be0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9be0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9be0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9be0-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9be0-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9be0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9be0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9be0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9be0-114">Not supported.</span></span>    |
|<span data-ttu-id="a9be0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9be0-115">Application</span></span> | <span data-ttu-id="a9be0-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9be0-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9be0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9be0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="a9be0-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9be0-118">Optional request headers</span></span>

| <span data-ttu-id="a9be0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a9be0-119">Name</span></span>       | <span data-ttu-id="a9be0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a9be0-120">Value</span></span> | <span data-ttu-id="a9be0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a9be0-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="a9be0-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="a9be0-122">_if-match_</span></span> | <span data-ttu-id="a9be0-123">etag</span><span class="sxs-lookup"><span data-stu-id="a9be0-123">etag</span></span>  | <span data-ttu-id="a9be0-124">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="a9be0-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="a9be0-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9be0-125">Request body</span></span>

<span data-ttu-id="a9be0-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9be0-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="a9be0-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a9be0-127">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a9be0-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9be0-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a9be0-129">C#</span><span class="sxs-lookup"><span data-stu-id="a9be0-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9be0-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="a9be0-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a9be0-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a9be0-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a9be0-132">Java</span><span class="sxs-lookup"><span data-stu-id="a9be0-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="a9be0-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9be0-133">Response</span></span>

<span data-ttu-id="a9be0-134">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="a9be0-134">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
