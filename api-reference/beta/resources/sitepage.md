---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: Ситепаже
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7b1634e79214f1cece85a78af29db6422ac03a81
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583405"
---
# <a name="sitepage-resource"></a><span data-ttu-id="46d61-102">ресурс Ситепаже</span><span class="sxs-lookup"><span data-stu-id="46d61-102">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46d61-103">Этот ресурс представляет страницу в [списке][]SitePages.</span><span class="sxs-lookup"><span data-stu-id="46d61-103">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="46d61-104">Он содержит заголовок, макет и коллекцию [веб-частей][]s.</span><span class="sxs-lookup"><span data-stu-id="46d61-104">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="46d61-105">Задачи на странице</span><span class="sxs-lookup"><span data-stu-id="46d61-105">Tasks on a page</span></span>

<span data-ttu-id="46d61-106">Для ресурсов **ситепаже** доступны следующие задачи.</span><span class="sxs-lookup"><span data-stu-id="46d61-106">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="46d61-107">Все приведенные ниже примеры относятся к [сайту][], например: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="46d61-107">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="46d61-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="46d61-108">Common task</span></span>                     | <span data-ttu-id="46d61-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="46d61-109">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="46d61-110">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="46d61-110">[List pages][]</span></span>                  | <span data-ttu-id="46d61-111">ПОЛУЧЕНИЕ/Pages</span><span class="sxs-lookup"><span data-stu-id="46d61-111">GET /pages</span></span>
| <span data-ttu-id="46d61-112">[Вывод страницы][]</span><span class="sxs-lookup"><span data-stu-id="46d61-112">[Get page][]</span></span>                    | <span data-ttu-id="46d61-113">ПОЛУЧЕНИЕ/Пажес/{Паже-ИД}</span><span class="sxs-lookup"><span data-stu-id="46d61-113">GET /pages/{page-id}</span></span>
| <span data-ttu-id="46d61-114">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="46d61-114">[Create][]</span></span>                      | <span data-ttu-id="46d61-115">POST/Pages</span><span class="sxs-lookup"><span data-stu-id="46d61-115">POST /pages</span></span>
| <span data-ttu-id="46d61-116">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="46d61-116">[Delete][]</span></span>                      | <span data-ttu-id="46d61-117">Удаление/Пажес/{Паже-ИД}</span><span class="sxs-lookup"><span data-stu-id="46d61-117">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="46d61-118">[публикация][];</span><span class="sxs-lookup"><span data-stu-id="46d61-118">[Publish][]</span></span>                     | <span data-ttu-id="46d61-119">POST/Пажес/{Паже-ИД}/публиш</span><span class="sxs-lookup"><span data-stu-id="46d61-119">POST /pages/{page-id}/publish</span></span>

[Перечисление страниц]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Вывод страницы]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Создание]: ../api/sitepage-create.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[публикация]: ../api/sitepage-publish.md;
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="46d61-125">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="46d61-125">JSON representation</span></span>

<span data-ttu-id="46d61-126">Ниже показано представление ресурса **ситепаже** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46d61-126">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="46d61-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="46d61-127">Properties</span></span>

<span data-ttu-id="46d61-128">Ресурс **ситепаже** имеет следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="46d61-128">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="46d61-129">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="46d61-129">Property name</span></span>    | <span data-ttu-id="46d61-130">Тип</span><span class="sxs-lookup"><span data-stu-id="46d61-130">Type</span></span>                         | <span data-ttu-id="46d61-131">Описание</span><span class="sxs-lookup"><span data-stu-id="46d61-131">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="46d61-132">contentType</span><span class="sxs-lookup"><span data-stu-id="46d61-132">contentType</span></span>      | <span data-ttu-id="46d61-133">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="46d61-133">[contentTypeInfo][]</span></span>          | <span data-ttu-id="46d61-134">Тип контента страницы.</span><span class="sxs-lookup"><span data-stu-id="46d61-134">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="46d61-135">Контент страницы</span><span class="sxs-lookup"><span data-stu-id="46d61-135">Page Content</span></span>

<span data-ttu-id="46d61-136">Ресурс **ситепаже** имеет следующие поля контента.</span><span class="sxs-lookup"><span data-stu-id="46d61-136">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="46d61-137">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="46d61-137">Property name</span></span>      | <span data-ttu-id="46d61-138">Тип</span><span class="sxs-lookup"><span data-stu-id="46d61-138">Type</span></span>                       | <span data-ttu-id="46d61-139">Описание</span><span class="sxs-lookup"><span data-stu-id="46d61-139">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="46d61-140">title</span><span class="sxs-lookup"><span data-stu-id="46d61-140">title</span></span>              | <span data-ttu-id="46d61-141">string</span><span class="sxs-lookup"><span data-stu-id="46d61-141">string</span></span>                     | <span data-ttu-id="46d61-142">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="46d61-142">The title of the page.</span></span>
| <span data-ttu-id="46d61-143">pageLayout</span><span class="sxs-lookup"><span data-stu-id="46d61-143">pageLayout</span></span>         | <span data-ttu-id="46d61-144">string</span><span class="sxs-lookup"><span data-stu-id="46d61-144">string</span></span>                     | <span data-ttu-id="46d61-145">Имя макета страницы.</span><span class="sxs-lookup"><span data-stu-id="46d61-145">The name of the page layout of the page.</span></span>
| <span data-ttu-id="46d61-146">webParts</span><span class="sxs-lookup"><span data-stu-id="46d61-146">webParts</span></span>           | <span data-ttu-id="46d61-147">[Частей][]</span><span class="sxs-lookup"><span data-stu-id="46d61-147">[webPart][]</span></span>                | <span data-ttu-id="46d61-148">Веб-части на странице.</span><span class="sxs-lookup"><span data-stu-id="46d61-148">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="46d61-149">Метаданные для разработки</span><span class="sxs-lookup"><span data-stu-id="46d61-149">Authoring Metadata</span></span>

