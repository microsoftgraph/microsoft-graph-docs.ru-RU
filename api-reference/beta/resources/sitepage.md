---
author: rahmit
description: Этот ресурс представляет страницу в списке SitePages.
ms.date: 03/15/2018
title: ситепаже
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: d92a78ff73854d465ba8363b7bddff66be6bffc4
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953618"
---
# <a name="sitepage-resource"></a><span data-ttu-id="baf10-103">ресурс Ситепаже</span><span class="sxs-lookup"><span data-stu-id="baf10-103">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baf10-104">Этот ресурс представляет страницу в [списке][]SitePages.</span><span class="sxs-lookup"><span data-stu-id="baf10-104">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="baf10-105">Он содержит заголовок, макет и коллекцию [веб-частей][]s.</span><span class="sxs-lookup"><span data-stu-id="baf10-105">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="baf10-106">Задачи на странице</span><span class="sxs-lookup"><span data-stu-id="baf10-106">Tasks on a page</span></span>

<span data-ttu-id="baf10-107">Для ресурсов **ситепаже** доступны следующие задачи.</span><span class="sxs-lookup"><span data-stu-id="baf10-107">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="baf10-108">Все приведенные ниже примеры относятся к [сайту][], например: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="baf10-108">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="baf10-109">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="baf10-109">Common task</span></span>                     | <span data-ttu-id="baf10-110">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="baf10-110">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="baf10-111">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="baf10-111">[List pages][]</span></span>                  | <span data-ttu-id="baf10-112">ПОЛУЧЕНИЕ/Pages</span><span class="sxs-lookup"><span data-stu-id="baf10-112">GET /pages</span></span>
| <span data-ttu-id="baf10-113">[Вывод страницы][]</span><span class="sxs-lookup"><span data-stu-id="baf10-113">[Get page][]</span></span>                    | <span data-ttu-id="baf10-114">ПОЛУЧЕНИЕ/Пажес/{Паже-ИД}</span><span class="sxs-lookup"><span data-stu-id="baf10-114">GET /pages/{page-id}</span></span>
| <span data-ttu-id="baf10-115">[создание][];</span><span class="sxs-lookup"><span data-stu-id="baf10-115">[Create][]</span></span>                      | <span data-ttu-id="baf10-116">POST/Pages</span><span class="sxs-lookup"><span data-stu-id="baf10-116">POST /pages</span></span>
| <span data-ttu-id="baf10-117">[удаление][];</span><span class="sxs-lookup"><span data-stu-id="baf10-117">[Delete][]</span></span>                      | <span data-ttu-id="baf10-118">Удаление/Пажес/{Паже-ИД}</span><span class="sxs-lookup"><span data-stu-id="baf10-118">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="baf10-119">[публикация][];</span><span class="sxs-lookup"><span data-stu-id="baf10-119">[Publish][]</span></span>                     | <span data-ttu-id="baf10-120">POST/Пажес/{Паже-ИД}/публиш</span><span class="sxs-lookup"><span data-stu-id="baf10-120">POST /pages/{page-id}/publish</span></span>

[Перечисление страниц]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Вывод страницы]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Создание]: ../api/sitepage-create.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[публикация]: ../api/sitepage-publish.md;
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="baf10-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="baf10-126">JSON representation</span></span>

