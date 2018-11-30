---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Удаление страницы на сайте SharePoint
ms.openlocfilehash: c537acec2e205ffd556a35789f75be95e2b94017
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076730"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="1bc70-102">Удалить страницу в списке страниц сайта узла</span><span class="sxs-lookup"><span data-stu-id="1bc70-102">Delete page from the site pages list of a site</span></span>

> <span data-ttu-id="1bc70-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1bc70-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1bc70-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bc70-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1bc70-105">Удаляет [sitePage][] страниц сайта [списка][] на [сайте][].</span><span class="sxs-lookup"><span data-stu-id="1bc70-105">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="1bc70-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bc70-109">Permissions</span></span>

<span data-ttu-id="1bc70-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bc70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="1bc70-112">**Примечание:** Для удаления элемента, пользователю должно быть предоставлено доступ на запись приложения для удаляемого элемента.</span><span class="sxs-lookup"><span data-stu-id="1bc70-112">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="1bc70-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bc70-113">Permission type</span></span>      | <span data-ttu-id="1bc70-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bc70-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bc70-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bc70-115">Delegated (work or school account)</span></span> | <span data-ttu-id="1bc70-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bc70-116">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1bc70-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bc70-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bc70-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bc70-118">Not supported.</span></span>    |
|<span data-ttu-id="1bc70-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bc70-119">Application</span></span> | <span data-ttu-id="1bc70-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bc70-120">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bc70-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bc70-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="1bc70-122">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bc70-122">Optional request headers</span></span>

| <span data-ttu-id="1bc70-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1bc70-123">Name</span></span>       | <span data-ttu-id="1bc70-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1bc70-124">Value</span></span> | <span data-ttu-id="1bc70-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1bc70-125">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="1bc70-126">_if-match_</span><span class="sxs-lookup"><span data-stu-id="1bc70-126">_if-match_</span></span> | <span data-ttu-id="1bc70-127">etag</span><span class="sxs-lookup"><span data-stu-id="1bc70-127">etag</span></span>  | <span data-ttu-id="1bc70-128">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="1bc70-128">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="1bc70-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1bc70-129">Request body</span></span>

<span data-ttu-id="1bc70-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bc70-130">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="1bc70-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1bc70-131">Response</span></span>

<span data-ttu-id="1bc70-132">Успешно завершена, этот вызов возвращает `204 No Content` уведомление о том, что ресурс был удален и возникла ничего не возвращает.</span><span class="sxs-lookup"><span data-stu-id="1bc70-132">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="1bc70-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1bc70-133">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="1bc70-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bc70-134">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="1bc70-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="1bc70-135">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete"
} -->
