---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Удаление записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bbc9d7b98cc532a8bed10da622cb49509d339d5a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598026"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="51162-102">Удаление элемента из списка</span><span class="sxs-lookup"><span data-stu-id="51162-102">Delete an item from a list</span></span>

<span data-ttu-id="51162-103">Удаление элемента из [списка][].</span><span class="sxs-lookup"><span data-stu-id="51162-103">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="51162-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51162-105">Permissions</span></span>

<span data-ttu-id="51162-106">Чтобы можно было удалить элемент, пользователь должен предоставить приложению доступ на запись к элементу, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="51162-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="51162-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51162-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51162-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51162-109">Permission type</span></span>      | <span data-ttu-id="51162-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51162-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51162-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51162-111">Delegated (work or school account)</span></span> | <span data-ttu-id="51162-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51162-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="51162-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51162-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51162-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51162-114">Not supported.</span></span>    |
|<span data-ttu-id="51162-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51162-115">Application</span></span> | <span data-ttu-id="51162-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51162-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51162-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51162-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="51162-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51162-118">Optional request headers</span></span>

| <span data-ttu-id="51162-119">Имя</span><span class="sxs-lookup"><span data-stu-id="51162-119">Name</span></span>       | <span data-ttu-id="51162-120">Значение</span><span class="sxs-lookup"><span data-stu-id="51162-120">Value</span></span> | <span data-ttu-id="51162-121">Описание</span><span class="sxs-lookup"><span data-stu-id="51162-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="51162-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="51162-122">_if-match_</span></span> | <span data-ttu-id="51162-123">etag</span><span class="sxs-lookup"><span data-stu-id="51162-123">etag</span></span>  | <span data-ttu-id="51162-124">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="51162-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="51162-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51162-125">Request body</span></span>

<span data-ttu-id="51162-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51162-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="51162-127">Пример</span><span class="sxs-lookup"><span data-stu-id="51162-127">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="51162-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="51162-128">Response</span></span>

<span data-ttu-id="51162-129">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="51162-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="51162-130">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="51162-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="51162-131">C#</span><span class="sxs-lookup"><span data-stu-id="51162-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51162-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51162-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
