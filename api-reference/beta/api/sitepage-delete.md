---
author: rahmit
description: Удаляет объект Ситепаже из списка страниц сайта на сайте.
ms.date: 05/07/2018
title: Удаление страницы с сайта SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bdf3dacabb99d5dfcfe47dcb954ff1cfd0b62ccb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977862"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="a7345-103">Удаление страницы из списка страниц сайта</span><span class="sxs-lookup"><span data-stu-id="a7345-103">Delete page from the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7345-104">Удаляет объект [ситепаже][] из [списка][] страниц сайта на [сайте][].</span><span class="sxs-lookup"><span data-stu-id="a7345-104">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="a7345-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7345-108">Permissions</span></span>

<span data-ttu-id="a7345-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7345-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="a7345-111">**Примечание:** Чтобы удалить элемент, пользователь должен получить доступ к приложению на запись для элемента, который требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="a7345-111">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="a7345-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7345-112">Permission type</span></span>      | <span data-ttu-id="a7345-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7345-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7345-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7345-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a7345-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7345-115">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a7345-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7345-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7345-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7345-117">Not supported.</span></span>    |
|<span data-ttu-id="a7345-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7345-118">Application</span></span> | <span data-ttu-id="a7345-119">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7345-119">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7345-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7345-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="a7345-121">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7345-121">Optional request headers</span></span>

| <span data-ttu-id="a7345-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a7345-122">Name</span></span>       | <span data-ttu-id="a7345-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a7345-123">Value</span></span> | <span data-ttu-id="a7345-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a7345-124">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="a7345-125">_if-match_</span><span class="sxs-lookup"><span data-stu-id="a7345-125">_if-match_</span></span> | <span data-ttu-id="a7345-126">etag</span><span class="sxs-lookup"><span data-stu-id="a7345-126">etag</span></span>  | <span data-ttu-id="a7345-127">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="a7345-127">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="a7345-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7345-128">Request body</span></span>

<span data-ttu-id="a7345-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7345-129">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="a7345-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7345-130">Response</span></span>

<span data-ttu-id="a7345-131">В случае успешного выполнения этот вызов возвращает `204 No Content` ответ, указывающий на то, что ресурс был удален и что не было возвращено.</span><span class="sxs-lookup"><span data-stu-id="a7345-131">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="a7345-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a7345-132">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="a7345-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7345-133">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="a7345-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7345-134">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete",
  "suppressions": []
}
-->
