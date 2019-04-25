---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: d2fbdcb870d86efb983de1e3ba75154b6e15f619
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522007"
---
# <a name="site-resource-type"></a><span data-ttu-id="f4b81-102">Тип ресурса site</span><span class="sxs-lookup"><span data-stu-id="f4b81-102">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4b81-103">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f4b81-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="f4b81-104">Методы</span><span class="sxs-lookup"><span data-stu-id="f4b81-104">Methods</span></span>

| <span data-ttu-id="f4b81-105">Метод</span><span class="sxs-lookup"><span data-stu-id="f4b81-105">Method</span></span>                         | <span data-ttu-id="f4b81-106">Путь REST</span><span class="sxs-lookup"><span data-stu-id="f4b81-106">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="f4b81-107">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-107">[Get root site][]</span></span>              | <span data-ttu-id="f4b81-108">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="f4b81-108">GET /sites/root</span></span>
| <span data-ttu-id="f4b81-109">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-109">[Get site][]</span></span>                   | <span data-ttu-id="f4b81-110">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="f4b81-110">GET /sites/{site-id}</span></span>
| <span data-ttu-id="f4b81-111">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-111">[Get site by path][]</span></span>           | <span data-ttu-id="f4b81-112">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="f4b81-112">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="f4b81-113">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-113">[Get site for a group][]</span></span>       | <span data-ttu-id="f4b81-114">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="f4b81-114">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="f4b81-115">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-115">[Get analytics][]</span></span>              | <span data-ttu-id="f4b81-116">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="f4b81-116">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="f4b81-117">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-117">[Get activities by interval][]</span></span> | <span data-ttu-id="f4b81-118">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="f4b81-118">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="f4b81-119">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-119">[List pages][]</span></span>                 | <span data-ttu-id="f4b81-120">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="f4b81-120">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="f4b81-121">[Перечисление корневых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-121">[List root sites][]</span></span>            | <span data-ttu-id="f4b81-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="f4b81-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="f4b81-123">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-123">[Search for sites][]</span></span>           | <span data-ttu-id="f4b81-124">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="f4b81-124">GET /sites?search={query}</span></span>

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


## <a name="properties"></a><span data-ttu-id="f4b81-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4b81-134">Properties</span></span>

