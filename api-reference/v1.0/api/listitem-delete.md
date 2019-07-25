---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Удаление записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fd472f685b5fc35809f3516ed1b3f13e1f77e9ae
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880733"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="b4542-102">Удаление элемента из списка</span><span class="sxs-lookup"><span data-stu-id="b4542-102">Delete an item from a list</span></span>

<span data-ttu-id="b4542-103">Удаление элемента из [списка][].</span><span class="sxs-lookup"><span data-stu-id="b4542-103">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="b4542-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4542-105">Permissions</span></span>

<span data-ttu-id="b4542-106">Чтобы можно было удалить элемент, пользователь должен предоставить приложению доступ на запись к элементу, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="b4542-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="b4542-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4542-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4542-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4542-109">Permission type</span></span>      | <span data-ttu-id="b4542-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4542-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4542-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4542-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b4542-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4542-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4542-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4542-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4542-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4542-114">Not supported.</span></span>    |
|<span data-ttu-id="b4542-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4542-115">Application</span></span> | <span data-ttu-id="b4542-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4542-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4542-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4542-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="b4542-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4542-118">Optional request headers</span></span>

| <span data-ttu-id="b4542-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b4542-119">Name</span></span>       | <span data-ttu-id="b4542-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b4542-120">Value</span></span> | <span data-ttu-id="b4542-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b4542-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="b4542-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="b4542-122">_if-match_</span></span> | <span data-ttu-id="b4542-123">etag</span><span class="sxs-lookup"><span data-stu-id="b4542-123">etag</span></span>  | <span data-ttu-id="b4542-124">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="b4542-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="b4542-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4542-125">Request body</span></span>

<span data-ttu-id="b4542-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4542-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="b4542-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b4542-127">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b4542-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4542-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4542-129">C#</span><span class="sxs-lookup"><span data-stu-id="b4542-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4542-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="b4542-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4542-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b4542-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b4542-132">Java</span><span class="sxs-lookup"><span data-stu-id="b4542-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-item-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="b4542-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4542-133">Response</span></span>

<span data-ttu-id="b4542-134">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="b4542-134">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
