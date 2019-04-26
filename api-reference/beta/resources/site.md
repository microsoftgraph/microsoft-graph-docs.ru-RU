---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 63d4232c2af37541f2a96359f9d2a209d065bc98
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343061"
---
# <a name="site-resource-type"></a><span data-ttu-id="ec309-102">Тип ресурса site</span><span class="sxs-lookup"><span data-stu-id="ec309-102">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec309-103">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ec309-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="ec309-104">Методы</span><span class="sxs-lookup"><span data-stu-id="ec309-104">Methods</span></span>

| <span data-ttu-id="ec309-105">Метод</span><span class="sxs-lookup"><span data-stu-id="ec309-105">Method</span></span>                         | <span data-ttu-id="ec309-106">Путь REST</span><span class="sxs-lookup"><span data-stu-id="ec309-106">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="ec309-107">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="ec309-107">[Get root site][]</span></span>              | <span data-ttu-id="ec309-108">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="ec309-108">GET /sites/root</span></span>
| <span data-ttu-id="ec309-109">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="ec309-109">[Get site][]</span></span>                   | <span data-ttu-id="ec309-110">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="ec309-110">GET /sites/{site-id}</span></span>
| <span data-ttu-id="ec309-111">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="ec309-111">[Get site by path][]</span></span>           | <span data-ttu-id="ec309-112">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="ec309-112">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="ec309-113">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="ec309-113">[Get site for a group][]</span></span>       | <span data-ttu-id="ec309-114">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="ec309-114">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="ec309-115">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="ec309-115">[Get analytics][]</span></span>              | <span data-ttu-id="ec309-116">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="ec309-116">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="ec309-117">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="ec309-117">[Get activities by interval][]</span></span> | <span data-ttu-id="ec309-118">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="ec309-118">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="ec309-119">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="ec309-119">[List pages][]</span></span>                 | <span data-ttu-id="ec309-120">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="ec309-120">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="ec309-121">[Перечисление корневых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="ec309-121">[List root sites][]</span></span>            | <span data-ttu-id="ec309-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="ec309-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="ec309-123">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="ec309-123">[Search for sites][]</span></span>           | <span data-ttu-id="ec309-124">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="ec309-124">GET /sites?search={query}</span></span>

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


## <a name="properties"></a><span data-ttu-id="ec309-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec309-134">Properties</span></span>

| <span data-ttu-id="ec309-135">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ec309-135">Property name</span></span>            | <span data-ttu-id="ec309-136">Тип</span><span class="sxs-lookup"><span data-stu-id="ec309-136">Type</span></span>               | <span data-ttu-id="ec309-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ec309-137">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="ec309-138">**id**</span><span class="sxs-lookup"><span data-stu-id="ec309-138">**id**</span></span>                   | <span data-ttu-id="ec309-139">string</span><span class="sxs-lookup"><span data-stu-id="ec309-139">string</span></span>             | <span data-ttu-id="ec309-p101">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec309-p101">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="ec309-142">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ec309-142">**createdDateTime**</span></span>      | <span data-ttu-id="ec309-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec309-143">DateTimeOffset</span></span>     | <span data-ttu-id="ec309-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec309-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ec309-146">**description**</span><span class="sxs-lookup"><span data-stu-id="ec309-146">**description**</span></span>          | <span data-ttu-id="ec309-147">string</span><span class="sxs-lookup"><span data-stu-id="ec309-147">string</span></span>             | <span data-ttu-id="ec309-148">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="ec309-148">The descriptive text for the site.</span></span>
| <span data-ttu-id="ec309-149">**eTag**</span><span class="sxs-lookup"><span data-stu-id="ec309-149">**eTag**</span></span>                 | <span data-ttu-id="ec309-150">string</span><span class="sxs-lookup"><span data-stu-id="ec309-150">string</span></span>             | <span data-ttu-id="ec309-p103">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec309-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="ec309-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ec309-153">**displayName**</span></span>          | <span data-ttu-id="ec309-154">string</span><span class="sxs-lookup"><span data-stu-id="ec309-154">string</span></span>             | <span data-ttu-id="ec309-p104">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec309-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="ec309-157">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ec309-157">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ec309-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec309-158">DateTimeOffset</span></span>     | <span data-ttu-id="ec309-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec309-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ec309-161">**name**</span><span class="sxs-lookup"><span data-stu-id="ec309-161">**name**</span></span>                 | <span data-ttu-id="ec309-162">string</span><span class="sxs-lookup"><span data-stu-id="ec309-162">string</span></span>             | <span data-ttu-id="ec309-163">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="ec309-163">The name / title of the item.</span></span>
| <span data-ttu-id="ec309-164">**root**</span><span class="sxs-lookup"><span data-stu-id="ec309-164">**root**</span></span>                 | <span data-ttu-id="ec309-165">[root][]</span><span class="sxs-lookup"><span data-stu-id="ec309-165">[root][]</span></span>           | <span data-ttu-id="ec309-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec309-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="ec309-168">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="ec309-168">**sharepointIds**</span></span>        | <span data-ttu-id="ec309-169">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ec309-169">[sharepointIds][]</span></span>  | <span data-ttu-id="ec309-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec309-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ec309-172">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="ec309-172">**siteCollection**</span></span>       | <span data-ttu-id="ec309-173">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="ec309-173">[siteCollection][]</span></span> | <span data-ttu-id="ec309-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec309-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="ec309-177">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="ec309-177">**webUrl**</span></span>               | <span data-ttu-id="ec309-178">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="ec309-178">string (url)</span></span>       | <span data-ttu-id="ec309-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec309-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="ec309-181">Связи</span><span class="sxs-lookup"><span data-stu-id="ec309-181">Relationships</span></span>

| <span data-ttu-id="ec309-182">Имя связи</span><span class="sxs-lookup"><span data-stu-id="ec309-182">Relationship name</span></span> | <span data-ttu-id="ec309-183">Тип</span><span class="sxs-lookup"><span data-stu-id="ec309-183">Type</span></span>                             | <span data-ttu-id="ec309-184">Описание</span><span class="sxs-lookup"><span data-stu-id="ec309-184">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="ec309-185">**analytics**</span><span class="sxs-lookup"><span data-stu-id="ec309-185">**analytics**</span></span>     | <span data-ttu-id="ec309-186">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="ec309-186">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="ec309-187">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ec309-187">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="ec309-188">**columns**</span><span class="sxs-lookup"><span data-stu-id="ec309-188">**columns**</span></span>       | <span data-ttu-id="ec309-189">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="ec309-189">Collection([columnDefinition][])</span></span> | <span data-ttu-id="ec309-190">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ec309-190">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="ec309-191">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="ec309-191">**contentTypes**</span></span>  | <span data-ttu-id="ec309-192">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="ec309-192">Collection([contentType][])</span></span>      | <span data-ttu-id="ec309-193">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="ec309-193">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="ec309-194">**drive**</span><span class="sxs-lookup"><span data-stu-id="ec309-194">**drive**</span></span>         | <span data-ttu-id="ec309-195">[drive][]</span><span class="sxs-lookup"><span data-stu-id="ec309-195">[drive][]</span></span>                        | <span data-ttu-id="ec309-196">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="ec309-196">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="ec309-197">**drives**</span><span class="sxs-lookup"><span data-stu-id="ec309-197">**drives**</span></span>        | <span data-ttu-id="ec309-198">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="ec309-198">Collection([drive][])</span></span>            | <span data-ttu-id="ec309-199">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ec309-199">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="ec309-200">**items**</span><span class="sxs-lookup"><span data-stu-id="ec309-200">**items**</span></span>         | <span data-ttu-id="ec309-201">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="ec309-201">Collection([baseItem][])</span></span>         | <span data-ttu-id="ec309-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="ec309-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="ec309-204">**lists**</span><span class="sxs-lookup"><span data-stu-id="ec309-204">**lists**</span></span>         | <span data-ttu-id="ec309-205">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="ec309-205">Collection([list][])</span></span>             | <span data-ttu-id="ec309-206">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ec309-206">The collection of lists under this site.</span></span>
| <span data-ttu-id="ec309-207">**pages**</span><span class="sxs-lookup"><span data-stu-id="ec309-207">**pages**</span></span>         | <span data-ttu-id="ec309-208">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="ec309-208">Collection([sitePage][])</span></span>         | <span data-ttu-id="ec309-209">Коллекция страниц в списке SitePages на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ec309-209">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="ec309-210">**sites**</span><span class="sxs-lookup"><span data-stu-id="ec309-210">**sites**</span></span>         | <span data-ttu-id="ec309-211">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="ec309-211">Collection([site][])</span></span>             | <span data-ttu-id="ec309-212">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="ec309-212">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="ec309-224">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec309-224">JSON representation</span></span>

<span data-ttu-id="ec309-225">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec309-225">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="ec309-226">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="ec309-226">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
