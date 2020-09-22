---
author: rahmit
description: Этот ресурс представляет страницу в списке SitePages.
ms.date: 03/15/2018
title: ситепаже
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: bdb7c0c89938eb3419607839aa1973812788063c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997699"
---
# <a name="sitepage-resource"></a><span data-ttu-id="dcb68-103">ресурс Ситепаже</span><span class="sxs-lookup"><span data-stu-id="dcb68-103">sitePage resource</span></span>

<span data-ttu-id="dcb68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcb68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcb68-105">Этот ресурс представляет страницу в [списке][]SitePages.</span><span class="sxs-lookup"><span data-stu-id="dcb68-105">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="dcb68-106">Он содержит заголовок, макет и коллекцию [веб-частей][]s.</span><span class="sxs-lookup"><span data-stu-id="dcb68-106">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="dcb68-107">Задачи на странице</span><span class="sxs-lookup"><span data-stu-id="dcb68-107">Tasks on a page</span></span>

<span data-ttu-id="dcb68-108">Для ресурсов **ситепаже** доступны следующие задачи.</span><span class="sxs-lookup"><span data-stu-id="dcb68-108">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="dcb68-109">Все приведенные ниже примеры относятся к [сайту][], например: `https://graph.microsoft.com/{api-version}/sites/{site-id}` .</span><span class="sxs-lookup"><span data-stu-id="dcb68-109">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="dcb68-110">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="dcb68-110">Common task</span></span>                     | <span data-ttu-id="dcb68-111">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="dcb68-111">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="dcb68-112">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="dcb68-112">[List pages][]</span></span>                  | <span data-ttu-id="dcb68-113">ПОЛУЧЕНИЕ/Pages</span><span class="sxs-lookup"><span data-stu-id="dcb68-113">GET /pages</span></span>
| <span data-ttu-id="dcb68-114">[Вывод страницы][]</span><span class="sxs-lookup"><span data-stu-id="dcb68-114">[Get page][]</span></span>                    | <span data-ttu-id="dcb68-115">ПОЛУЧЕНИЕ/Пажес/{Паже-ИД}</span><span class="sxs-lookup"><span data-stu-id="dcb68-115">GET /pages/{page-id}</span></span>
| <span data-ttu-id="dcb68-116">[создание][];</span><span class="sxs-lookup"><span data-stu-id="dcb68-116">[Create][]</span></span>                      | <span data-ttu-id="dcb68-117">POST/Pages</span><span class="sxs-lookup"><span data-stu-id="dcb68-117">POST /pages</span></span>
| <span data-ttu-id="dcb68-118">[удаление][];</span><span class="sxs-lookup"><span data-stu-id="dcb68-118">[Delete][]</span></span>                      | <span data-ttu-id="dcb68-119">Удаление/Пажес/{Паже-ИД}</span><span class="sxs-lookup"><span data-stu-id="dcb68-119">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="dcb68-120">[публикация][];</span><span class="sxs-lookup"><span data-stu-id="dcb68-120">[Publish][]</span></span>                     | <span data-ttu-id="dcb68-121">POST/Пажес/{Паже-ИД}/публиш</span><span class="sxs-lookup"><span data-stu-id="dcb68-121">POST /pages/{page-id}/publish</span></span>

[Перечисление страниц]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Вывод страницы]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Создание]: ../api/sitepage-create.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[публикация]: ../api/sitepage-publish.md;
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="dcb68-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dcb68-127">JSON representation</span></span>

<span data-ttu-id="dcb68-128">Ниже показано представление ресурса **ситепаже** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcb68-128">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dcb68-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="dcb68-129">Properties</span></span>

<span data-ttu-id="dcb68-130">Ресурс **ситепаже** имеет следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="dcb68-130">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="dcb68-131">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dcb68-131">Property name</span></span>    | <span data-ttu-id="dcb68-132">Тип</span><span class="sxs-lookup"><span data-stu-id="dcb68-132">Type</span></span>                         | <span data-ttu-id="dcb68-133">Описание</span><span class="sxs-lookup"><span data-stu-id="dcb68-133">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="dcb68-134">contentType</span><span class="sxs-lookup"><span data-stu-id="dcb68-134">contentType</span></span>      | <span data-ttu-id="dcb68-135">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="dcb68-135">[contentTypeInfo][]</span></span>          | <span data-ttu-id="dcb68-136">Тип контента страницы.</span><span class="sxs-lookup"><span data-stu-id="dcb68-136">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="dcb68-137">Контент страницы</span><span class="sxs-lookup"><span data-stu-id="dcb68-137">Page Content</span></span>

<span data-ttu-id="dcb68-138">Ресурс **ситепаже** имеет следующие поля контента.</span><span class="sxs-lookup"><span data-stu-id="dcb68-138">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="dcb68-139">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dcb68-139">Property name</span></span>      | <span data-ttu-id="dcb68-140">Тип</span><span class="sxs-lookup"><span data-stu-id="dcb68-140">Type</span></span>                       | <span data-ttu-id="dcb68-141">Описание</span><span class="sxs-lookup"><span data-stu-id="dcb68-141">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="dcb68-142">title</span><span class="sxs-lookup"><span data-stu-id="dcb68-142">title</span></span>              | <span data-ttu-id="dcb68-143">string</span><span class="sxs-lookup"><span data-stu-id="dcb68-143">string</span></span>                     | <span data-ttu-id="dcb68-144">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="dcb68-144">The title of the page.</span></span>
| <span data-ttu-id="dcb68-145">pageLayout</span><span class="sxs-lookup"><span data-stu-id="dcb68-145">pageLayout</span></span>         | <span data-ttu-id="dcb68-146">string</span><span class="sxs-lookup"><span data-stu-id="dcb68-146">string</span></span>                     | <span data-ttu-id="dcb68-147">Имя макета страницы.</span><span class="sxs-lookup"><span data-stu-id="dcb68-147">The name of the page layout of the page.</span></span>
| <span data-ttu-id="dcb68-148">webParts</span><span class="sxs-lookup"><span data-stu-id="dcb68-148">webParts</span></span>           | <span data-ttu-id="dcb68-149">[Частей][]</span><span class="sxs-lookup"><span data-stu-id="dcb68-149">[webPart][]</span></span>                | <span data-ttu-id="dcb68-150">Веб-части на странице.</span><span class="sxs-lookup"><span data-stu-id="dcb68-150">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="dcb68-151">Метаданные для разработки</span><span class="sxs-lookup"><span data-stu-id="dcb68-151">Authoring Metadata</span></span>

