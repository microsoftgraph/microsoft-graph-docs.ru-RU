---
author: JeremyKelley
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 625017970be66b64ffa593e726b6aaf647fe05d6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092288"
---
# <a name="site-resource-type"></a><span data-ttu-id="43693-103">Тип ресурса site</span><span class="sxs-lookup"><span data-stu-id="43693-103">site resource type</span></span>

<span data-ttu-id="43693-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43693-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43693-105">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="43693-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="43693-106">Методы</span><span class="sxs-lookup"><span data-stu-id="43693-106">Methods</span></span>

| <span data-ttu-id="43693-107">Метод</span><span class="sxs-lookup"><span data-stu-id="43693-107">Method</span></span>                         | <span data-ttu-id="43693-108">Путь REST</span><span class="sxs-lookup"><span data-stu-id="43693-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="43693-109">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="43693-109">[Get root site][]</span></span>              | <span data-ttu-id="43693-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="43693-110">GET /sites/root</span></span>
| <span data-ttu-id="43693-111">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="43693-111">[Get site][]</span></span>                   | <span data-ttu-id="43693-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="43693-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="43693-113">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="43693-113">[Get site by path][]</span></span>           | <span data-ttu-id="43693-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="43693-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="43693-115">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="43693-115">[Get site for a group][]</span></span>       | <span data-ttu-id="43693-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="43693-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="43693-117">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="43693-117">[Get analytics][]</span></span>              | <span data-ttu-id="43693-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="43693-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="43693-119">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="43693-119">[Get activities by interval][]</span></span> | <span data-ttu-id="43693-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="43693-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="43693-121">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="43693-121">[List pages][]</span></span>                 | <span data-ttu-id="43693-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="43693-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="43693-123">[Перечисление корневых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="43693-123">[List root sites][]</span></span>            | <span data-ttu-id="43693-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="43693-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="43693-125">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="43693-125">[Search for sites][]</span></span>           | <span data-ttu-id="43693-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="43693-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="43693-127">[Отслеживание сайта][]</span><span class="sxs-lookup"><span data-stu-id="43693-127">[Follow site][]</span></span>                | <span data-ttu-id="43693-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="43693-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="43693-129">[Прекращение отслеживания сайта][]</span><span class="sxs-lookup"><span data-stu-id="43693-129">[Unfollow site][]</span></span>              | <span data-ttu-id="43693-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="43693-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="43693-131">[Перечисление отслеживаемых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="43693-131">[List followed sites][]</span></span>        | <span data-ttu-id="43693-132">GET /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="43693-132">GET /me/followedSites</span></span>

[Получение сайта]: ../api/site-get.md
[Get site]: ../api/site-get.md
[Получение корневого сайта]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[Получение сайта по пути]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[Получение сайта для группы]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Перечисление страниц]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Перечисление корневых сайтов]: ../api/site-list.md
[List root sites]: ../api/site-list.md
[Поиск сайтов]: ../api/site-search.md
[Search for sites]: ../api/site-search.md
[Отслеживание сайта]: ../api/site-follow.md
[Follow site]: ../api/site-follow.md
[Прекращение отслеживания сайта]: ../api/site-unfollow.md
[Unfollow site]: ../api/site-unfollow.md
[Перечисление отслеживаемых сайтов]: ../api/sites-list-followed.md
[List followed sites]: ../api/sites-list-followed.md


## <a name="properties"></a><span data-ttu-id="43693-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="43693-145">Properties</span></span>

