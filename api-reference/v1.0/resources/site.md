---
author: JeremyKelley
ms.author: JeremyKelley
title: Ресурс site
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 40add99dfbeee28d82b3d02def833497c01385df
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968851"
---
# <a name="site-resource"></a><span data-ttu-id="5d01d-103">Ресурс site</span><span class="sxs-lookup"><span data-stu-id="5d01d-103">Site resource</span></span>

<span data-ttu-id="5d01d-104">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5d01d-104">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="5d01d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5d01d-105">Methods</span></span>

| <span data-ttu-id="5d01d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="5d01d-106">Method</span></span>                | <span data-ttu-id="5d01d-107">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="5d01d-107">Return type</span></span> | <span data-ttu-id="5d01d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5d01d-108">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="5d01d-109">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-109">[Get root site][]</span></span>        | <span data-ttu-id="5d01d-110">site</span><span class="sxs-lookup"><span data-stu-id="5d01d-110">Site</span></span> | <span data-ttu-id="5d01d-111">Получение доступа к корневому сайту SharePoint внутри клиента.</span><span class="sxs-lookup"><span data-stu-id="5d01d-111">To access the root SharePoint site within a tenant:</span></span>
| <span data-ttu-id="5d01d-112">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-112">[Get site][]</span></span>             | <span data-ttu-id="5d01d-113">site</span><span class="sxs-lookup"><span data-stu-id="5d01d-113">Site</span></span> | <span data-ttu-id="5d01d-114">Получение доступа к сайту SharePoint с помощью параметра siteId.</span><span class="sxs-lookup"><span data-stu-id="5d01d-114">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="5d01d-115">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-115">[Get site by path][]</span></span>     | <span data-ttu-id="5d01d-116">site</span><span class="sxs-lookup"><span data-stu-id="5d01d-116">Site</span></span> | <span data-ttu-id="5d01d-117">Получение доступа к корневому сайту SharePoint с использованием относительного пути.</span><span class="sxs-lookup"><span data-stu-id="5d01d-117">To access the root SharePoint site with a relative path:</span></span>
| <span data-ttu-id="5d01d-118">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-118">[Get site for a group][]</span></span> | <span data-ttu-id="5d01d-119">site</span><span class="sxs-lookup"><span data-stu-id="5d01d-119">Site</span></span> | <span data-ttu-id="5d01d-120">Получение доступа к сайту группы для группы.</span><span class="sxs-lookup"><span data-stu-id="5d01d-120">To access the team site for a group:</span></span>
| <span data-ttu-id="5d01d-121">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-121">[Get analytics][]</span></span>              | <span data-ttu-id="5d01d-122">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-122">[itemAnalytics][]</span></span> | <span data-ttu-id="5d01d-123">Получение аналитических данных для ресурса.</span><span class="sxs-lookup"><span data-stu-id="5d01d-123">Get analytics for this resource.</span></span> 
| <span data-ttu-id="5d01d-124">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-124">[Get activities by interval][]</span></span> | <span data-ttu-id="5d01d-125">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-125">[itemActivityStat][]</span></span> | <span data-ttu-id="5d01d-126">Получение коллекции объектов **itemActivityStats** в пределах указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="5d01d-126">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="5d01d-127">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-127">[Search for sites][]</span></span>     | <span data-ttu-id="5d01d-128">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="5d01d-128">Specifies a collection of site templates.</span></span> | <span data-ttu-id="5d01d-129">Поиск сайтов, соответствующих указанным ключевым словам, в клиенте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5d01d-129">Search across a SharePoint tenant for sites that match provided keywords.</span></span>

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
[Получение действий по интервалу]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md
[Поиск сайтов]: ../api/site-search.md
[Search for sites]: ../api/site-search.md
[itemActivityStat]: itemactivitystat.md

## <a name="properties"></a><span data-ttu-id="5d01d-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d01d-138">Properties</span></span>

