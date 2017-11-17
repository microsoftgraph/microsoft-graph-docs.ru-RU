---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: site
ms.openlocfilehash: db465f93f336a51d862daf6e05b1d6bc422247ea
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="site-resource"></a><span data-ttu-id="47906-102">Ресурс site</span><span class="sxs-lookup"><span data-stu-id="47906-102">Site resource</span></span>

<span data-ttu-id="47906-103">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="47906-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="47906-104">Задачи</span><span class="sxs-lookup"><span data-stu-id="47906-104">Tasks</span></span>

<span data-ttu-id="47906-105">Все приведенные ниже примеры относятся к `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="47906-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="47906-106">Имя задачи</span><span class="sxs-lookup"><span data-stu-id="47906-106">Task name</span></span>                | <span data-ttu-id="47906-107">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="47906-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="47906-108">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="47906-108">[Get root site][]</span></span>        | <span data-ttu-id="47906-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="47906-109">GET /sites/root</span></span>
| <span data-ttu-id="47906-110">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="47906-110">[Get site][]</span></span>             | <span data-ttu-id="47906-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="47906-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="47906-112">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="47906-112">[Get site by path][]</span></span>     | <span data-ttu-id="47906-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="47906-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="47906-114">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="47906-114">[Get site for a group][]</span></span> | <span data-ttu-id="47906-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="47906-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="47906-116">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="47906-116">[Search for sites][]</span></span>     | <span data-ttu-id="47906-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="47906-117">GET /sites?search={query}</span></span>

[Получение сайта]: ../api/site_get.md
[Получение корневого сайта]: ../api/site_get.md
[Получение сайта по пути]: ../api/site_getbypath.md
[Получение сайта для группы]: ../api/site_get.md
[Поиск сайтов]: ../api/site_search.md

## <a name="json-representation"></a><span data-ttu-id="47906-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47906-123">JSON representation</span></span>

<span data-ttu-id="47906-124">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47906-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="47906-125">Ресурс **driveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="47906-125">The **driveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource",
       "@odata.type": "microsoft.graph.site",
       "keyProperty": "id",
       "optionalProperties": [ "root", "sharepointIds", "siteCollection", "drive", "drives", "sites" ] } -->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "onenote": [ { "@odata.type": "microsoft.graph.onenote"} ],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="47906-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="47906-126">Properties</span></span>

| <span data-ttu-id="47906-127">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="47906-127">Property name</span></span>            | <span data-ttu-id="47906-128">Тип</span><span class="sxs-lookup"><span data-stu-id="47906-128">Type</span></span>                                | <span data-ttu-id="47906-129">Описание</span><span class="sxs-lookup"><span data-stu-id="47906-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="47906-130">**id**</span><span class="sxs-lookup"><span data-stu-id="47906-130">**id**</span></span>                   | <span data-ttu-id="47906-131">string</span><span class="sxs-lookup"><span data-stu-id="47906-131">string</span></span>                              | <span data-ttu-id="47906-p101">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47906-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="47906-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="47906-134">**createdDateTime**</span></span>      | <span data-ttu-id="47906-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47906-135">DateTimeOffset</span></span>                      | <span data-ttu-id="47906-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47906-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="47906-138">**description**</span><span class="sxs-lookup"><span data-stu-id="47906-138">**description**</span></span>          | <span data-ttu-id="47906-139">string</span><span class="sxs-lookup"><span data-stu-id="47906-139">string</span></span>                              | <span data-ttu-id="47906-140">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="47906-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="47906-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="47906-141">**displayName**</span></span>          | <span data-ttu-id="47906-142">string</span><span class="sxs-lookup"><span data-stu-id="47906-142">string</span></span>                              | <span data-ttu-id="47906-p103">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47906-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="47906-145">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="47906-145">**lastModifiedDateTime**</span></span> | <span data-ttu-id="47906-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47906-146">DateTimeOffset</span></span>                      | <span data-ttu-id="47906-p104">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47906-p104">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="47906-149">**name**</span><span class="sxs-lookup"><span data-stu-id="47906-149">**name**</span></span>                 | <span data-ttu-id="47906-150">string</span><span class="sxs-lookup"><span data-stu-id="47906-150">string</span></span>                              | <span data-ttu-id="47906-151">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="47906-151">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="47906-152">**root**</span><span class="sxs-lookup"><span data-stu-id="47906-152">**root**</span></span>                 | [<span data-ttu-id="47906-153">root</span><span class="sxs-lookup"><span data-stu-id="47906-153">root</span></span>](root.md)                     | <span data-ttu-id="47906-p105">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47906-p105">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="47906-156">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="47906-156">**sharepointIds**</span></span>        | [<span data-ttu-id="47906-157">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="47906-157">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="47906-p106">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47906-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="47906-160">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="47906-160">**siteCollection**</span></span>       | [<span data-ttu-id="47906-161">siteCollection</span><span class="sxs-lookup"><span data-stu-id="47906-161">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="47906-p107">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47906-p107">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="47906-165">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="47906-165">**webUrl**</span></span>               | <span data-ttu-id="47906-166">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="47906-166">string (url)</span></span>                        | <span data-ttu-id="47906-p108">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47906-p108">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="47906-169">Связи</span><span class="sxs-lookup"><span data-stu-id="47906-169">Relationships</span></span>

| <span data-ttu-id="47906-170">Имя связи</span><span class="sxs-lookup"><span data-stu-id="47906-170">Relationship name</span></span> | <span data-ttu-id="47906-171">Тип</span><span class="sxs-lookup"><span data-stu-id="47906-171">Type</span></span>                             | <span data-ttu-id="47906-172">Описание</span><span class="sxs-lookup"><span data-stu-id="47906-172">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="47906-173">**columns**</span><span class="sxs-lookup"><span data-stu-id="47906-173">**columns**</span></span>       | <span data-ttu-id="47906-174">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="47906-174">Collection([columnDefinition][])</span></span> | <span data-ttu-id="47906-175">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="47906-175">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="47906-176">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="47906-176"><ContentTypes></span></span>  | <span data-ttu-id="47906-177">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="47906-177">Collection([contentType][])</span></span>      | <span data-ttu-id="47906-178">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="47906-178">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="47906-179">**drive**</span><span class="sxs-lookup"><span data-stu-id="47906-179">**drive**</span></span>         | <span data-ttu-id="47906-180">[drive][]</span><span class="sxs-lookup"><span data-stu-id="47906-180">[drive][]</span></span>                        | <span data-ttu-id="47906-181">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="47906-181">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="47906-182">**drives**</span><span class="sxs-lookup"><span data-stu-id="47906-182">**drives**</span></span>        | <span data-ttu-id="47906-183">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="47906-183">Collection([drive][])</span></span>            | <span data-ttu-id="47906-184">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="47906-184">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="47906-185">**items**</span><span class="sxs-lookup"><span data-stu-id="47906-185">**items**</span></span>         | <span data-ttu-id="47906-186">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="47906-186">Collection([baseItem][])</span></span>         | <span data-ttu-id="47906-p109">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="47906-p109">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="47906-189">**lists**</span><span class="sxs-lookup"><span data-stu-id="47906-189">**Lists**</span></span>         | <span data-ttu-id="47906-190">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="47906-190">Collection([list][])</span></span>             | <span data-ttu-id="47906-191">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="47906-191">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="47906-192">**sites**</span><span class="sxs-lookup"><span data-stu-id="47906-192">**sites**</span></span>         | <span data-ttu-id="47906-193">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="47906-193">Collection([site][])</span></span>             | <span data-ttu-id="47906-194">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="47906-194">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="47906-195">**onenote**</span><span class="sxs-lookup"><span data-stu-id="47906-195">**onenote**</span></span>       | <span data-ttu-id="47906-196">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="47906-196">[onenote][]</span></span>                      | <span data-ttu-id="47906-197">Вызывает службу OneNote для выполнения операций, связанных с записными книжками.</span><span class="sxs-lookup"><span data-stu-id="47906-197">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contentType.md
[drive]: drive.md
[identitySet]: identityset.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