<span data-ttu-id="baf10-127">Ниже показано представление ресурса **ситепаже** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="baf10-127">Here is a JSON representation of a **sitePage** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage",
  "openType": true
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayoutType": "String",
  "webParts": [{ "@odata.type": "microsoft.graph.webPart" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

   /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="baf10-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="baf10-128">Properties</span></span>

<span data-ttu-id="baf10-129">Ресурс **ситепаже** имеет следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="baf10-129">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="baf10-130">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="baf10-130">Property name</span></span>    | <span data-ttu-id="baf10-131">Тип</span><span class="sxs-lookup"><span data-stu-id="baf10-131">Type</span></span>                         | <span data-ttu-id="baf10-132">Описание</span><span class="sxs-lookup"><span data-stu-id="baf10-132">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="baf10-133">contentType</span><span class="sxs-lookup"><span data-stu-id="baf10-133">contentType</span></span>      | <span data-ttu-id="baf10-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="baf10-134">[contentTypeInfo][]</span></span>          | <span data-ttu-id="baf10-135">Тип контента страницы.</span><span class="sxs-lookup"><span data-stu-id="baf10-135">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="baf10-136">Контент страницы</span><span class="sxs-lookup"><span data-stu-id="baf10-136">Page Content</span></span>

<span data-ttu-id="baf10-137">Ресурс **ситепаже** имеет следующие поля контента.</span><span class="sxs-lookup"><span data-stu-id="baf10-137">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="baf10-138">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="baf10-138">Property name</span></span>      | <span data-ttu-id="baf10-139">Тип</span><span class="sxs-lookup"><span data-stu-id="baf10-139">Type</span></span>                       | <span data-ttu-id="baf10-140">Описание</span><span class="sxs-lookup"><span data-stu-id="baf10-140">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="baf10-141">title</span><span class="sxs-lookup"><span data-stu-id="baf10-141">title</span></span>              | <span data-ttu-id="baf10-142">string</span><span class="sxs-lookup"><span data-stu-id="baf10-142">string</span></span>                     | <span data-ttu-id="baf10-143">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="baf10-143">The title of the page.</span></span>
| <span data-ttu-id="baf10-144">pageLayout</span><span class="sxs-lookup"><span data-stu-id="baf10-144">pageLayout</span></span>         | <span data-ttu-id="baf10-145">string</span><span class="sxs-lookup"><span data-stu-id="baf10-145">string</span></span>                     | <span data-ttu-id="baf10-146">Имя макета страницы.</span><span class="sxs-lookup"><span data-stu-id="baf10-146">The name of the page layout of the page.</span></span>
| <span data-ttu-id="baf10-147">webParts</span><span class="sxs-lookup"><span data-stu-id="baf10-147">webParts</span></span>           | <span data-ttu-id="baf10-148">[Частей][]</span><span class="sxs-lookup"><span data-stu-id="baf10-148">[webPart][]</span></span>                | <span data-ttu-id="baf10-149">Веб-части на странице.</span><span class="sxs-lookup"><span data-stu-id="baf10-149">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="baf10-150">Метаданные для разработки</span><span class="sxs-lookup"><span data-stu-id="baf10-150">Authoring Metadata</span></span>

<span data-ttu-id="baf10-151">Ресурс **ситепаже** содержит следующие метаданные, связанные с созданием и отправкой.</span><span class="sxs-lookup"><span data-stu-id="baf10-151">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="baf10-152">Свойство Публишингстате будет отражать состояние создания страницы, например извлеченный или опубликованный.</span><span class="sxs-lookup"><span data-stu-id="baf10-152">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="baf10-153">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="baf10-153">Property name</span></span>          | <span data-ttu-id="baf10-154">Тип</span><span class="sxs-lookup"><span data-stu-id="baf10-154">Type</span></span>                   | <span data-ttu-id="baf10-155">Описание</span><span class="sxs-lookup"><span data-stu-id="baf10-155">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="baf10-156">publishingState</span><span class="sxs-lookup"><span data-stu-id="baf10-156">publishingState</span></span>        | <span data-ttu-id="baf10-157">[publicationFacet][].</span><span class="sxs-lookup"><span data-stu-id="baf10-157">[publicationFacet][]</span></span>   | <span data-ttu-id="baf10-158">Состояние публикации и версия MM.mm страницы.</span><span class="sxs-lookup"><span data-stu-id="baf10-158">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="baf10-159">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="baf10-159">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="baf10-160">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="baf10-160">Property name</span></span>        | <span data-ttu-id="baf10-161">Тип</span><span class="sxs-lookup"><span data-stu-id="baf10-161">Type</span></span>              | <span data-ttu-id="baf10-162">Описание</span><span class="sxs-lookup"><span data-stu-id="baf10-162">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="baf10-163">id</span><span class="sxs-lookup"><span data-stu-id="baf10-163">id</span></span>                   | <span data-ttu-id="baf10-164">строка</span><span class="sxs-lookup"><span data-stu-id="baf10-164">string</span></span>            | <span data-ttu-id="baf10-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="baf10-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="baf10-167">name</span><span class="sxs-lookup"><span data-stu-id="baf10-167">name</span></span>                 | <span data-ttu-id="baf10-168">string</span><span class="sxs-lookup"><span data-stu-id="baf10-168">string</span></span>            | <span data-ttu-id="baf10-169">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="baf10-169">The name / title of the item.</span></span>
| <span data-ttu-id="baf10-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="baf10-170">createdBy</span></span>            | <span data-ttu-id="baf10-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="baf10-171">[identitySet][]</span></span>   | <span data-ttu-id="baf10-172">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="baf10-172">Identity of the creator of this item.</span></span> <span data-ttu-id="baf10-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="baf10-173">Read-only.</span></span>
| <span data-ttu-id="baf10-174">eTag</span><span class="sxs-lookup"><span data-stu-id="baf10-174">eTag</span></span>                 | <span data-ttu-id="baf10-175">string</span><span class="sxs-lookup"><span data-stu-id="baf10-175">string</span></span>            | <span data-ttu-id="baf10-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="baf10-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="baf10-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="baf10-178">lastModifiedBy</span></span>       | <span data-ttu-id="baf10-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="baf10-179">[identitySet][]</span></span>   | <span data-ttu-id="baf10-180">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="baf10-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="baf10-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="baf10-181">Read-only.</span></span>
| <span data-ttu-id="baf10-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="baf10-182">lastModifiedDateTime</span></span> | <span data-ttu-id="baf10-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baf10-183">DateTimeOffset</span></span>    | <span data-ttu-id="baf10-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="baf10-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="baf10-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="baf10-186">parentReference</span></span>      | <span data-ttu-id="baf10-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="baf10-187">[itemReference][]</span></span> | <span data-ttu-id="baf10-188">Сведения о родительском элементе, если элемент выступает в роли родительского элемента.</span><span class="sxs-lookup"><span data-stu-id="baf10-188">Parent information, if the item has a parent.</span></span> <span data-ttu-id="baf10-189">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="baf10-189">Read-only.</span></span>
| <span data-ttu-id="baf10-190">webUrl</span><span class="sxs-lookup"><span data-stu-id="baf10-190">webUrl</span></span>               | <span data-ttu-id="baf10-191">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="baf10-191">string (url)</span></span>      | <span data-ttu-id="baf10-p110">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="baf10-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="baf10-194">Связи</span><span class="sxs-lookup"><span data-stu-id="baf10-194">Relationships</span></span>

<span data-ttu-id="baf10-195">У ресурса **ситепаже** нет отношений с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="baf10-195">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md.
[сайта]: site.md
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
  "suppressions": []
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
