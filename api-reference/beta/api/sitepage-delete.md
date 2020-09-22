---
author: rahmit
description: Удаляет объект Ситепаже из списка страниц сайта на сайте.
ms.date: 05/07/2018
title: Удаление страницы с сайта SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d573553ee87b70adfd1f2cde575ce6182dedf8b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044489"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="eb108-103">Удаление страницы из списка страниц сайта</span><span class="sxs-lookup"><span data-stu-id="eb108-103">Delete page from the site pages list of a site</span></span>

<span data-ttu-id="eb108-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb108-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb108-105">Удаляет объект [ситепаже][] из [списка][] страниц сайта на [сайте][].</span><span class="sxs-lookup"><span data-stu-id="eb108-105">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="eb108-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb108-109">Permissions</span></span>

<span data-ttu-id="eb108-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb108-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="eb108-112">**Примечание:** Чтобы удалить элемент, пользователь должен получить доступ к приложению на запись для элемента, который требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="eb108-112">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="eb108-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb108-113">Permission type</span></span>      | <span data-ttu-id="eb108-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb108-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb108-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb108-115">Delegated (work or school account)</span></span> | <span data-ttu-id="eb108-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb108-116">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb108-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb108-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb108-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb108-118">Not supported.</span></span>    |
|<span data-ttu-id="eb108-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb108-119">Application</span></span> | <span data-ttu-id="eb108-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb108-120">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb108-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb108-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="eb108-122">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb108-122">Optional request headers</span></span>

| <span data-ttu-id="eb108-123">Имя</span><span class="sxs-lookup"><span data-stu-id="eb108-123">Name</span></span>       | <span data-ttu-id="eb108-124">Значение</span><span class="sxs-lookup"><span data-stu-id="eb108-124">Value</span></span> | <span data-ttu-id="eb108-125">Описание</span><span class="sxs-lookup"><span data-stu-id="eb108-125">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="eb108-126">_if-match_</span><span class="sxs-lookup"><span data-stu-id="eb108-126">_if-match_</span></span> | <span data-ttu-id="eb108-127">etag</span><span class="sxs-lookup"><span data-stu-id="eb108-127">etag</span></span>  | <span data-ttu-id="eb108-128">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="eb108-128">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="eb108-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb108-129">Request body</span></span>

<span data-ttu-id="eb108-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb108-130">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="eb108-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb108-131">Response</span></span>

<span data-ttu-id="eb108-132">В случае успешного выполнения этот вызов возвращает `204 No Content` ответ, указывающий на то, что ресурс был удален и что не было возвращено.</span><span class="sxs-lookup"><span data-stu-id="eb108-132">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="eb108-133">Пример</span><span class="sxs-lookup"><span data-stu-id="eb108-133">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="eb108-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb108-134">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="eb108-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb108-135">Response</span></span>

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


