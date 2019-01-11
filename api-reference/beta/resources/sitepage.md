---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.openlocfilehash: d4673138106e23afedb5ff0f28d8ce72fa2797b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871493"
---
# <a name="sitepage-resource"></a><span data-ttu-id="7fcfa-102">sitePage ресурсов</span><span class="sxs-lookup"><span data-stu-id="7fcfa-102">sitePage resource</span></span>

> <span data-ttu-id="7fcfa-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fcfa-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7fcfa-105">Этот ресурс представляет страницу SitePages [списка][].</span><span class="sxs-lookup"><span data-stu-id="7fcfa-105">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="7fcfa-106">Он содержит заголовок, макет и коллекцию s [веб-части][].</span><span class="sxs-lookup"><span data-stu-id="7fcfa-106">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="7fcfa-107">Задачи на странице</span><span class="sxs-lookup"><span data-stu-id="7fcfa-107">Tasks on a page</span></span>

<span data-ttu-id="7fcfa-108">Для **sitePage** ресурсов доступны следующие задачи.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-108">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="7fcfa-109">Всех приведенных ниже примерах относительны [сайта][], например: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-109">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="7fcfa-110">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="7fcfa-110">Common task</span></span>                     | <span data-ttu-id="7fcfa-111">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="7fcfa-111">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="7fcfa-112">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="7fcfa-112">[List pages][]</span></span>                  | <span data-ttu-id="7fcfa-113">Получение /pages</span><span class="sxs-lookup"><span data-stu-id="7fcfa-113">GET /pages</span></span>
| <span data-ttu-id="7fcfa-114">[Получение страницы][]</span><span class="sxs-lookup"><span data-stu-id="7fcfa-114">[Get page][]</span></span>                    | <span data-ttu-id="7fcfa-115">Получение /pages/ {идентификатор страницы}</span><span class="sxs-lookup"><span data-stu-id="7fcfa-115">GET /pages/{page-id}</span></span>
| <span data-ttu-id="7fcfa-116">[создание][];</span><span class="sxs-lookup"><span data-stu-id="7fcfa-116">[Create][]</span></span>                      | <span data-ttu-id="7fcfa-117">POST /pages</span><span class="sxs-lookup"><span data-stu-id="7fcfa-117">POST /pages</span></span>
| <span data-ttu-id="7fcfa-118">[удаление][];</span><span class="sxs-lookup"><span data-stu-id="7fcfa-118">[Delete][]</span></span>                      | <span data-ttu-id="7fcfa-119">Удаление /pages/ {идентификатор страницы}</span><span class="sxs-lookup"><span data-stu-id="7fcfa-119">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="7fcfa-120">[публикация][];</span><span class="sxs-lookup"><span data-stu-id="7fcfa-120">[Publish][]</span></span>                     | <span data-ttu-id="7fcfa-121">Учет /pages/ {идентификатор страницы} аудио- и публикация</span><span class="sxs-lookup"><span data-stu-id="7fcfa-121">POST /pages/{page-id}/publish</span></span>

[Перечисление страниц]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Получение страницы]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Создание]: ../api/sitepage-create.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[публикация]: ../api/sitepage-publish.md;
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="7fcfa-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7fcfa-127">JSON representation</span></span>

<span data-ttu-id="7fcfa-128">Ниже представлена JSON **sitePage** ресурса.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-128">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7fcfa-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="7fcfa-129">Properties</span></span>

<span data-ttu-id="7fcfa-130">Ресурс **sitePage** имеет следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-130">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="7fcfa-131">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7fcfa-131">Property name</span></span>    | <span data-ttu-id="7fcfa-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7fcfa-132">Type</span></span>                         | <span data-ttu-id="7fcfa-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7fcfa-133">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="7fcfa-134">contentType</span><span class="sxs-lookup"><span data-stu-id="7fcfa-134">contentType</span></span>      | <span data-ttu-id="7fcfa-135">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="7fcfa-135">[contentTypeInfo][]</span></span>          | <span data-ttu-id="7fcfa-136">Тип страницы содержимого.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-136">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="7fcfa-137">Контент страницы</span><span class="sxs-lookup"><span data-stu-id="7fcfa-137">Page Content</span></span>

<span data-ttu-id="7fcfa-138">Ресурс **sitePage** имеет следующие поля содержимого.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-138">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="7fcfa-139">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7fcfa-139">Property name</span></span>      | <span data-ttu-id="7fcfa-140">Тип</span><span class="sxs-lookup"><span data-stu-id="7fcfa-140">Type</span></span>                       | <span data-ttu-id="7fcfa-141">Описание</span><span class="sxs-lookup"><span data-stu-id="7fcfa-141">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="7fcfa-142">должности.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-142">title</span></span>              | <span data-ttu-id="7fcfa-143">строка</span><span class="sxs-lookup"><span data-stu-id="7fcfa-143">string</span></span>                     | <span data-ttu-id="7fcfa-144">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-144">The title of the page.</span></span>
| <span data-ttu-id="7fcfa-145">pageLayout</span><span class="sxs-lookup"><span data-stu-id="7fcfa-145">pageLayout</span></span>         | <span data-ttu-id="7fcfa-146">string</span><span class="sxs-lookup"><span data-stu-id="7fcfa-146">string</span></span>                     | <span data-ttu-id="7fcfa-147">Имя страницы макета страницы.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-147">The name of the page layout of the page.</span></span>
| <span data-ttu-id="7fcfa-148">веб-части</span><span class="sxs-lookup"><span data-stu-id="7fcfa-148">webParts</span></span>           | <span data-ttu-id="7fcfa-149">[веб-части][]</span><span class="sxs-lookup"><span data-stu-id="7fcfa-149">[webPart][]</span></span>                | <span data-ttu-id="7fcfa-150">Веб-частей на странице.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-150">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="7fcfa-151">Создание метаданных</span><span class="sxs-lookup"><span data-stu-id="7fcfa-151">Authoring Metadata</span></span>

