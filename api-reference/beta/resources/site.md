---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 1676a314b7c1283918518655b3180cbc70ca193e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952351"
---
# <a name="site-resource-type"></a><span data-ttu-id="f2859-102">Тип ресурса сайта</span><span class="sxs-lookup"><span data-stu-id="f2859-102">site resource type</span></span>

> <span data-ttu-id="f2859-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2859-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2859-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2859-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2859-105">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f2859-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="f2859-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f2859-106">Methods</span></span>

| <span data-ttu-id="f2859-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f2859-107">Method</span></span>                         | <span data-ttu-id="f2859-108">Путь REST</span><span class="sxs-lookup"><span data-stu-id="f2859-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="f2859-109">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="f2859-109">[Get root site][]</span></span>              | <span data-ttu-id="f2859-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="f2859-110">GET /sites/root</span></span>
| <span data-ttu-id="f2859-111">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="f2859-111">[Get site][]</span></span>                   | <span data-ttu-id="f2859-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="f2859-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="f2859-113">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="f2859-113">[Get site by path][]</span></span>           | <span data-ttu-id="f2859-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="f2859-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="f2859-115">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="f2859-115">[Get site for a group][]</span></span>       | <span data-ttu-id="f2859-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="f2859-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="f2859-117">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="f2859-117">[Get analytics][]</span></span>              | <span data-ttu-id="f2859-118">GET/Sites / {идентификатор сайта} / аналитики</span><span class="sxs-lookup"><span data-stu-id="f2859-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="f2859-119">[Получение действий по интервал][]</span><span class="sxs-lookup"><span data-stu-id="f2859-119">[Get activities by interval][]</span></span> | <span data-ttu-id="f2859-120">GET/Sites / {идентификатор сайта} / getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="f2859-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="f2859-121">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="f2859-121">[List pages][]</span></span>                 | <span data-ttu-id="f2859-122">GET/Sites / {идентификатор сайта} / pages</span><span class="sxs-lookup"><span data-stu-id="f2859-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="f2859-123">[Узлы корневого списка][]</span><span class="sxs-lookup"><span data-stu-id="f2859-123">[List root sites][]</span></span>            | <span data-ttu-id="f2859-124">/ Sites GET? фильтра = ne корневой значение null и выделить = siteCollection, webUrl</span><span class="sxs-lookup"><span data-stu-id="f2859-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="f2859-125">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="f2859-125">[Search for sites][]</span></span>           | <span data-ttu-id="f2859-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="f2859-126">GET /sites?search={query}</span></span>

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
[Получение действий по интервал]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Перечисление страниц]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Узлы корневого списка]: ../api/site-list.md
[List root sites]: ../api/site-list.md
[Поиск сайтов]: ../api/site-search.md
[Search for sites]: ../api/site-search.md


## <a name="properties"></a><span data-ttu-id="f2859-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2859-136">Properties</span></span>

| <span data-ttu-id="f2859-137">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f2859-137">Property name</span></span>            | <span data-ttu-id="f2859-138">Тип</span><span class="sxs-lookup"><span data-stu-id="f2859-138">Type</span></span>               | <span data-ttu-id="f2859-139">Описание</span><span class="sxs-lookup"><span data-stu-id="f2859-139">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="f2859-140">**id**</span><span class="sxs-lookup"><span data-stu-id="f2859-140">**id**</span></span>                   | <span data-ttu-id="f2859-141">строка</span><span class="sxs-lookup"><span data-stu-id="f2859-141">string</span></span>             | <span data-ttu-id="f2859-p102">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2859-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="f2859-144">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="f2859-144">**createdDateTime**</span></span>      | <span data-ttu-id="f2859-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2859-145">DateTimeOffset</span></span>     | <span data-ttu-id="f2859-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2859-p103">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="f2859-148">**description**</span><span class="sxs-lookup"><span data-stu-id="f2859-148">**description**</span></span>          | <span data-ttu-id="f2859-149">строка</span><span class="sxs-lookup"><span data-stu-id="f2859-149">string</span></span>             | <span data-ttu-id="f2859-150">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="f2859-150">The descriptive text for the site.</span></span>
| <span data-ttu-id="f2859-151">**eTag**;</span><span class="sxs-lookup"><span data-stu-id="f2859-151">**eTag**</span></span>                 | <span data-ttu-id="f2859-152">string</span><span class="sxs-lookup"><span data-stu-id="f2859-152">string</span></span>             | <span data-ttu-id="f2859-p104">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2859-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="f2859-155">**displayName**</span><span class="sxs-lookup"><span data-stu-id="f2859-155">**displayName**</span></span>          | <span data-ttu-id="f2859-156">строка</span><span class="sxs-lookup"><span data-stu-id="f2859-156">string</span></span>             | <span data-ttu-id="f2859-p105">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2859-p105">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="f2859-159">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f2859-159">**lastModifiedDateTime**</span></span> | <span data-ttu-id="f2859-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2859-160">DateTimeOffset</span></span>     | <span data-ttu-id="f2859-p106">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2859-p106">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f2859-163">**name**</span><span class="sxs-lookup"><span data-stu-id="f2859-163">**name**</span></span>                 | <span data-ttu-id="f2859-164">строка</span><span class="sxs-lookup"><span data-stu-id="f2859-164">string</span></span>             | <span data-ttu-id="f2859-165">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="f2859-165">The name / title of the item.</span></span>
| <span data-ttu-id="f2859-166">**root**</span><span class="sxs-lookup"><span data-stu-id="f2859-166">**root**</span></span>                 | <span data-ttu-id="f2859-167">[root][]</span><span class="sxs-lookup"><span data-stu-id="f2859-167">[root][]</span></span>           | <span data-ttu-id="f2859-p107">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2859-p107">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="f2859-170">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="f2859-170">**sharepointIds**</span></span>        | <span data-ttu-id="f2859-171">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f2859-171">[sharepointIds][]</span></span>  | <span data-ttu-id="f2859-p108">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2859-p108">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="f2859-174">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="f2859-174">**siteCollection**</span></span>       | <span data-ttu-id="f2859-175">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="f2859-175">[siteCollection][]</span></span> | <span data-ttu-id="f2859-p109">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2859-p109">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="f2859-179">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="f2859-179">**webUrl**</span></span>               | <span data-ttu-id="f2859-180">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="f2859-180">string (url)</span></span>       | <span data-ttu-id="f2859-p110">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2859-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="f2859-183">Связи</span><span class="sxs-lookup"><span data-stu-id="f2859-183">Relationships</span></span>

