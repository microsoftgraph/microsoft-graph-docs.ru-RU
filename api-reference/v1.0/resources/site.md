---
author: JeremyKelley
ms.author: JeremyKelley
title: Ресурс site
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1878b46f7738f440808960e43310b2d7606ee22f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533694"
---
# <a name="site-resource"></a><span data-ttu-id="d2194-103">Ресурс site</span><span class="sxs-lookup"><span data-stu-id="d2194-103">site resource</span></span>

<span data-ttu-id="d2194-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2194-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2194-105">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d2194-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="d2194-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d2194-106">Methods</span></span>

| <span data-ttu-id="d2194-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d2194-107">Method</span></span>                | <span data-ttu-id="d2194-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="d2194-108">Return type</span></span> | <span data-ttu-id="d2194-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d2194-109">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="d2194-110">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="d2194-110">[Get root site][]</span></span>        | <span data-ttu-id="d2194-111">site</span><span class="sxs-lookup"><span data-stu-id="d2194-111">site</span></span> | <span data-ttu-id="d2194-112">Получение доступа к корневому сайту SharePoint внутри клиента.</span><span class="sxs-lookup"><span data-stu-id="d2194-112">Access the root SharePoint site within a tenant.</span></span>
| <span data-ttu-id="d2194-113">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="d2194-113">[Get site][]</span></span>             | <span data-ttu-id="d2194-114">site</span><span class="sxs-lookup"><span data-stu-id="d2194-114">site</span></span> | <span data-ttu-id="d2194-115">Получение доступа к сайту SharePoint с помощью параметра siteId.</span><span class="sxs-lookup"><span data-stu-id="d2194-115">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="d2194-116">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="d2194-116">[Get site by path][]</span></span>     | <span data-ttu-id="d2194-117">site</span><span class="sxs-lookup"><span data-stu-id="d2194-117">site</span></span> | <span data-ttu-id="d2194-118">Получение доступа к корневому сайту SharePoint с использованием относительного пути.</span><span class="sxs-lookup"><span data-stu-id="d2194-118">Access the root SharePoint site with a relative path.</span></span>
| <span data-ttu-id="d2194-119">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="d2194-119">[Get site for a group][]</span></span> | <span data-ttu-id="d2194-120">site</span><span class="sxs-lookup"><span data-stu-id="d2194-120">site</span></span> | <span data-ttu-id="d2194-121">Получение доступа к сайту группы для группы.</span><span class="sxs-lookup"><span data-stu-id="d2194-121">Access the team site for a group.</span></span>
| <span data-ttu-id="d2194-122">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="d2194-122">[Get analytics][]</span></span>              | <span data-ttu-id="d2194-123">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="d2194-123">[itemAnalytics][]</span></span> | <span data-ttu-id="d2194-124">Получение аналитических данных для ресурса.</span><span class="sxs-lookup"><span data-stu-id="d2194-124">Get analytics for this resource.</span></span> 
| <span data-ttu-id="d2194-125">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="d2194-125">[Get activities by interval][]</span></span> | <span data-ttu-id="d2194-126">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="d2194-126">[itemActivityStat][]</span></span> | <span data-ttu-id="d2194-127">Получение коллекции объектов **itemActivityStats** в пределах указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="d2194-127">Get a collection of **itemActivityStats** within the specified time interval.</span></span>
| <span data-ttu-id="d2194-128">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="d2194-128">[Search for sites][]</span></span>     | <span data-ttu-id="d2194-129">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="d2194-129">collection of site</span></span> | <span data-ttu-id="d2194-130">Поиск сайтов, соответствующих указанным ключевым словам, в клиенте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d2194-130">Search across a SharePoint tenant for sites that match keywords provided.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d2194-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2194-139">Properties</span></span>