<span data-ttu-id="7fcfa-152">Ресурс **sitePage** имеет следующие метаданные, связанные с разработки.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-152">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="7fcfa-153">Свойство publishingState будет отражают состояние как извлечь или опубликовать разработки страниц.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-153">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="7fcfa-154">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7fcfa-154">Property name</span></span>          | <span data-ttu-id="7fcfa-155">Тип</span><span class="sxs-lookup"><span data-stu-id="7fcfa-155">Type</span></span>                   | <span data-ttu-id="7fcfa-156">Описание</span><span class="sxs-lookup"><span data-stu-id="7fcfa-156">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="7fcfa-157">publishingState</span><span class="sxs-lookup"><span data-stu-id="7fcfa-157">publishingState</span></span>        | <span data-ttu-id="7fcfa-158">[publicationFacet][].</span><span class="sxs-lookup"><span data-stu-id="7fcfa-158">[publicationFacet][]</span></span>   | <span data-ttu-id="7fcfa-159">Состояния публикации и MM.mm версия страницы.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-159">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="7fcfa-160">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="7fcfa-161">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7fcfa-161">Property name</span></span>        | <span data-ttu-id="7fcfa-162">Тип</span><span class="sxs-lookup"><span data-stu-id="7fcfa-162">Type</span></span>              | <span data-ttu-id="7fcfa-163">Описание</span><span class="sxs-lookup"><span data-stu-id="7fcfa-163">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="7fcfa-164">id</span><span class="sxs-lookup"><span data-stu-id="7fcfa-164">id</span></span>                   | <span data-ttu-id="7fcfa-165">строка</span><span class="sxs-lookup"><span data-stu-id="7fcfa-165">string</span></span>            | <span data-ttu-id="7fcfa-p105">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="7fcfa-168">name</span><span class="sxs-lookup"><span data-stu-id="7fcfa-168">name</span></span>                 | <span data-ttu-id="7fcfa-169">строка</span><span class="sxs-lookup"><span data-stu-id="7fcfa-169">string</span></span>            | <span data-ttu-id="7fcfa-170">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-170">The name / title of the item.</span></span>
| <span data-ttu-id="7fcfa-171">createdBy</span><span class="sxs-lookup"><span data-stu-id="7fcfa-171">createdBy</span></span>            | <span data-ttu-id="7fcfa-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7fcfa-172">[identitySet][]</span></span>   | <span data-ttu-id="7fcfa-173">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-173">Identity of the creator of this item.</span></span> <span data-ttu-id="7fcfa-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-174">Read-only.</span></span>
| <span data-ttu-id="7fcfa-175">eTag</span><span class="sxs-lookup"><span data-stu-id="7fcfa-175">eTag</span></span>                 | <span data-ttu-id="7fcfa-176">string</span><span class="sxs-lookup"><span data-stu-id="7fcfa-176">string</span></span>            | <span data-ttu-id="7fcfa-p107">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-p107">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="7fcfa-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7fcfa-179">lastModifiedBy</span></span>       | <span data-ttu-id="7fcfa-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7fcfa-180">[identitySet][]</span></span>   | <span data-ttu-id="7fcfa-181">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="7fcfa-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-182">Read-only.</span></span>
| <span data-ttu-id="7fcfa-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7fcfa-183">lastModifiedDateTime</span></span> | <span data-ttu-id="7fcfa-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fcfa-184">DateTimeOffset</span></span>    | <span data-ttu-id="7fcfa-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="7fcfa-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="7fcfa-187">parentReference</span></span>      | <span data-ttu-id="7fcfa-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="7fcfa-188">[itemReference][]</span></span> | <span data-ttu-id="7fcfa-p110">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-p110">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="7fcfa-191">webUrl</span><span class="sxs-lookup"><span data-stu-id="7fcfa-191">webUrl</span></span>               | <span data-ttu-id="7fcfa-192">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="7fcfa-192">string (url)</span></span>      | <span data-ttu-id="7fcfa-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="7fcfa-195">Связи</span><span class="sxs-lookup"><span data-stu-id="7fcfa-195">Relationships</span></span>

<span data-ttu-id="7fcfa-196">Ресурс **sitePage** не имеет отношения к другим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="7fcfa-196">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[списки]: list.md
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