<span data-ttu-id="dcb68-152">Ресурс **ситепаже** содержит следующие метаданные, связанные с созданием и отправкой.</span><span class="sxs-lookup"><span data-stu-id="dcb68-152">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="dcb68-153">Свойство Публишингстате будет отражать состояние создания страницы, например извлеченный или опубликованный.</span><span class="sxs-lookup"><span data-stu-id="dcb68-153">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="dcb68-154">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dcb68-154">Property name</span></span>          | <span data-ttu-id="dcb68-155">Тип</span><span class="sxs-lookup"><span data-stu-id="dcb68-155">Type</span></span>                   | <span data-ttu-id="dcb68-156">Описание</span><span class="sxs-lookup"><span data-stu-id="dcb68-156">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="dcb68-157">publishingState</span><span class="sxs-lookup"><span data-stu-id="dcb68-157">publishingState</span></span>        | <span data-ttu-id="dcb68-158">[publicationFacet][].</span><span class="sxs-lookup"><span data-stu-id="dcb68-158">[publicationFacet][]</span></span>   | <span data-ttu-id="dcb68-159">Состояние публикации и версия MM.mm страницы.</span><span class="sxs-lookup"><span data-stu-id="dcb68-159">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="dcb68-160">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="dcb68-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="dcb68-161">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dcb68-161">Property name</span></span>        | <span data-ttu-id="dcb68-162">Тип</span><span class="sxs-lookup"><span data-stu-id="dcb68-162">Type</span></span>              | <span data-ttu-id="dcb68-163">Описание</span><span class="sxs-lookup"><span data-stu-id="dcb68-163">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="dcb68-164">id</span><span class="sxs-lookup"><span data-stu-id="dcb68-164">id</span></span>                   | <span data-ttu-id="dcb68-165">string</span><span class="sxs-lookup"><span data-stu-id="dcb68-165">string</span></span>            | <span data-ttu-id="dcb68-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcb68-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="dcb68-168">name</span><span class="sxs-lookup"><span data-stu-id="dcb68-168">name</span></span>                 | <span data-ttu-id="dcb68-169">string</span><span class="sxs-lookup"><span data-stu-id="dcb68-169">string</span></span>            | <span data-ttu-id="dcb68-170">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="dcb68-170">The name / title of the item.</span></span>
| <span data-ttu-id="dcb68-171">createdBy</span><span class="sxs-lookup"><span data-stu-id="dcb68-171">createdBy</span></span>            | <span data-ttu-id="dcb68-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dcb68-172">[identitySet][]</span></span>   | <span data-ttu-id="dcb68-173">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="dcb68-173">Identity of the creator of this item.</span></span> <span data-ttu-id="dcb68-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcb68-174">Read-only.</span></span>
| <span data-ttu-id="dcb68-175">eTag</span><span class="sxs-lookup"><span data-stu-id="dcb68-175">eTag</span></span>                 | <span data-ttu-id="dcb68-176">string</span><span class="sxs-lookup"><span data-stu-id="dcb68-176">string</span></span>            | <span data-ttu-id="dcb68-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcb68-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="dcb68-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="dcb68-179">lastModifiedBy</span></span>       | <span data-ttu-id="dcb68-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dcb68-180">[identitySet][]</span></span>   | <span data-ttu-id="dcb68-181">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="dcb68-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="dcb68-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcb68-182">Read-only.</span></span>
| <span data-ttu-id="dcb68-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dcb68-183">lastModifiedDateTime</span></span> | <span data-ttu-id="dcb68-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcb68-184">DateTimeOffset</span></span>    | <span data-ttu-id="dcb68-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcb68-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="dcb68-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="dcb68-187">parentReference</span></span>      | <span data-ttu-id="dcb68-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="dcb68-188">[itemReference][]</span></span> | <span data-ttu-id="dcb68-189">Сведения о родительском элементе, если элемент выступает в роли родительского элемента.</span><span class="sxs-lookup"><span data-stu-id="dcb68-189">Parent information, if the item has a parent.</span></span> <span data-ttu-id="dcb68-190">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcb68-190">Read-only.</span></span>
| <span data-ttu-id="dcb68-191">webUrl</span><span class="sxs-lookup"><span data-stu-id="dcb68-191">webUrl</span></span>               | <span data-ttu-id="dcb68-192">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="dcb68-192">string (url)</span></span>      | <span data-ttu-id="dcb68-p110">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcb68-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="dcb68-195">Связи</span><span class="sxs-lookup"><span data-stu-id="dcb68-195">Relationships</span></span>

<span data-ttu-id="dcb68-196">У ресурса **ситепаже** нет отношений с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="dcb68-196">The **sitePage** resource does not have relationships to other resources.</span></span>

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