| <span data-ttu-id="d2194-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2194-140">Property</span></span>            | <span data-ttu-id="d2194-141">Тип</span><span class="sxs-lookup"><span data-stu-id="d2194-141">Type</span></span>                                | <span data-ttu-id="d2194-142">Описание</span><span class="sxs-lookup"><span data-stu-id="d2194-142">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d2194-143">**id**</span><span class="sxs-lookup"><span data-stu-id="d2194-143">**id**</span></span>                   | <span data-ttu-id="d2194-144">string</span><span class="sxs-lookup"><span data-stu-id="d2194-144">string</span></span>                              | <span data-ttu-id="d2194-p101">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2194-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="d2194-147">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="d2194-147">**createdDateTime**</span></span>      | <span data-ttu-id="d2194-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2194-148">DateTimeOffset</span></span>                      | <span data-ttu-id="d2194-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2194-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="d2194-151">**description**</span><span class="sxs-lookup"><span data-stu-id="d2194-151">**description**</span></span>          | <span data-ttu-id="d2194-152">string</span><span class="sxs-lookup"><span data-stu-id="d2194-152">string</span></span>                              | <span data-ttu-id="d2194-153">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="d2194-153">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="d2194-154">**displayName**</span><span class="sxs-lookup"><span data-stu-id="d2194-154">**displayName**</span></span>          | <span data-ttu-id="d2194-155">string</span><span class="sxs-lookup"><span data-stu-id="d2194-155">string</span></span>                              | <span data-ttu-id="d2194-p103">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2194-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="d2194-158">**eTag**</span><span class="sxs-lookup"><span data-stu-id="d2194-158">**eTag**</span></span>                 | <span data-ttu-id="d2194-159">string</span><span class="sxs-lookup"><span data-stu-id="d2194-159">string</span></span>                              | <span data-ttu-id="d2194-p104">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2194-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="d2194-162">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="d2194-162">**lastModifiedDateTime**</span></span> | <span data-ttu-id="d2194-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2194-163">DateTimeOffset</span></span>                      | <span data-ttu-id="d2194-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2194-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="d2194-166">**name**</span><span class="sxs-lookup"><span data-stu-id="d2194-166">**name**</span></span>                 | <span data-ttu-id="d2194-167">string</span><span class="sxs-lookup"><span data-stu-id="d2194-167">string</span></span>                              | <span data-ttu-id="d2194-168">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="d2194-168">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="d2194-169">**root**</span><span class="sxs-lookup"><span data-stu-id="d2194-169">**root**</span></span>                 | [<span data-ttu-id="d2194-170">root</span><span class="sxs-lookup"><span data-stu-id="d2194-170">root</span></span>](root.md)                     | <span data-ttu-id="d2194-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2194-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="d2194-173">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="d2194-173">**sharepointIds**</span></span>        | [<span data-ttu-id="d2194-174">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="d2194-174">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="d2194-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2194-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="d2194-177">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="d2194-177">**siteCollection**</span></span>       | [<span data-ttu-id="d2194-178">siteCollection</span><span class="sxs-lookup"><span data-stu-id="d2194-178">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="d2194-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2194-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="d2194-182">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="d2194-182">**webUrl**</span></span>               | <span data-ttu-id="d2194-183">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="d2194-183">string (url)</span></span>                        | <span data-ttu-id="d2194-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2194-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="d2194-186">Связи</span><span class="sxs-lookup"><span data-stu-id="d2194-186">Relationships</span></span>

| <span data-ttu-id="d2194-187">Связь</span><span class="sxs-lookup"><span data-stu-id="d2194-187">Relationship</span></span>      | <span data-ttu-id="d2194-188">Тип</span><span class="sxs-lookup"><span data-stu-id="d2194-188">Type</span></span>                             | <span data-ttu-id="d2194-189">Описание</span><span class="sxs-lookup"><span data-stu-id="d2194-189">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="d2194-190">**analytics**</span><span class="sxs-lookup"><span data-stu-id="d2194-190">**analytics**</span></span>     | <span data-ttu-id="d2194-191">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="d2194-191">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="d2194-192">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="d2194-192">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="d2194-193">**columns**</span><span class="sxs-lookup"><span data-stu-id="d2194-193">**columns**</span></span>       | <span data-ttu-id="d2194-194">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="d2194-194">Collection([columnDefinition][])</span></span> | <span data-ttu-id="d2194-195">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="d2194-195">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="d2194-196">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="d2194-196">**contentTypes**</span></span>  | <span data-ttu-id="d2194-197">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="d2194-197">Collection([contentType][])</span></span>      | <span data-ttu-id="d2194-198">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="d2194-198">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="d2194-199">**drive**</span><span class="sxs-lookup"><span data-stu-id="d2194-199">**drive**</span></span>         | <span data-ttu-id="d2194-200">[drive][]</span><span class="sxs-lookup"><span data-stu-id="d2194-200">[drive][]</span></span>                        | <span data-ttu-id="d2194-201">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="d2194-201">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="d2194-202">**drives**</span><span class="sxs-lookup"><span data-stu-id="d2194-202">**drives**</span></span>        | <span data-ttu-id="d2194-203">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="d2194-203">Collection([drive][])</span></span>            | <span data-ttu-id="d2194-204">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="d2194-204">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="d2194-205">**items**</span><span class="sxs-lookup"><span data-stu-id="d2194-205">**items**</span></span>         | <span data-ttu-id="d2194-206">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="d2194-206">Collection([baseItem][])</span></span>         | <span data-ttu-id="d2194-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="d2194-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="d2194-209">**lists**</span><span class="sxs-lookup"><span data-stu-id="d2194-209">**lists**</span></span>         | <span data-ttu-id="d2194-210">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="d2194-210">Collection([list][])</span></span>             | <span data-ttu-id="d2194-211">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="d2194-211">The collection of lists under this site.</span></span>
| <span data-ttu-id="d2194-212">**sites**</span><span class="sxs-lookup"><span data-stu-id="d2194-212">**sites**</span></span>         | <span data-ttu-id="d2194-213">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="d2194-213">Collection([site][])</span></span>             | <span data-ttu-id="d2194-214">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="d2194-214">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="d2194-215">**onenote**</span><span class="sxs-lookup"><span data-stu-id="d2194-215">**onenote**</span></span>       | <span data-ttu-id="d2194-216">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="d2194-216">[onenote][]</span></span>                      | <span data-ttu-id="d2194-217">Вызывает службу OneNote для выполнения операций, связанных с записными книжками.</span><span class="sxs-lookup"><span data-stu-id="d2194-217">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="d2194-226">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2194-226">JSON representation</span></span>

<span data-ttu-id="d2194-227">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2194-227">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="d2194-228">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="d2194-228">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
