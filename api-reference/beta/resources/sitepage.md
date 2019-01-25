---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7b1634e79214f1cece85a78af29db6422ac03a81
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522303"
---
# <a name="sitepage-resource"></a><span data-ttu-id="72d04-102">sitePage ресурсов</span><span class="sxs-lookup"><span data-stu-id="72d04-102">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72d04-103">Этот ресурс представляет страницу SitePages [списка][].</span><span class="sxs-lookup"><span data-stu-id="72d04-103">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="72d04-104">Он содержит заголовок, макет и коллекцию s [веб-части][].</span><span class="sxs-lookup"><span data-stu-id="72d04-104">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="72d04-105">Задачи на странице</span><span class="sxs-lookup"><span data-stu-id="72d04-105">Tasks on a page</span></span>

<span data-ttu-id="72d04-106">Для **sitePage** ресурсов доступны следующие задачи.</span><span class="sxs-lookup"><span data-stu-id="72d04-106">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="72d04-107">Все приведенные ниже примеры относятся к сайту, например [][].</span><span class="sxs-lookup"><span data-stu-id="72d04-107">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="72d04-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="72d04-108">Common task</span></span>                     | <span data-ttu-id="72d04-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="72d04-109">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="72d04-110">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="72d04-110">[List pages][]</span></span>                  | <span data-ttu-id="72d04-111">Запрос GET для страниц</span><span class="sxs-lookup"><span data-stu-id="72d04-111">GET /pages</span></span>
| <span data-ttu-id="72d04-112">[Получение страницы][]</span><span class="sxs-lookup"><span data-stu-id="72d04-112">[Get page][]</span></span>                    | <span data-ttu-id="72d04-113">Получение /pages/ {идентификатор страницы}</span><span class="sxs-lookup"><span data-stu-id="72d04-113">GET /pages/{page-id}</span></span>
| <span data-ttu-id="72d04-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="72d04-114">[Create][]</span></span>                      | <span data-ttu-id="72d04-115">POST pages</span><span class="sxs-lookup"><span data-stu-id="72d04-115">POST /pages</span></span>
| <span data-ttu-id="72d04-116">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="72d04-116">[Delete][]</span></span>                      | <span data-ttu-id="72d04-117">Удаление /pages/ {идентификатор страницы}</span><span class="sxs-lookup"><span data-stu-id="72d04-117">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="72d04-118">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="72d04-118">[Publish][]</span></span>                     | <span data-ttu-id="72d04-119">Учет /pages/ {идентификатор страницы} аудио- и публикация</span><span class="sxs-lookup"><span data-stu-id="72d04-119">POST /pages/{page-id}/publish</span></span>

[Перечисление страниц]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Получение страницы]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="72d04-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72d04-125">JSON representation</span></span>

<span data-ttu-id="72d04-126">Ниже представлена JSON **sitePage** ресурса.</span><span class="sxs-lookup"><span data-stu-id="72d04-126">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="72d04-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="72d04-127">Properties</span></span>

<span data-ttu-id="72d04-128">Ресурс **sitePage** имеет следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="72d04-128">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="72d04-129">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="72d04-129">Property name</span></span>    | <span data-ttu-id="72d04-130">Тип</span><span class="sxs-lookup"><span data-stu-id="72d04-130">Type</span></span>                         | <span data-ttu-id="72d04-131">Описание</span><span class="sxs-lookup"><span data-stu-id="72d04-131">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="72d04-132">contentType</span><span class="sxs-lookup"><span data-stu-id="72d04-132">contentType</span></span>      | <span data-ttu-id="72d04-133">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="72d04-133">[contentTypeInfo][]</span></span>          | <span data-ttu-id="72d04-134">Тип страницы содержимого.</span><span class="sxs-lookup"><span data-stu-id="72d04-134">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="72d04-135">Содержимое страницы</span><span class="sxs-lookup"><span data-stu-id="72d04-135">Page Content</span></span>

<span data-ttu-id="72d04-136">Ресурс **sitePage** имеет следующие поля содержимого.</span><span class="sxs-lookup"><span data-stu-id="72d04-136">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="72d04-137">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="72d04-137">Property name</span></span>      | <span data-ttu-id="72d04-138">Тип</span><span class="sxs-lookup"><span data-stu-id="72d04-138">Type</span></span>                       | <span data-ttu-id="72d04-139">Описание</span><span class="sxs-lookup"><span data-stu-id="72d04-139">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="72d04-140">должности.</span><span class="sxs-lookup"><span data-stu-id="72d04-140">title</span></span>              | <span data-ttu-id="72d04-141">строка</span><span class="sxs-lookup"><span data-stu-id="72d04-141">string</span></span>                     | <span data-ttu-id="72d04-142">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="72d04-142">The title of the page.</span></span>
| <span data-ttu-id="72d04-143">pageLayout</span><span class="sxs-lookup"><span data-stu-id="72d04-143">pageLayout</span></span>         | <span data-ttu-id="72d04-144">string</span><span class="sxs-lookup"><span data-stu-id="72d04-144">string</span></span>                     | <span data-ttu-id="72d04-145">Имя страницы макета страницы.</span><span class="sxs-lookup"><span data-stu-id="72d04-145">The name of the page layout of the page.</span></span>
| <span data-ttu-id="72d04-146">веб-части</span><span class="sxs-lookup"><span data-stu-id="72d04-146">webParts</span></span>           | <span data-ttu-id="72d04-147">веб-часть</span><span class="sxs-lookup"><span data-stu-id="72d04-147">[webPart][]</span></span>                | <span data-ttu-id="72d04-148">Веб-частей на странице.</span><span class="sxs-lookup"><span data-stu-id="72d04-148">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="72d04-149">Создание метаданных</span><span class="sxs-lookup"><span data-stu-id="72d04-149">Authoring Metadata</span></span>