| <span data-ttu-id="5d01d-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d01d-139">Property</span></span>            | <span data-ttu-id="5d01d-140">Тип</span><span class="sxs-lookup"><span data-stu-id="5d01d-140">Type</span></span>                                | <span data-ttu-id="5d01d-141">Описание</span><span class="sxs-lookup"><span data-stu-id="5d01d-141">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5d01d-142">**id**</span><span class="sxs-lookup"><span data-stu-id="5d01d-142">**id**</span></span>                   | <span data-ttu-id="5d01d-143">string</span><span class="sxs-lookup"><span data-stu-id="5d01d-143">string</span></span>                              | <span data-ttu-id="5d01d-p101">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d01d-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="5d01d-146">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="5d01d-146">**createdDateTime**</span></span>      | <span data-ttu-id="5d01d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d01d-147">DateTimeOffset</span></span>                      | <span data-ttu-id="5d01d-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d01d-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="5d01d-150">**description**</span><span class="sxs-lookup"><span data-stu-id="5d01d-150">**description**</span></span>          | <span data-ttu-id="5d01d-151">string</span><span class="sxs-lookup"><span data-stu-id="5d01d-151">string</span></span>                              | <span data-ttu-id="5d01d-152">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="5d01d-152">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="5d01d-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="5d01d-153">**displayName**</span></span>          | <span data-ttu-id="5d01d-154">string</span><span class="sxs-lookup"><span data-stu-id="5d01d-154">string</span></span>                              | <span data-ttu-id="5d01d-p103">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d01d-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="5d01d-157">**eTag**</span><span class="sxs-lookup"><span data-stu-id="5d01d-157">**eTag**</span></span>                 | <span data-ttu-id="5d01d-158">string</span><span class="sxs-lookup"><span data-stu-id="5d01d-158">string</span></span>                              | <span data-ttu-id="5d01d-p104">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d01d-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="5d01d-161">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="5d01d-161">**lastModifiedDateTime**</span></span> | <span data-ttu-id="5d01d-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d01d-162">DateTimeOffset</span></span>                      | <span data-ttu-id="5d01d-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d01d-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="5d01d-165">**name**</span><span class="sxs-lookup"><span data-stu-id="5d01d-165">**name**</span></span>                 | <span data-ttu-id="5d01d-166">string</span><span class="sxs-lookup"><span data-stu-id="5d01d-166">string</span></span>                              | <span data-ttu-id="5d01d-167">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="5d01d-167">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="5d01d-168">**root**</span><span class="sxs-lookup"><span data-stu-id="5d01d-168">**root**</span></span>                 | [<span data-ttu-id="5d01d-169">root</span><span class="sxs-lookup"><span data-stu-id="5d01d-169">root</span></span>](root.md)                     | <span data-ttu-id="5d01d-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d01d-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="5d01d-172">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="5d01d-172">**sharepointIds**</span></span>        | [<span data-ttu-id="5d01d-173">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="5d01d-173">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="5d01d-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d01d-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="5d01d-176">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="5d01d-176">**siteCollection**</span></span>       | [<span data-ttu-id="5d01d-177">siteCollection</span><span class="sxs-lookup"><span data-stu-id="5d01d-177">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="5d01d-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d01d-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="5d01d-181">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="5d01d-181">**webUrl**</span></span>               | <span data-ttu-id="5d01d-182">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="5d01d-182">string (url)</span></span>                        | <span data-ttu-id="5d01d-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d01d-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="5d01d-185">Связи</span><span class="sxs-lookup"><span data-stu-id="5d01d-185">Relationships</span></span>

| <span data-ttu-id="5d01d-186">Отношение</span><span class="sxs-lookup"><span data-stu-id="5d01d-186">Relationship</span></span>      | <span data-ttu-id="5d01d-187">Тип</span><span class="sxs-lookup"><span data-stu-id="5d01d-187">Type</span></span>                             | <span data-ttu-id="5d01d-188">Описание</span><span class="sxs-lookup"><span data-stu-id="5d01d-188">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="5d01d-189">**analytics**</span><span class="sxs-lookup"><span data-stu-id="5d01d-189">**analytics**</span></span>     | <span data-ttu-id="5d01d-190">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-190">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="5d01d-191">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="5d01d-191">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="5d01d-192">**columns**</span><span class="sxs-lookup"><span data-stu-id="5d01d-192">**columns**</span></span>       | <span data-ttu-id="5d01d-193">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="5d01d-193">Collection([columnDefinition][])</span></span> | <span data-ttu-id="5d01d-194">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="5d01d-194">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="5d01d-195">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="5d01d-195">**contentTypes**</span></span>  | <span data-ttu-id="5d01d-196">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="5d01d-196">Collection([contentType][])</span></span>      | <span data-ttu-id="5d01d-197">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="5d01d-197">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="5d01d-198">**drive**</span><span class="sxs-lookup"><span data-stu-id="5d01d-198">**drive**</span></span>         | <span data-ttu-id="5d01d-199">[drive][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-199">[drive][]</span></span>                        | <span data-ttu-id="5d01d-200">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="5d01d-200">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="5d01d-201">**drives**</span><span class="sxs-lookup"><span data-stu-id="5d01d-201">**drives**</span></span>        | <span data-ttu-id="5d01d-202">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="5d01d-202">Collection([drive][])</span></span>            | <span data-ttu-id="5d01d-203">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="5d01d-203">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="5d01d-204">**items**</span><span class="sxs-lookup"><span data-stu-id="5d01d-204">**items**</span></span>         | <span data-ttu-id="5d01d-205">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="5d01d-205">Collection([baseItem][])</span></span>         | <span data-ttu-id="5d01d-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="5d01d-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="5d01d-208">**lists**</span><span class="sxs-lookup"><span data-stu-id="5d01d-208">**lists**</span></span>         | <span data-ttu-id="5d01d-209">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="5d01d-209">Collection([list][])</span></span>             | <span data-ttu-id="5d01d-210">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="5d01d-210">The collection of lists under this site.</span></span>
| <span data-ttu-id="5d01d-211">**sites**</span><span class="sxs-lookup"><span data-stu-id="5d01d-211">**sites**</span></span>         | <span data-ttu-id="5d01d-212">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="5d01d-212">Collection([site][])</span></span>             | <span data-ttu-id="5d01d-213">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="5d01d-213">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="5d01d-214">**onenote**</span><span class="sxs-lookup"><span data-stu-id="5d01d-214">**onenote**</span></span>       | <span data-ttu-id="5d01d-215">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="5d01d-215">[onenote][]</span></span>                      | <span data-ttu-id="5d01d-216">Вызывает службу OneNote для выполнения операций, связанных с записными книжками.</span><span class="sxs-lookup"><span data-stu-id="5d01d-216">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="5d01d-225">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d01d-225">JSON representation</span></span>

<span data-ttu-id="5d01d-226">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d01d-226">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="5d01d-227">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="5d01d-227">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "onenote": { "@odata.type": "microsoft.graph.onenote"},

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
