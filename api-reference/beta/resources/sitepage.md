---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
ms.openlocfilehash: 65cfe61dadd1708abffe2d01abbbb15f40d158ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080470"
---
# <a name="sitepage-resource"></a><span data-ttu-id="1b40e-102">sitePage ресурсов</span><span class="sxs-lookup"><span data-stu-id="1b40e-102">sitePage resource</span></span>

> <span data-ttu-id="1b40e-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b40e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b40e-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b40e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b40e-105">Этот ресурс представляет страницу SitePages [списка][].</span><span class="sxs-lookup"><span data-stu-id="1b40e-105">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="1b40e-106">Он содержит заголовок, макет и коллекцию s [веб-части][].</span><span class="sxs-lookup"><span data-stu-id="1b40e-106">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="1b40e-107">Задачи на странице</span><span class="sxs-lookup"><span data-stu-id="1b40e-107">Tasks on a page</span></span>

<span data-ttu-id="1b40e-108">Для **sitePage** ресурсов доступны следующие задачи.</span><span class="sxs-lookup"><span data-stu-id="1b40e-108">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="1b40e-109">Всех приведенных ниже примерах относительны [сайта][], например: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="1b40e-109">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="1b40e-110">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="1b40e-110">Common task</span></span>                     | <span data-ttu-id="1b40e-111">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="1b40e-111">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="1b40e-112">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="1b40e-112">[List pages][]</span></span>                  | <span data-ttu-id="1b40e-113">Получение /pages</span><span class="sxs-lookup"><span data-stu-id="1b40e-113">GET /pages</span></span>
| <span data-ttu-id="1b40e-114">[Получение страницы][]</span><span class="sxs-lookup"><span data-stu-id="1b40e-114">[Get page][]</span></span>                    | <span data-ttu-id="1b40e-115">Получение /pages/ {идентификатор страницы}</span><span class="sxs-lookup"><span data-stu-id="1b40e-115">GET /pages/{page-id}</span></span>
| <span data-ttu-id="1b40e-116">[Create][]</span><span class="sxs-lookup"><span data-stu-id="1b40e-116">[Create][]</span></span>                      | <span data-ttu-id="1b40e-117">POST /pages</span><span class="sxs-lookup"><span data-stu-id="1b40e-117">POST /pages</span></span>
| <span data-ttu-id="1b40e-118">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="1b40e-118">[Delete][]</span></span>                      | <span data-ttu-id="1b40e-119">Удаление /pages/ {идентификатор страницы}</span><span class="sxs-lookup"><span data-stu-id="1b40e-119">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="1b40e-120">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="1b40e-120">[Publish][]</span></span>                     | <span data-ttu-id="1b40e-121">Учет /pages/ {идентификатор страницы} аудио- и публикация</span><span class="sxs-lookup"><span data-stu-id="1b40e-121">POST /pages/{page-id}/publish</span></span>

[Перечисление страниц]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Получение страницы]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="1b40e-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b40e-127">JSON representation</span></span>