<span data-ttu-id="46d61-150">Ресурс **ситепаже** содержит следующие метаданные, связанные с созданием и отправкой.</span><span class="sxs-lookup"><span data-stu-id="46d61-150">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="46d61-151">Свойство Публишингстате будет отражать состояние создания страницы, например извлеченный или опубликованный.</span><span class="sxs-lookup"><span data-stu-id="46d61-151">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="46d61-152">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="46d61-152">Property name</span></span>          | <span data-ttu-id="46d61-153">Тип</span><span class="sxs-lookup"><span data-stu-id="46d61-153">Type</span></span>                   | <span data-ttu-id="46d61-154">Описание</span><span class="sxs-lookup"><span data-stu-id="46d61-154">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="46d61-155">publishingState</span><span class="sxs-lookup"><span data-stu-id="46d61-155">publishingState</span></span>        | <span data-ttu-id="46d61-156">[publicationFacet][].</span><span class="sxs-lookup"><span data-stu-id="46d61-156">[publicationFacet][]</span></span>   | <span data-ttu-id="46d61-157">Состояние публикации и версия MM.mm страницы.</span><span class="sxs-lookup"><span data-stu-id="46d61-157">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="46d61-158">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="46d61-158">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="46d61-159">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="46d61-159">Property name</span></span>        | <span data-ttu-id="46d61-160">Тип</span><span class="sxs-lookup"><span data-stu-id="46d61-160">Type</span></span>              | <span data-ttu-id="46d61-161">Описание</span><span class="sxs-lookup"><span data-stu-id="46d61-161">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="46d61-162">id</span><span class="sxs-lookup"><span data-stu-id="46d61-162">id</span></span>                   | <span data-ttu-id="46d61-163">строка</span><span class="sxs-lookup"><span data-stu-id="46d61-163">string</span></span>            | <span data-ttu-id="46d61-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46d61-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="46d61-166">name</span><span class="sxs-lookup"><span data-stu-id="46d61-166">name</span></span>                 | <span data-ttu-id="46d61-167">string</span><span class="sxs-lookup"><span data-stu-id="46d61-167">string</span></span>            | <span data-ttu-id="46d61-168">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="46d61-168">The name / title of the item.</span></span>
| <span data-ttu-id="46d61-169">createdBy</span><span class="sxs-lookup"><span data-stu-id="46d61-169">createdBy</span></span>            | <span data-ttu-id="46d61-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="46d61-170">[identitySet][]</span></span>   | <span data-ttu-id="46d61-171">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="46d61-171">Identity of the creator of this item.</span></span> <span data-ttu-id="46d61-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46d61-172">Read-only.</span></span>
| <span data-ttu-id="46d61-173">eTag</span><span class="sxs-lookup"><span data-stu-id="46d61-173">eTag</span></span>                 | <span data-ttu-id="46d61-174">string</span><span class="sxs-lookup"><span data-stu-id="46d61-174">string</span></span>            | <span data-ttu-id="46d61-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46d61-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="46d61-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="46d61-177">lastModifiedBy</span></span>       | <span data-ttu-id="46d61-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="46d61-178">[identitySet][]</span></span>   | <span data-ttu-id="46d61-179">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="46d61-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="46d61-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46d61-180">Read-only.</span></span>
| <span data-ttu-id="46d61-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46d61-181">lastModifiedDateTime</span></span> | <span data-ttu-id="46d61-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46d61-182">DateTimeOffset</span></span>    | <span data-ttu-id="46d61-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46d61-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="46d61-185">parentReference</span><span class="sxs-lookup"><span data-stu-id="46d61-185">parentReference</span></span>      | <span data-ttu-id="46d61-186">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="46d61-186">[itemReference][]</span></span> | <span data-ttu-id="46d61-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46d61-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="46d61-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="46d61-189">webUrl</span></span>               | <span data-ttu-id="46d61-190">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="46d61-190">string (url)</span></span>      | <span data-ttu-id="46d61-p110">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46d61-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="46d61-193">Связи</span><span class="sxs-lookup"><span data-stu-id="46d61-193">Relationships</span></span>

<span data-ttu-id="46d61-194">У ресурса **ситепаже** нет отношений с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="46d61-194">The **sitePage** resource does not have relationships to other resources.</span></span>

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
[Частей]: webpart.md
[webPart]: webpart.md

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
