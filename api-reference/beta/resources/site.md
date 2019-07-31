---
author: JeremyKelley
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 691f91b63fdff583476c5308f4b8370a563120a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008357"
---
# <a name="site-resource-type"></a><span data-ttu-id="39ea8-103">Тип ресурса site</span><span class="sxs-lookup"><span data-stu-id="39ea8-103">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39ea8-104">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="39ea8-104">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="39ea8-105">Методы</span><span class="sxs-lookup"><span data-stu-id="39ea8-105">Methods</span></span>

| <span data-ttu-id="39ea8-106">Метод</span><span class="sxs-lookup"><span data-stu-id="39ea8-106">Method</span></span>                         | <span data-ttu-id="39ea8-107">Путь REST</span><span class="sxs-lookup"><span data-stu-id="39ea8-107">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="39ea8-108">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-108">[Get root site][]</span></span>              | <span data-ttu-id="39ea8-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="39ea8-109">GET /sites/root</span></span>
| <span data-ttu-id="39ea8-110">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-110">[Get site][]</span></span>                   | <span data-ttu-id="39ea8-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="39ea8-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="39ea8-112">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-112">[Get site by path][]</span></span>           | <span data-ttu-id="39ea8-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="39ea8-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="39ea8-114">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-114">[Get site for a group][]</span></span>       | <span data-ttu-id="39ea8-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="39ea8-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="39ea8-116">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-116">[Get analytics][]</span></span>              | <span data-ttu-id="39ea8-117">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="39ea8-117">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="39ea8-118">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-118">[Get activities by interval][]</span></span> | <span data-ttu-id="39ea8-119">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="39ea8-119">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="39ea8-120">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-120">[List pages][]</span></span>                 | <span data-ttu-id="39ea8-121">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="39ea8-121">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="39ea8-122">[Перечисление корневых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-122">[List root sites][]</span></span>            | <span data-ttu-id="39ea8-123">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="39ea8-123">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="39ea8-124">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-124">[Search for sites][]</span></span>           | <span data-ttu-id="39ea8-125">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="39ea8-125">GET /sites?search={query}</span></span>
| <span data-ttu-id="39ea8-126">[Отслеживание сайта][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-126">[Follow Site][]</span></span>                | <span data-ttu-id="39ea8-127">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="39ea8-127">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="39ea8-128">[Прекращение отслеживания сайта][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-128">[Unfollow Site][]</span></span>              | <span data-ttu-id="39ea8-129">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="39ea8-129">POST /users/{user-id}/followedSites/remove</span></span>

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


## <a name="properties"></a><span data-ttu-id="39ea8-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="39ea8-141">Properties</span></span>

| <span data-ttu-id="39ea8-142">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="39ea8-142">Property name</span></span>            | <span data-ttu-id="39ea8-143">Тип</span><span class="sxs-lookup"><span data-stu-id="39ea8-143">Type</span></span>               | <span data-ttu-id="39ea8-144">Описание</span><span class="sxs-lookup"><span data-stu-id="39ea8-144">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="39ea8-145">**id**</span><span class="sxs-lookup"><span data-stu-id="39ea8-145">**id**</span></span>                   | <span data-ttu-id="39ea8-146">строка</span><span class="sxs-lookup"><span data-stu-id="39ea8-146">string</span></span>             | <span data-ttu-id="39ea8-147">[Уникальный идентификатор](#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="39ea8-147">The unique identifier of the item.</span></span> <span data-ttu-id="39ea8-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ea8-148">Read-only.</span></span>
| <span data-ttu-id="39ea8-149">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="39ea8-149">**createdDateTime**</span></span>      | <span data-ttu-id="39ea8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ea8-150">DateTimeOffset</span></span>     | <span data-ttu-id="39ea8-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ea8-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="39ea8-153">**description**</span><span class="sxs-lookup"><span data-stu-id="39ea8-153">**description**</span></span>          | <span data-ttu-id="39ea8-154">string</span><span class="sxs-lookup"><span data-stu-id="39ea8-154">string</span></span>             | <span data-ttu-id="39ea8-155">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="39ea8-155">The descriptive text for the site.</span></span>
| <span data-ttu-id="39ea8-156">**eTag**</span><span class="sxs-lookup"><span data-stu-id="39ea8-156">**eTag**</span></span>                 | <span data-ttu-id="39ea8-157">string</span><span class="sxs-lookup"><span data-stu-id="39ea8-157">string</span></span>             | <span data-ttu-id="39ea8-p103">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ea8-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="39ea8-160">**displayName**</span><span class="sxs-lookup"><span data-stu-id="39ea8-160">**displayName**</span></span>          | <span data-ttu-id="39ea8-161">string</span><span class="sxs-lookup"><span data-stu-id="39ea8-161">string</span></span>             | <span data-ttu-id="39ea8-p104">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ea8-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="39ea8-164">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="39ea8-164">**lastModifiedDateTime**</span></span> | <span data-ttu-id="39ea8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ea8-165">DateTimeOffset</span></span>     | <span data-ttu-id="39ea8-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ea8-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="39ea8-168">**name**</span><span class="sxs-lookup"><span data-stu-id="39ea8-168">**name**</span></span>                 | <span data-ttu-id="39ea8-169">string</span><span class="sxs-lookup"><span data-stu-id="39ea8-169">string</span></span>             | <span data-ttu-id="39ea8-170">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="39ea8-170">The name / title of the item.</span></span>
| <span data-ttu-id="39ea8-171">**root**</span><span class="sxs-lookup"><span data-stu-id="39ea8-171">**root**</span></span>                 | <span data-ttu-id="39ea8-172">[root][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-172">[root][]</span></span>           | <span data-ttu-id="39ea8-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ea8-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="39ea8-175">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="39ea8-175">**sharepointIds**</span></span>        | <span data-ttu-id="39ea8-176">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-176">[sharepointIds][]</span></span>  | <span data-ttu-id="39ea8-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ea8-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="39ea8-179">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="39ea8-179">**siteCollection**</span></span>       | <span data-ttu-id="39ea8-180">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-180">[siteCollection][]</span></span> | <span data-ttu-id="39ea8-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ea8-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="39ea8-184">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="39ea8-184">**webUrl**</span></span>               | <span data-ttu-id="39ea8-185">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="39ea8-185">string (url)</span></span>       | <span data-ttu-id="39ea8-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ea8-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="39ea8-188">Свойство id</span><span class="sxs-lookup"><span data-stu-id="39ea8-188">id property</span></span>
<span data-ttu-id="39ea8-189">Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="39ea8-189">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>
* <span data-ttu-id="39ea8-190">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="39ea8-190">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="39ea8-191">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="39ea8-191">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="39ea8-192">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="39ea8-192">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="39ea8-193">Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="39ea8-193">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="39ea8-194">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="39ea8-194">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="39ea8-195">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="39ea8-195">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="39ea8-196">Связи</span><span class="sxs-lookup"><span data-stu-id="39ea8-196">Relationships</span></span>

| <span data-ttu-id="39ea8-197">Имя связи</span><span class="sxs-lookup"><span data-stu-id="39ea8-197">Relationship name</span></span> | <span data-ttu-id="39ea8-198">Тип</span><span class="sxs-lookup"><span data-stu-id="39ea8-198">Type</span></span>                             | <span data-ttu-id="39ea8-199">Описание</span><span class="sxs-lookup"><span data-stu-id="39ea8-199">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="39ea8-200">**analytics**</span><span class="sxs-lookup"><span data-stu-id="39ea8-200">**analytics**</span></span>     | <span data-ttu-id="39ea8-201">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-201">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="39ea8-202">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="39ea8-202">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="39ea8-203">**columns**</span><span class="sxs-lookup"><span data-stu-id="39ea8-203">**columns**</span></span>       | <span data-ttu-id="39ea8-204">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="39ea8-204">Collection([columnDefinition][])</span></span> | <span data-ttu-id="39ea8-205">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="39ea8-205">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="39ea8-206">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="39ea8-206">**contentTypes**</span></span>  | <span data-ttu-id="39ea8-207">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="39ea8-207">Collection([contentType][])</span></span>      | <span data-ttu-id="39ea8-208">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="39ea8-208">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="39ea8-209">**drive**</span><span class="sxs-lookup"><span data-stu-id="39ea8-209">**drive**</span></span>         | <span data-ttu-id="39ea8-210">[drive][]</span><span class="sxs-lookup"><span data-stu-id="39ea8-210">[drive][]</span></span>                        | <span data-ttu-id="39ea8-211">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="39ea8-211">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="39ea8-212">**drives**</span><span class="sxs-lookup"><span data-stu-id="39ea8-212">**drives**</span></span>        | <span data-ttu-id="39ea8-213">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="39ea8-213">Collection([drive][])</span></span>            | <span data-ttu-id="39ea8-214">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="39ea8-214">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="39ea8-215">**items**</span><span class="sxs-lookup"><span data-stu-id="39ea8-215">**items**</span></span>         | <span data-ttu-id="39ea8-216">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="39ea8-216">Collection([baseItem][])</span></span>         | <span data-ttu-id="39ea8-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="39ea8-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="39ea8-219">**lists**</span><span class="sxs-lookup"><span data-stu-id="39ea8-219">**lists**</span></span>         | <span data-ttu-id="39ea8-220">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="39ea8-220">Collection([list][])</span></span>             | <span data-ttu-id="39ea8-221">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="39ea8-221">The collection of lists under this site.</span></span>
| <span data-ttu-id="39ea8-222">**pages**</span><span class="sxs-lookup"><span data-stu-id="39ea8-222">**pages**</span></span>         | <span data-ttu-id="39ea8-223">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="39ea8-223">Collection([sitePage][])</span></span>         | <span data-ttu-id="39ea8-224">Коллекция страниц в списке SitePages на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="39ea8-224">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="39ea8-225">**sites**</span><span class="sxs-lookup"><span data-stu-id="39ea8-225">**sites**</span></span>         | <span data-ttu-id="39ea8-226">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="39ea8-226">Collection([site][])</span></span>             | <span data-ttu-id="39ea8-227">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="39ea8-227">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="39ea8-239">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39ea8-239">JSON representation</span></span>

<span data-ttu-id="39ea8-240">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39ea8-240">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="39ea8-241">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="39ea8-241">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
