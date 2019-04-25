---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Удаление страницы с сайта SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f855942288556fdf07e2b3af78408976c34eb052
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537135"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="4a001-102">Удаление страницы из списка страниц сайта</span><span class="sxs-lookup"><span data-stu-id="4a001-102">Delete page from the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a001-103">Удаляет объект [ситепаже][] из [списка][] страниц сайта на [сайте][].</span><span class="sxs-lookup"><span data-stu-id="4a001-103">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="4a001-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a001-107">Permissions</span></span>

<span data-ttu-id="4a001-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a001-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="4a001-110">**Примечание:** Чтобы удалить элемент, пользователь должен получить доступ к приложению на запись для элемента, который требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="4a001-110">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="4a001-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a001-111">Permission type</span></span>      | <span data-ttu-id="4a001-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a001-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a001-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a001-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4a001-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a001-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a001-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a001-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a001-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a001-116">Not supported.</span></span>    |
|<span data-ttu-id="4a001-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a001-117">Application</span></span> | <span data-ttu-id="4a001-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a001-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a001-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a001-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="4a001-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a001-120">Optional request headers</span></span>

| <span data-ttu-id="4a001-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4a001-121">Name</span></span>       | <span data-ttu-id="4a001-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4a001-122">Value</span></span> | <span data-ttu-id="4a001-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4a001-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="4a001-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="4a001-124">_if-match_</span></span> | <span data-ttu-id="4a001-125">etag</span><span class="sxs-lookup"><span data-stu-id="4a001-125">etag</span></span>  | <span data-ttu-id="4a001-126">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="4a001-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="4a001-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a001-127">Request body</span></span>

<span data-ttu-id="4a001-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a001-128">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="4a001-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a001-129">Response</span></span>

<span data-ttu-id="4a001-130">В случае успешного выполнения этот вызов возвращает `204 No Content` ответ, указывающий на то, что ресурс был удален и что не было возвращено.</span><span class="sxs-lookup"><span data-stu-id="4a001-130">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="4a001-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4a001-131">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="4a001-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a001-132">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="4a001-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a001-133">Response</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