<span data-ttu-id="1b40e-128">Ниже представлена JSON **sitePage** ресурса.</span><span class="sxs-lookup"><span data-stu-id="1b40e-128">Here is a JSON representation of a **sitePage** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayout": "Article",
  "webParts": [{ "@odata.type": "microsoft.graph.sitePageWebParts" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

  /* inherited from baseItem */
  "id": "string",
  "name": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="1b40e-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b40e-129">Properties</span></span>

<span data-ttu-id="1b40e-130">Ресурс **sitePage** имеет следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="1b40e-130">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="1b40e-131">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1b40e-131">Property name</span></span>    | <span data-ttu-id="1b40e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="1b40e-132">Type</span></span>                         | <span data-ttu-id="1b40e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="1b40e-133">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="1b40e-134">contentType</span><span class="sxs-lookup"><span data-stu-id="1b40e-134">contentType</span></span>      | <span data-ttu-id="1b40e-135">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="1b40e-135">[contentTypeInfo][]</span></span>          | <span data-ttu-id="1b40e-136">Тип страницы содержимого.</span><span class="sxs-lookup"><span data-stu-id="1b40e-136">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="1b40e-137">Контент страницы</span><span class="sxs-lookup"><span data-stu-id="1b40e-137">Page Content</span></span>

<span data-ttu-id="1b40e-138">Ресурс **sitePage** имеет следующие поля содержимого.</span><span class="sxs-lookup"><span data-stu-id="1b40e-138">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="1b40e-139">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1b40e-139">Property name</span></span>      | <span data-ttu-id="1b40e-140">Тип</span><span class="sxs-lookup"><span data-stu-id="1b40e-140">Type</span></span>                       | <span data-ttu-id="1b40e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="1b40e-141">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="1b40e-142">должности.</span><span class="sxs-lookup"><span data-stu-id="1b40e-142">title</span></span>              | <span data-ttu-id="1b40e-143">строка</span><span class="sxs-lookup"><span data-stu-id="1b40e-143">string</span></span>                     | <span data-ttu-id="1b40e-144">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="1b40e-144">The title of the page.</span></span>
| <span data-ttu-id="1b40e-145">pageLayout</span><span class="sxs-lookup"><span data-stu-id="1b40e-145">pageLayout</span></span>         | <span data-ttu-id="1b40e-146">string</span><span class="sxs-lookup"><span data-stu-id="1b40e-146">string</span></span>                     | <span data-ttu-id="1b40e-147">Имя страницы макета страницы.</span><span class="sxs-lookup"><span data-stu-id="1b40e-147">The name of the page layout of the page.</span></span>
| <span data-ttu-id="1b40e-148">веб-части</span><span class="sxs-lookup"><span data-stu-id="1b40e-148">webParts</span></span>           | <span data-ttu-id="1b40e-149">[веб-части][]</span><span class="sxs-lookup"><span data-stu-id="1b40e-149">[webPart][]</span></span>                | <span data-ttu-id="1b40e-150">Веб-частей на странице.</span><span class="sxs-lookup"><span data-stu-id="1b40e-150">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="1b40e-151">Создание метаданных</span><span class="sxs-lookup"><span data-stu-id="1b40e-151">Authoring Metadata</span></span>

<span data-ttu-id="1b40e-152">Ресурс **sitePage** имеет следующие метаданные, связанные с разработки.</span><span class="sxs-lookup"><span data-stu-id="1b40e-152">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="1b40e-153">Свойство publishingState будет отражают состояние как извлечь или опубликовать разработки страниц.</span><span class="sxs-lookup"><span data-stu-id="1b40e-153">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="1b40e-154">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1b40e-154">Property name</span></span>          | <span data-ttu-id="1b40e-155">Тип</span><span class="sxs-lookup"><span data-stu-id="1b40e-155">Type</span></span>                   | <span data-ttu-id="1b40e-156">Description</span><span class="sxs-lookup"><span data-stu-id="1b40e-156">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="1b40e-157">publishingState</span><span class="sxs-lookup"><span data-stu-id="1b40e-157">publishingState</span></span>        | <span data-ttu-id="1b40e-158">[publicationFacet][].</span><span class="sxs-lookup"><span data-stu-id="1b40e-158">[publicationFacet][]</span></span>   | <span data-ttu-id="1b40e-159">Состояния публикации и MM.mm версия страницы.</span><span class="sxs-lookup"><span data-stu-id="1b40e-159">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="1b40e-160">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="1b40e-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="1b40e-161">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1b40e-161">Property name</span></span>        | <span data-ttu-id="1b40e-162">Тип</span><span class="sxs-lookup"><span data-stu-id="1b40e-162">Type</span></span>              | <span data-ttu-id="1b40e-163">Описание</span><span class="sxs-lookup"><span data-stu-id="1b40e-163">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="1b40e-164">id</span><span class="sxs-lookup"><span data-stu-id="1b40e-164">id</span></span>                   | <span data-ttu-id="1b40e-165">строка</span><span class="sxs-lookup"><span data-stu-id="1b40e-165">string</span></span>            | <span data-ttu-id="1b40e-p105">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b40e-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="1b40e-168">name</span><span class="sxs-lookup"><span data-stu-id="1b40e-168">name</span></span>                 | <span data-ttu-id="1b40e-169">строка</span><span class="sxs-lookup"><span data-stu-id="1b40e-169">string</span></span>            | <span data-ttu-id="1b40e-170">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="1b40e-170">The name / title of the item.</span></span>
| <span data-ttu-id="1b40e-171">createdBy</span><span class="sxs-lookup"><span data-stu-id="1b40e-171">createdBy</span></span>            | <span data-ttu-id="1b40e-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1b40e-172">[identitySet][]</span></span>   | <span data-ttu-id="1b40e-173">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="1b40e-173">Identity of the creator of this item.</span></span> <span data-ttu-id="1b40e-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b40e-174">Read-only.</span></span>
| <span data-ttu-id="1b40e-175">eTag</span><span class="sxs-lookup"><span data-stu-id="1b40e-175">eTag</span></span>                 | <span data-ttu-id="1b40e-176">string</span><span class="sxs-lookup"><span data-stu-id="1b40e-176">string</span></span>            | <span data-ttu-id="1b40e-p107">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b40e-p107">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="1b40e-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1b40e-179">lastModifiedBy</span></span>       | <span data-ttu-id="1b40e-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1b40e-180">[identitySet][]</span></span>   | <span data-ttu-id="1b40e-181">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="1b40e-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="1b40e-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b40e-182">Read-only.</span></span>
| <span data-ttu-id="1b40e-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b40e-183">lastModifiedDateTime</span></span> | <span data-ttu-id="1b40e-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b40e-184">DateTimeOffset</span></span>    | <span data-ttu-id="1b40e-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b40e-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="1b40e-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="1b40e-187">parentReference</span></span>      | <span data-ttu-id="1b40e-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="1b40e-188">[itemReference][]</span></span> | <span data-ttu-id="1b40e-p110">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b40e-p110">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="1b40e-191">webUrl</span><span class="sxs-lookup"><span data-stu-id="1b40e-191">webUrl</span></span>               | <span data-ttu-id="1b40e-192">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="1b40e-192">string (url)</span></span>      | <span data-ttu-id="1b40e-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b40e-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="1b40e-195">Связи</span><span class="sxs-lookup"><span data-stu-id="1b40e-195">Relationships</span></span>

<span data-ttu-id="1b40e-196">Ресурс **sitePage** не имеет отношения к другим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="1b40e-196">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md.
[site]: site.md
[веб-части]: webpart.md
[webPart]: webpart.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  }
} -->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
