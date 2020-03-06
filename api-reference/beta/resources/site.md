---
author: JeremyKelley
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: be567e1ba44790c54127ccee17dbb0d396f15e0c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520557"
---
# <a name="site-resource-type"></a><span data-ttu-id="43452-103">Тип ресурса site</span><span class="sxs-lookup"><span data-stu-id="43452-103">site resource type</span></span>

<span data-ttu-id="43452-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43452-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43452-105">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="43452-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="43452-106">Методы</span><span class="sxs-lookup"><span data-stu-id="43452-106">Methods</span></span>

| <span data-ttu-id="43452-107">Метод</span><span class="sxs-lookup"><span data-stu-id="43452-107">Method</span></span>                         | <span data-ttu-id="43452-108">Путь REST</span><span class="sxs-lookup"><span data-stu-id="43452-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="43452-109">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="43452-109">[Get root site][]</span></span>              | <span data-ttu-id="43452-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="43452-110">GET /sites/root</span></span>
| <span data-ttu-id="43452-111">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="43452-111">[Get site][]</span></span>                   | <span data-ttu-id="43452-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="43452-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="43452-113">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="43452-113">[Get site by path][]</span></span>           | <span data-ttu-id="43452-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="43452-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="43452-115">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="43452-115">[Get site for a group][]</span></span>       | <span data-ttu-id="43452-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="43452-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="43452-117">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="43452-117">[Get analytics][]</span></span>              | <span data-ttu-id="43452-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="43452-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="43452-119">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="43452-119">[Get activities by interval][]</span></span> | <span data-ttu-id="43452-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="43452-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="43452-121">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="43452-121">[List pages][]</span></span>                 | <span data-ttu-id="43452-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="43452-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="43452-123">[Перечисление корневых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="43452-123">[List root sites][]</span></span>            | <span data-ttu-id="43452-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="43452-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="43452-125">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="43452-125">[Search for sites][]</span></span>           | <span data-ttu-id="43452-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="43452-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="43452-127">[Отслеживание сайта][]</span><span class="sxs-lookup"><span data-stu-id="43452-127">[Follow Site][]</span></span>                | <span data-ttu-id="43452-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="43452-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="43452-129">[Прекращение отслеживания сайта][]</span><span class="sxs-lookup"><span data-stu-id="43452-129">[Unfollow Site][]</span></span>              | <span data-ttu-id="43452-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="43452-130">POST /users/{user-id}/followedSites/remove</span></span>

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


## <a name="properties"></a><span data-ttu-id="43452-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="43452-142">Properties</span></span>

| <span data-ttu-id="43452-143">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="43452-143">Property name</span></span>            | <span data-ttu-id="43452-144">Тип</span><span class="sxs-lookup"><span data-stu-id="43452-144">Type</span></span>               | <span data-ttu-id="43452-145">Описание</span><span class="sxs-lookup"><span data-stu-id="43452-145">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="43452-146">**id**</span><span class="sxs-lookup"><span data-stu-id="43452-146">**id**</span></span>                   | <span data-ttu-id="43452-147">строка</span><span class="sxs-lookup"><span data-stu-id="43452-147">string</span></span>             | <span data-ttu-id="43452-148">[Уникальный идентификатор](#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="43452-148">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="43452-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43452-149">Read-only.</span></span>
| <span data-ttu-id="43452-150">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="43452-150">**createdDateTime**</span></span>      | <span data-ttu-id="43452-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43452-151">DateTimeOffset</span></span>     | <span data-ttu-id="43452-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43452-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="43452-154">**description**</span><span class="sxs-lookup"><span data-stu-id="43452-154">**description**</span></span>          | <span data-ttu-id="43452-155">string</span><span class="sxs-lookup"><span data-stu-id="43452-155">string</span></span>             | <span data-ttu-id="43452-156">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="43452-156">The descriptive text for the site.</span></span>
| <span data-ttu-id="43452-157">**eTag**</span><span class="sxs-lookup"><span data-stu-id="43452-157">**eTag**</span></span>                 | <span data-ttu-id="43452-158">string</span><span class="sxs-lookup"><span data-stu-id="43452-158">string</span></span>             | <span data-ttu-id="43452-p103">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43452-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="43452-161">**displayName**</span><span class="sxs-lookup"><span data-stu-id="43452-161">**displayName**</span></span>          | <span data-ttu-id="43452-162">string</span><span class="sxs-lookup"><span data-stu-id="43452-162">string</span></span>             | <span data-ttu-id="43452-p104">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43452-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="43452-165">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="43452-165">**lastModifiedDateTime**</span></span> | <span data-ttu-id="43452-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43452-166">DateTimeOffset</span></span>     | <span data-ttu-id="43452-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43452-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="43452-169">**name**</span><span class="sxs-lookup"><span data-stu-id="43452-169">**name**</span></span>                 | <span data-ttu-id="43452-170">string</span><span class="sxs-lookup"><span data-stu-id="43452-170">string</span></span>             | <span data-ttu-id="43452-171">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="43452-171">The name / title of the item.</span></span>
| <span data-ttu-id="43452-172">**root**</span><span class="sxs-lookup"><span data-stu-id="43452-172">**root**</span></span>                 | <span data-ttu-id="43452-173">[root][]</span><span class="sxs-lookup"><span data-stu-id="43452-173">[root][]</span></span>           | <span data-ttu-id="43452-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43452-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="43452-176">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="43452-176">**sharepointIds**</span></span>        | <span data-ttu-id="43452-177">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="43452-177">[sharepointIds][]</span></span>  | <span data-ttu-id="43452-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43452-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="43452-180">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="43452-180">**siteCollection**</span></span>       | <span data-ttu-id="43452-181">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="43452-181">[siteCollection][]</span></span> | <span data-ttu-id="43452-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43452-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="43452-185">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="43452-185">**webUrl**</span></span>               | <span data-ttu-id="43452-186">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="43452-186">string (url)</span></span>       | <span data-ttu-id="43452-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43452-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="43452-189">Свойство id</span><span class="sxs-lookup"><span data-stu-id="43452-189">id property</span></span>
<span data-ttu-id="43452-190">Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="43452-190">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="43452-191">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="43452-191">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="43452-192">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="43452-192">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="43452-193">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="43452-193">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="43452-194">Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="43452-194">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="43452-195">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="43452-195">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="43452-196">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="43452-196">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="43452-197">Связи</span><span class="sxs-lookup"><span data-stu-id="43452-197">Relationships</span></span>

| <span data-ttu-id="43452-198">Имя связи</span><span class="sxs-lookup"><span data-stu-id="43452-198">Relationship name</span></span> | <span data-ttu-id="43452-199">Тип</span><span class="sxs-lookup"><span data-stu-id="43452-199">Type</span></span>                             | <span data-ttu-id="43452-200">Описание</span><span class="sxs-lookup"><span data-stu-id="43452-200">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="43452-201">**analytics**</span><span class="sxs-lookup"><span data-stu-id="43452-201">**analytics**</span></span>     | <span data-ttu-id="43452-202">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="43452-202">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="43452-203">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="43452-203">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="43452-204">**columns**</span><span class="sxs-lookup"><span data-stu-id="43452-204">**columns**</span></span>       | <span data-ttu-id="43452-205">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="43452-205">Collection([columnDefinition][])</span></span> | <span data-ttu-id="43452-206">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="43452-206">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="43452-207">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="43452-207">**contentTypes**</span></span>  | <span data-ttu-id="43452-208">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="43452-208">Collection([contentType][])</span></span>      | <span data-ttu-id="43452-209">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="43452-209">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="43452-210">**drive**</span><span class="sxs-lookup"><span data-stu-id="43452-210">**drive**</span></span>         | <span data-ttu-id="43452-211">[drive][]</span><span class="sxs-lookup"><span data-stu-id="43452-211">[drive][]</span></span>                        | <span data-ttu-id="43452-212">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="43452-212">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="43452-213">**drives**</span><span class="sxs-lookup"><span data-stu-id="43452-213">**drives**</span></span>        | <span data-ttu-id="43452-214">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="43452-214">Collection([drive][])</span></span>            | <span data-ttu-id="43452-215">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="43452-215">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="43452-216">**items**</span><span class="sxs-lookup"><span data-stu-id="43452-216">**items**</span></span>         | <span data-ttu-id="43452-217">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="43452-217">Collection([baseItem][])</span></span>         | <span data-ttu-id="43452-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="43452-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="43452-220">**lists**</span><span class="sxs-lookup"><span data-stu-id="43452-220">**lists**</span></span>         | <span data-ttu-id="43452-221">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="43452-221">Collection([list][])</span></span>             | <span data-ttu-id="43452-222">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="43452-222">The collection of lists under this site.</span></span>
| <span data-ttu-id="43452-223">**pages**</span><span class="sxs-lookup"><span data-stu-id="43452-223">**pages**</span></span>         | <span data-ttu-id="43452-224">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="43452-224">Collection([sitePage][])</span></span>         | <span data-ttu-id="43452-225">Коллекция страниц в списке SitePages на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="43452-225">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="43452-226">**sites**</span><span class="sxs-lookup"><span data-stu-id="43452-226">**sites**</span></span>         | <span data-ttu-id="43452-227">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="43452-227">Collection([site][])</span></span>             | <span data-ttu-id="43452-228">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="43452-228">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="43452-240">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43452-240">JSON representation</span></span>

<span data-ttu-id="43452-241">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43452-241">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="43452-242">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="43452-242">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
