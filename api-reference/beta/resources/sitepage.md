---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a756929212dbca04f16e9e4701e34bbd8d4de28f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939240"
---
# <a name="sitepage-resource"></a><span data-ttu-id="dcc35-102">sitePage ресурсов</span><span class="sxs-lookup"><span data-stu-id="dcc35-102">sitePage resource</span></span>

> <span data-ttu-id="dcc35-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dcc35-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dcc35-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcc35-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dcc35-105">Этот ресурс представляет страницу SitePages [списка][].</span><span class="sxs-lookup"><span data-stu-id="dcc35-105">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="dcc35-106">Он содержит заголовок, макет и коллекцию s [веб-части][].</span><span class="sxs-lookup"><span data-stu-id="dcc35-106">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="dcc35-107">Задачи на странице</span><span class="sxs-lookup"><span data-stu-id="dcc35-107">Tasks on a page</span></span>

<span data-ttu-id="dcc35-108">Для **sitePage** ресурсов доступны следующие задачи.</span><span class="sxs-lookup"><span data-stu-id="dcc35-108">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="dcc35-109">Всех приведенных ниже примерах относительны [сайта][], например: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="dcc35-109">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="dcc35-110">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="dcc35-110">Common task</span></span>                     | <span data-ttu-id="dcc35-111">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="dcc35-111">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="dcc35-112">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="dcc35-112">[List pages][]</span></span>                  | <span data-ttu-id="dcc35-113">Получение /pages</span><span class="sxs-lookup"><span data-stu-id="dcc35-113">GET /pages</span></span>
| <span data-ttu-id="dcc35-114">[Получение страницы][]</span><span class="sxs-lookup"><span data-stu-id="dcc35-114">[Get page][]</span></span>                    | <span data-ttu-id="dcc35-115">Получение /pages/ {идентификатор страницы}</span><span class="sxs-lookup"><span data-stu-id="dcc35-115">GET /pages/{page-id}</span></span>
| <span data-ttu-id="dcc35-116">[создание][];</span><span class="sxs-lookup"><span data-stu-id="dcc35-116">[Create][]</span></span>                      | <span data-ttu-id="dcc35-117">POST /pages</span><span class="sxs-lookup"><span data-stu-id="dcc35-117">POST /pages</span></span>
| <span data-ttu-id="dcc35-118">[удаление][];</span><span class="sxs-lookup"><span data-stu-id="dcc35-118">[Delete][]</span></span>                      | <span data-ttu-id="dcc35-119">Удаление /pages/ {идентификатор страницы}</span><span class="sxs-lookup"><span data-stu-id="dcc35-119">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="dcc35-120">[публикация][];</span><span class="sxs-lookup"><span data-stu-id="dcc35-120">[Publish][]</span></span>                     | <span data-ttu-id="dcc35-121">Учет /pages/ {идентификатор страницы} аудио- и публикация</span><span class="sxs-lookup"><span data-stu-id="dcc35-121">POST /pages/{page-id}/publish</span></span>

[Перечисление страниц]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Получение страницы]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Создание]: ../api/sitepage-create.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[публикация]: ../api/sitepage-publish.md;
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="dcc35-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dcc35-127">JSON representation</span></span>

<span data-ttu-id="dcc35-128">Ниже представлена JSON **sitePage** ресурса.</span><span class="sxs-lookup"><span data-stu-id="dcc35-128">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dcc35-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="dcc35-129">Properties</span></span>

<span data-ttu-id="dcc35-130">Ресурс **sitePage** имеет следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="dcc35-130">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="dcc35-131">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dcc35-131">Property name</span></span>    | <span data-ttu-id="dcc35-132">Тип</span><span class="sxs-lookup"><span data-stu-id="dcc35-132">Type</span></span>                         | <span data-ttu-id="dcc35-133">Описание</span><span class="sxs-lookup"><span data-stu-id="dcc35-133">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="dcc35-134">contentType</span><span class="sxs-lookup"><span data-stu-id="dcc35-134">contentType</span></span>      | <span data-ttu-id="dcc35-135">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="dcc35-135">[contentTypeInfo][]</span></span>          | <span data-ttu-id="dcc35-136">Тип страницы содержимого.</span><span class="sxs-lookup"><span data-stu-id="dcc35-136">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="dcc35-137">Контент страницы</span><span class="sxs-lookup"><span data-stu-id="dcc35-137">Page Content</span></span>

<span data-ttu-id="dcc35-138">Ресурс **sitePage** имеет следующие поля содержимого.</span><span class="sxs-lookup"><span data-stu-id="dcc35-138">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="dcc35-139">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dcc35-139">Property name</span></span>      | <span data-ttu-id="dcc35-140">Тип</span><span class="sxs-lookup"><span data-stu-id="dcc35-140">Type</span></span>                       | <span data-ttu-id="dcc35-141">Описание</span><span class="sxs-lookup"><span data-stu-id="dcc35-141">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="dcc35-142">должности.</span><span class="sxs-lookup"><span data-stu-id="dcc35-142">title</span></span>              | <span data-ttu-id="dcc35-143">строка</span><span class="sxs-lookup"><span data-stu-id="dcc35-143">string</span></span>                     | <span data-ttu-id="dcc35-144">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="dcc35-144">The title of the page.</span></span>
| <span data-ttu-id="dcc35-145">pageLayout</span><span class="sxs-lookup"><span data-stu-id="dcc35-145">pageLayout</span></span>         | <span data-ttu-id="dcc35-146">строка</span><span class="sxs-lookup"><span data-stu-id="dcc35-146">string</span></span>                     | <span data-ttu-id="dcc35-147">Имя страницы макета страницы.</span><span class="sxs-lookup"><span data-stu-id="dcc35-147">The name of the page layout of the page.</span></span>
| <span data-ttu-id="dcc35-148">веб-части</span><span class="sxs-lookup"><span data-stu-id="dcc35-148">webParts</span></span>           | <span data-ttu-id="dcc35-149">[веб-части][]</span><span class="sxs-lookup"><span data-stu-id="dcc35-149">[webPart][]</span></span>                | <span data-ttu-id="dcc35-150">Веб-частей на странице.</span><span class="sxs-lookup"><span data-stu-id="dcc35-150">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="dcc35-151">Создание метаданных</span><span class="sxs-lookup"><span data-stu-id="dcc35-151">Authoring Metadata</span></span>