| <span data-ttu-id="43693-146">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="43693-146">Property name</span></span>            | <span data-ttu-id="43693-147">Тип</span><span class="sxs-lookup"><span data-stu-id="43693-147">Type</span></span>               | <span data-ttu-id="43693-148">Описание</span><span class="sxs-lookup"><span data-stu-id="43693-148">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="43693-149">**id**</span><span class="sxs-lookup"><span data-stu-id="43693-149">**id**</span></span>                   | <span data-ttu-id="43693-150">string</span><span class="sxs-lookup"><span data-stu-id="43693-150">string</span></span>             | <span data-ttu-id="43693-151">[Уникальный идентификатор](#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="43693-151">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="43693-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43693-152">Read-only.</span></span>
| <span data-ttu-id="43693-153">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="43693-153">**createdDateTime**</span></span>      | <span data-ttu-id="43693-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43693-154">DateTimeOffset</span></span>     | <span data-ttu-id="43693-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43693-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="43693-157">**description**</span><span class="sxs-lookup"><span data-stu-id="43693-157">**description**</span></span>          | <span data-ttu-id="43693-158">string</span><span class="sxs-lookup"><span data-stu-id="43693-158">string</span></span>             | <span data-ttu-id="43693-159">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="43693-159">The descriptive text for the site.</span></span>
| <span data-ttu-id="43693-160">**eTag**</span><span class="sxs-lookup"><span data-stu-id="43693-160">**eTag**</span></span>                 | <span data-ttu-id="43693-161">string</span><span class="sxs-lookup"><span data-stu-id="43693-161">string</span></span>             | <span data-ttu-id="43693-p103">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43693-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="43693-164">**displayName**</span><span class="sxs-lookup"><span data-stu-id="43693-164">**displayName**</span></span>          | <span data-ttu-id="43693-165">string</span><span class="sxs-lookup"><span data-stu-id="43693-165">string</span></span>             | <span data-ttu-id="43693-p104">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43693-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="43693-168">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="43693-168">**lastModifiedDateTime**</span></span> | <span data-ttu-id="43693-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43693-169">DateTimeOffset</span></span>     | <span data-ttu-id="43693-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43693-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="43693-172">**name**</span><span class="sxs-lookup"><span data-stu-id="43693-172">**name**</span></span>                 | <span data-ttu-id="43693-173">string</span><span class="sxs-lookup"><span data-stu-id="43693-173">string</span></span>             | <span data-ttu-id="43693-174">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="43693-174">The name / title of the item.</span></span>
| <span data-ttu-id="43693-175">**root**</span><span class="sxs-lookup"><span data-stu-id="43693-175">**root**</span></span>                 | <span data-ttu-id="43693-176">[root][]</span><span class="sxs-lookup"><span data-stu-id="43693-176">[root][]</span></span>           | <span data-ttu-id="43693-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43693-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="43693-179">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="43693-179">**sharepointIds**</span></span>        | <span data-ttu-id="43693-180">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="43693-180">[sharepointIds][]</span></span>  | <span data-ttu-id="43693-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43693-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="43693-183">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="43693-183">**siteCollection**</span></span>       | <span data-ttu-id="43693-184">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="43693-184">[siteCollection][]</span></span> | <span data-ttu-id="43693-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43693-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="43693-188">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="43693-188">**webUrl**</span></span>               | <span data-ttu-id="43693-189">string (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="43693-189">string (url)</span></span>       | <span data-ttu-id="43693-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43693-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="43693-192">Свойство id</span><span class="sxs-lookup"><span data-stu-id="43693-192">id property</span></span>
<span data-ttu-id="43693-193">Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="43693-193">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="43693-194">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="43693-194">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="43693-195">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="43693-195">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="43693-196">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="43693-196">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="43693-197">Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="43693-197">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="43693-198">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="43693-198">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="43693-199">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="43693-199">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="43693-200">Связи</span><span class="sxs-lookup"><span data-stu-id="43693-200">Relationships</span></span>

| <span data-ttu-id="43693-201">Имя связи</span><span class="sxs-lookup"><span data-stu-id="43693-201">Relationship name</span></span> | <span data-ttu-id="43693-202">Тип</span><span class="sxs-lookup"><span data-stu-id="43693-202">Type</span></span>                             | <span data-ttu-id="43693-203">Описание</span><span class="sxs-lookup"><span data-stu-id="43693-203">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="43693-204">**analytics**</span><span class="sxs-lookup"><span data-stu-id="43693-204">**analytics**</span></span>     | <span data-ttu-id="43693-205">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="43693-205">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="43693-206">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="43693-206">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="43693-207">**columns**</span><span class="sxs-lookup"><span data-stu-id="43693-207">**columns**</span></span>       | <span data-ttu-id="43693-208">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="43693-208">Collection([columnDefinition][])</span></span> | <span data-ttu-id="43693-209">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="43693-209">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="43693-210">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="43693-210">**contentTypes**</span></span>  | <span data-ttu-id="43693-211">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="43693-211">Collection([contentType][])</span></span>      | <span data-ttu-id="43693-212">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="43693-212">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="43693-213">**drive**</span><span class="sxs-lookup"><span data-stu-id="43693-213">**drive**</span></span>         | <span data-ttu-id="43693-214">[drive][]</span><span class="sxs-lookup"><span data-stu-id="43693-214">[drive][]</span></span>                        | <span data-ttu-id="43693-215">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="43693-215">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="43693-216">**drives**</span><span class="sxs-lookup"><span data-stu-id="43693-216">**drives**</span></span>        | <span data-ttu-id="43693-217">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="43693-217">Collection([drive][])</span></span>            | <span data-ttu-id="43693-218">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="43693-218">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="43693-219">**items**</span><span class="sxs-lookup"><span data-stu-id="43693-219">**items**</span></span>         | <span data-ttu-id="43693-220">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="43693-220">Collection([baseItem][])</span></span>         | <span data-ttu-id="43693-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="43693-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="43693-223">**lists**</span><span class="sxs-lookup"><span data-stu-id="43693-223">**lists**</span></span>         | <span data-ttu-id="43693-224">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="43693-224">Collection([list][])</span></span>             | <span data-ttu-id="43693-225">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="43693-225">The collection of lists under this site.</span></span>
| <span data-ttu-id="43693-226">**pages**</span><span class="sxs-lookup"><span data-stu-id="43693-226">**pages**</span></span>         | <span data-ttu-id="43693-227">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="43693-227">Collection([sitePage][])</span></span>         | <span data-ttu-id="43693-228">Коллекция страниц в списке SitePages на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="43693-228">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="43693-229">**sites**</span><span class="sxs-lookup"><span data-stu-id="43693-229">**sites**</span></span>         | <span data-ttu-id="43693-230">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="43693-230">Collection([site][])</span></span>             | <span data-ttu-id="43693-231">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="43693-231">The collection of the sub-sites under this site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="43693-243">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43693-243">JSON representation</span></span>

<span data-ttu-id="43693-244">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43693-244">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="43693-245">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="43693-245">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "sites"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.site"
}-->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": {
    "Resources/Site": "#"
  },
  "suppressions": []
}
-->