| <span data-ttu-id="f2859-184">Имя связи</span><span class="sxs-lookup"><span data-stu-id="f2859-184">Relationship name</span></span> | <span data-ttu-id="f2859-185">Тип</span><span class="sxs-lookup"><span data-stu-id="f2859-185">Type</span></span>                             | <span data-ttu-id="f2859-186">Описание</span><span class="sxs-lookup"><span data-stu-id="f2859-186">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="f2859-187">**Аналитика**</span><span class="sxs-lookup"><span data-stu-id="f2859-187">**analytics**</span></span>     | <span data-ttu-id="f2859-188">[itemAnalytics][] ресурсов</span><span class="sxs-lookup"><span data-stu-id="f2859-188">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="f2859-189">Аналитика о Просмотр действий, выполняемых на данном сайте.</span><span class="sxs-lookup"><span data-stu-id="f2859-189">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="f2859-190">**columns**</span><span class="sxs-lookup"><span data-stu-id="f2859-190">**columns**</span></span>       | <span data-ttu-id="f2859-191">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="f2859-191">Collection([columnDefinition][])</span></span> | <span data-ttu-id="f2859-192">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f2859-192">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="f2859-193">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="f2859-193">**contentTypes**</span></span>  | <span data-ttu-id="f2859-194">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="f2859-194">Collection([contentType][])</span></span>      | <span data-ttu-id="f2859-195">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="f2859-195">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="f2859-196">**drive**</span><span class="sxs-lookup"><span data-stu-id="f2859-196">**drive**</span></span>         | <span data-ttu-id="f2859-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="f2859-197">[drive][]</span></span>                        | <span data-ttu-id="f2859-198">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="f2859-198">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="f2859-199">**drives**</span><span class="sxs-lookup"><span data-stu-id="f2859-199">**drives**</span></span>        | <span data-ttu-id="f2859-200">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="f2859-200">Collection([drive][])</span></span>            | <span data-ttu-id="f2859-201">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f2859-201">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="f2859-202">**items**</span><span class="sxs-lookup"><span data-stu-id="f2859-202">**items**</span></span>         | <span data-ttu-id="f2859-203">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="f2859-203">Collection([baseItem][])</span></span>         | <span data-ttu-id="f2859-p111">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="f2859-p111">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="f2859-206">**lists**</span><span class="sxs-lookup"><span data-stu-id="f2859-206">**lists**</span></span>         | <span data-ttu-id="f2859-207">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="f2859-207">Collection([list][])</span></span>             | <span data-ttu-id="f2859-208">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f2859-208">The collection of lists under this site.</span></span>
| <span data-ttu-id="f2859-209">**страницы**</span><span class="sxs-lookup"><span data-stu-id="f2859-209">**pages**</span></span>         | <span data-ttu-id="f2859-210">Коллекции ([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="f2859-210">Collection([sitePage][])</span></span>         | <span data-ttu-id="f2859-211">Набор страниц в списке SitePages на данном сайте.</span><span class="sxs-lookup"><span data-stu-id="f2859-211">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="f2859-212">**sites**</span><span class="sxs-lookup"><span data-stu-id="f2859-212">**sites**</span></span>         | <span data-ttu-id="f2859-213">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="f2859-213">Collection([site][])</span></span>             | <span data-ttu-id="f2859-214">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="f2859-214">The collection of the sub-sites under this site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[списки]: list.md
[list]: list.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="f2859-226">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2859-226">JSON representation</span></span>

<span data-ttu-id="f2859-227">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2859-227">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="f2859-228">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="f2859-228">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