<span data-ttu-id="dcc35-152">Ресурс **sitePage** имеет следующие метаданные, связанные с разработки.</span><span class="sxs-lookup"><span data-stu-id="dcc35-152">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="dcc35-153">Свойство publishingState будет отражают состояние как извлечь или опубликовать разработки страниц.</span><span class="sxs-lookup"><span data-stu-id="dcc35-153">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="dcc35-154">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dcc35-154">Property name</span></span>          | <span data-ttu-id="dcc35-155">Тип</span><span class="sxs-lookup"><span data-stu-id="dcc35-155">Type</span></span>                   | <span data-ttu-id="dcc35-156">Описание</span><span class="sxs-lookup"><span data-stu-id="dcc35-156">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="dcc35-157">publishingState</span><span class="sxs-lookup"><span data-stu-id="dcc35-157">publishingState</span></span>        | <span data-ttu-id="dcc35-158">[publicationFacet][].</span><span class="sxs-lookup"><span data-stu-id="dcc35-158">[publicationFacet][]</span></span>   | <span data-ttu-id="dcc35-159">Состояния публикации и MM.mm версия страницы.</span><span class="sxs-lookup"><span data-stu-id="dcc35-159">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="dcc35-160">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="dcc35-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="dcc35-161">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dcc35-161">Property name</span></span>        | <span data-ttu-id="dcc35-162">Тип</span><span class="sxs-lookup"><span data-stu-id="dcc35-162">Type</span></span>              | <span data-ttu-id="dcc35-163">Описание</span><span class="sxs-lookup"><span data-stu-id="dcc35-163">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="dcc35-164">id</span><span class="sxs-lookup"><span data-stu-id="dcc35-164">id</span></span>                   | <span data-ttu-id="dcc35-165">строка</span><span class="sxs-lookup"><span data-stu-id="dcc35-165">string</span></span>            | <span data-ttu-id="dcc35-p105">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcc35-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="dcc35-168">name</span><span class="sxs-lookup"><span data-stu-id="dcc35-168">name</span></span>                 | <span data-ttu-id="dcc35-169">строка</span><span class="sxs-lookup"><span data-stu-id="dcc35-169">string</span></span>            | <span data-ttu-id="dcc35-170">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="dcc35-170">The name / title of the item.</span></span>
| <span data-ttu-id="dcc35-171">createdBy</span><span class="sxs-lookup"><span data-stu-id="dcc35-171">createdBy</span></span>            | <span data-ttu-id="dcc35-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dcc35-172">[identitySet][]</span></span>   | <span data-ttu-id="dcc35-173">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="dcc35-173">Identity of the creator of this item.</span></span> <span data-ttu-id="dcc35-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcc35-174">Read-only.</span></span>
| <span data-ttu-id="dcc35-175">eTag</span><span class="sxs-lookup"><span data-stu-id="dcc35-175">eTag</span></span>                 | <span data-ttu-id="dcc35-176">строка</span><span class="sxs-lookup"><span data-stu-id="dcc35-176">string</span></span>            | <span data-ttu-id="dcc35-p107">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcc35-p107">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="dcc35-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="dcc35-179">lastModifiedBy</span></span>       | <span data-ttu-id="dcc35-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dcc35-180">[identitySet][]</span></span>   | <span data-ttu-id="dcc35-181">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="dcc35-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="dcc35-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcc35-182">Read-only.</span></span>
| <span data-ttu-id="dcc35-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dcc35-183">lastModifiedDateTime</span></span> | <span data-ttu-id="dcc35-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcc35-184">DateTimeOffset</span></span>    | <span data-ttu-id="dcc35-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcc35-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="dcc35-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="dcc35-187">parentReference</span></span>      | <span data-ttu-id="dcc35-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="dcc35-188">[itemReference][]</span></span> | <span data-ttu-id="dcc35-p110">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcc35-p110">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="dcc35-191">webUrl</span><span class="sxs-lookup"><span data-stu-id="dcc35-191">webUrl</span></span>               | <span data-ttu-id="dcc35-192">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="dcc35-192">string (url)</span></span>      | <span data-ttu-id="dcc35-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcc35-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="dcc35-195">Связи</span><span class="sxs-lookup"><span data-stu-id="dcc35-195">Relationships</span></span>

<span data-ttu-id="dcc35-196">Ресурс **sitePage** не имеет отношения к другим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="dcc35-196">The **sitePage** resource does not have relationships to other resources.</span></span>

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
