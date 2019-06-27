---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Удаление записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 891e85f120fc9521a38469b8ed6852b9d36c9b09
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264563"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="2d476-102">Удаление элемента из списка</span><span class="sxs-lookup"><span data-stu-id="2d476-102">Delete an item from a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d476-103">Удаление элемента из [списка][].</span><span class="sxs-lookup"><span data-stu-id="2d476-103">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="2d476-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d476-105">Permissions</span></span>

<span data-ttu-id="2d476-106">Чтобы можно было удалить элемент, пользователь должен предоставить приложению доступ на запись к элементу, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="2d476-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="2d476-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d476-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d476-109">Permission type</span></span>      | <span data-ttu-id="2d476-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d476-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d476-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d476-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d476-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d476-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2d476-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d476-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d476-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d476-114">Not supported.</span></span>    |
|<span data-ttu-id="2d476-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d476-115">Application</span></span> | <span data-ttu-id="2d476-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d476-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d476-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d476-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="2d476-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d476-118">Optional request headers</span></span>

| <span data-ttu-id="2d476-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2d476-119">Name</span></span>       | <span data-ttu-id="2d476-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2d476-120">Value</span></span> | <span data-ttu-id="2d476-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2d476-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="2d476-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="2d476-122">_if-match_</span></span> | <span data-ttu-id="2d476-123">etag</span><span class="sxs-lookup"><span data-stu-id="2d476-123">etag</span></span>  | <span data-ttu-id="2d476-124">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="2d476-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="2d476-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2d476-125">Request body</span></span>

<span data-ttu-id="2d476-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d476-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="2d476-127">Пример</span><span class="sxs-lookup"><span data-stu-id="2d476-127">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="2d476-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d476-128">Response</span></span>

<span data-ttu-id="2d476-129">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="2d476-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2d476-130">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="2d476-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2d476-131">C#</span><span class="sxs-lookup"><span data-stu-id="2d476-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d476-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="2d476-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2d476-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2d476-133">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/listitem-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/listitem-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