| <span data-ttu-id="f4b81-135">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f4b81-135">Property name</span></span>            | <span data-ttu-id="f4b81-136">Тип</span><span class="sxs-lookup"><span data-stu-id="f4b81-136">Type</span></span>               | <span data-ttu-id="f4b81-137">Описание</span><span class="sxs-lookup"><span data-stu-id="f4b81-137">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="f4b81-138">**id**</span><span class="sxs-lookup"><span data-stu-id="f4b81-138">**id**</span></span>                   | <span data-ttu-id="f4b81-139">string</span><span class="sxs-lookup"><span data-stu-id="f4b81-139">string</span></span>             | <span data-ttu-id="f4b81-p101">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4b81-p101">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="f4b81-142">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="f4b81-142">**createdDateTime**</span></span>      | <span data-ttu-id="f4b81-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4b81-143">DateTimeOffset</span></span>     | <span data-ttu-id="f4b81-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4b81-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="f4b81-146">**description**</span><span class="sxs-lookup"><span data-stu-id="f4b81-146">**description**</span></span>          | <span data-ttu-id="f4b81-147">string</span><span class="sxs-lookup"><span data-stu-id="f4b81-147">string</span></span>             | <span data-ttu-id="f4b81-148">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="f4b81-148">The descriptive text for the site.</span></span>
| <span data-ttu-id="f4b81-149">**eTag**</span><span class="sxs-lookup"><span data-stu-id="f4b81-149">**eTag**</span></span>                 | <span data-ttu-id="f4b81-150">string</span><span class="sxs-lookup"><span data-stu-id="f4b81-150">string</span></span>             | <span data-ttu-id="f4b81-p103">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4b81-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="f4b81-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="f4b81-153">**displayName**</span></span>          | <span data-ttu-id="f4b81-154">string</span><span class="sxs-lookup"><span data-stu-id="f4b81-154">string</span></span>             | <span data-ttu-id="f4b81-p104">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4b81-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="f4b81-157">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f4b81-157">**lastModifiedDateTime**</span></span> | <span data-ttu-id="f4b81-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4b81-158">DateTimeOffset</span></span>     | <span data-ttu-id="f4b81-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4b81-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f4b81-161">**name**</span><span class="sxs-lookup"><span data-stu-id="f4b81-161">**name**</span></span>                 | <span data-ttu-id="f4b81-162">string</span><span class="sxs-lookup"><span data-stu-id="f4b81-162">string</span></span>             | <span data-ttu-id="f4b81-163">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="f4b81-163">The name / title of the item.</span></span>
| <span data-ttu-id="f4b81-164">**root**</span><span class="sxs-lookup"><span data-stu-id="f4b81-164">**root**</span></span>                 | <span data-ttu-id="f4b81-165">[root][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-165">[root][]</span></span>           | <span data-ttu-id="f4b81-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4b81-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="f4b81-168">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="f4b81-168">**sharepointIds**</span></span>        | <span data-ttu-id="f4b81-169">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-169">[sharepointIds][]</span></span>  | <span data-ttu-id="f4b81-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4b81-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="f4b81-172">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="f4b81-172">**siteCollection**</span></span>       | <span data-ttu-id="f4b81-173">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-173">[siteCollection][]</span></span> | <span data-ttu-id="f4b81-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4b81-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="f4b81-177">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="f4b81-177">**webUrl**</span></span>               | <span data-ttu-id="f4b81-178">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="f4b81-178">string (url)</span></span>       | <span data-ttu-id="f4b81-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4b81-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="f4b81-181">Связи</span><span class="sxs-lookup"><span data-stu-id="f4b81-181">Relationships</span></span>

| <span data-ttu-id="f4b81-182">Имя связи</span><span class="sxs-lookup"><span data-stu-id="f4b81-182">Relationship name</span></span> | <span data-ttu-id="f4b81-183">Тип</span><span class="sxs-lookup"><span data-stu-id="f4b81-183">Type</span></span>                             | <span data-ttu-id="f4b81-184">Описание</span><span class="sxs-lookup"><span data-stu-id="f4b81-184">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="f4b81-185">**analytics**</span><span class="sxs-lookup"><span data-stu-id="f4b81-185">**analytics**</span></span>     | <span data-ttu-id="f4b81-186">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-186">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="f4b81-187">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f4b81-187">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="f4b81-188">**columns**</span><span class="sxs-lookup"><span data-stu-id="f4b81-188">**columns**</span></span>       | <span data-ttu-id="f4b81-189">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="f4b81-189">Collection([columnDefinition][])</span></span> | <span data-ttu-id="f4b81-190">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f4b81-190">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="f4b81-191">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="f4b81-191">**contentTypes**</span></span>  | <span data-ttu-id="f4b81-192">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="f4b81-192">Collection([contentType][])</span></span>      | <span data-ttu-id="f4b81-193">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="f4b81-193">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="f4b81-194">**drive**</span><span class="sxs-lookup"><span data-stu-id="f4b81-194">**drive**</span></span>         | <span data-ttu-id="f4b81-195">[drive][]</span><span class="sxs-lookup"><span data-stu-id="f4b81-195">[drive][]</span></span>                        | <span data-ttu-id="f4b81-196">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="f4b81-196">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="f4b81-197">**drives**</span><span class="sxs-lookup"><span data-stu-id="f4b81-197">**drives**</span></span>        | <span data-ttu-id="f4b81-198">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="f4b81-198">Collection([drive][])</span></span>            | <span data-ttu-id="f4b81-199">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f4b81-199">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="f4b81-200">**items**</span><span class="sxs-lookup"><span data-stu-id="f4b81-200">**items**</span></span>         | <span data-ttu-id="f4b81-201">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="f4b81-201">Collection([baseItem][])</span></span>         | <span data-ttu-id="f4b81-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="f4b81-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="f4b81-204">**lists**</span><span class="sxs-lookup"><span data-stu-id="f4b81-204">**lists**</span></span>         | <span data-ttu-id="f4b81-205">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="f4b81-205">Collection([list][])</span></span>             | <span data-ttu-id="f4b81-206">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f4b81-206">The collection of lists under this site.</span></span>
| <span data-ttu-id="f4b81-207">**pages**</span><span class="sxs-lookup"><span data-stu-id="f4b81-207">**pages**</span></span>         | <span data-ttu-id="f4b81-208">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="f4b81-208">Collection([sitePage][])</span></span>         | <span data-ttu-id="f4b81-209">Коллекция страниц в списке SitePages на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f4b81-209">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="f4b81-210">**sites**</span><span class="sxs-lookup"><span data-stu-id="f4b81-210">**sites**</span></span>         | <span data-ttu-id="f4b81-211">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="f4b81-211">Collection([site][])</span></span>             | <span data-ttu-id="f4b81-212">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="f4b81-212">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="f4b81-224">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4b81-224">JSON representation</span></span>

<span data-ttu-id="f4b81-225">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4b81-225">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="f4b81-226">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="f4b81-226">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/site.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