<span data-ttu-id="72d04-150">Ресурс **sitePage** имеет следующие метаданные, связанные с разработки.</span><span class="sxs-lookup"><span data-stu-id="72d04-150">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="72d04-151">Свойство publishingState будет отражают состояние как извлечь или опубликовать разработки страниц.</span><span class="sxs-lookup"><span data-stu-id="72d04-151">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="72d04-152">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="72d04-152">Property name</span></span>          | <span data-ttu-id="72d04-153">Тип</span><span class="sxs-lookup"><span data-stu-id="72d04-153">Type</span></span>                   | <span data-ttu-id="72d04-154">Описание</span><span class="sxs-lookup"><span data-stu-id="72d04-154">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="72d04-155">publishingState</span><span class="sxs-lookup"><span data-stu-id="72d04-155">publishingState</span></span>        | <span data-ttu-id="72d04-156">[publicationFacet][].</span><span class="sxs-lookup"><span data-stu-id="72d04-156">[publicationFacet][]</span></span>   | <span data-ttu-id="72d04-157">Состояния публикации и MM.mm версия страницы.</span><span class="sxs-lookup"><span data-stu-id="72d04-157">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="72d04-158">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="72d04-158">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="72d04-159">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="72d04-159">Property name</span></span>        | <span data-ttu-id="72d04-160">Тип</span><span class="sxs-lookup"><span data-stu-id="72d04-160">Type</span></span>              | <span data-ttu-id="72d04-161">Описание</span><span class="sxs-lookup"><span data-stu-id="72d04-161">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="72d04-162">id</span><span class="sxs-lookup"><span data-stu-id="72d04-162">id</span></span>                   | <span data-ttu-id="72d04-163">string</span><span class="sxs-lookup"><span data-stu-id="72d04-163">string</span></span>            | <span data-ttu-id="72d04-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d04-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="72d04-166">name</span><span class="sxs-lookup"><span data-stu-id="72d04-166">name</span></span>                 | <span data-ttu-id="72d04-167">string</span><span class="sxs-lookup"><span data-stu-id="72d04-167">string</span></span>            | <span data-ttu-id="72d04-168">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="72d04-168">The name / title of the item.</span></span>
| <span data-ttu-id="72d04-169">createdBy</span><span class="sxs-lookup"><span data-stu-id="72d04-169">createdBy</span></span>            | <span data-ttu-id="72d04-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="72d04-170">[identitySet][]</span></span>   | <span data-ttu-id="72d04-171">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="72d04-171">Identity of the creator of this item.</span></span> <span data-ttu-id="72d04-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d04-172">Read-only.</span></span>
| <span data-ttu-id="72d04-173">eTag</span><span class="sxs-lookup"><span data-stu-id="72d04-173">eTag</span></span>                 | <span data-ttu-id="72d04-174">string</span><span class="sxs-lookup"><span data-stu-id="72d04-174">string</span></span>            | <span data-ttu-id="72d04-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d04-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="72d04-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="72d04-177">lastModifiedBy</span></span>       | <span data-ttu-id="72d04-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="72d04-178">[identitySet][]</span></span>   | <span data-ttu-id="72d04-179">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="72d04-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="72d04-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d04-180">Read-only.</span></span>
| <span data-ttu-id="72d04-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72d04-181">lastModifiedDateTime</span></span> | <span data-ttu-id="72d04-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72d04-182">DateTimeOffset</span></span>    | <span data-ttu-id="72d04-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d04-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="72d04-185">parentReference</span><span class="sxs-lookup"><span data-stu-id="72d04-185">parentReference</span></span>      | <span data-ttu-id="72d04-186">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="72d04-186">[itemReference][]</span></span> | <span data-ttu-id="72d04-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d04-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="72d04-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="72d04-189">webUrl</span></span>               | <span data-ttu-id="72d04-190">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="72d04-190">string (url)</span></span>      | <span data-ttu-id="72d04-p110">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d04-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="72d04-193">Связи</span><span class="sxs-lookup"><span data-stu-id="72d04-193">Relationships</span></span>

<span data-ttu-id="72d04-194">Ресурс **sitePage** не имеет отношения к другим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="72d04-194">The **sitePage** resource does not have relationships to other resources.</span></span>

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
<span data-ttu-id="72d04-202">веб-часть</span><span class="sxs-lookup"><span data-stu-id="72d04-202">[webPart]: webpart.md</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/sitepage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
