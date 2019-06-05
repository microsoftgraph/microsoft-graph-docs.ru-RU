---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f2386228c3758cc15d9c270f0da32608e4f2b901
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34683505"
---
# <a name="site-resource-type"></a><span data-ttu-id="760c1-102">Тип ресурса site</span><span class="sxs-lookup"><span data-stu-id="760c1-102">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="760c1-103">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="760c1-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="760c1-104">Методы</span><span class="sxs-lookup"><span data-stu-id="760c1-104">Methods</span></span>

| <span data-ttu-id="760c1-105">Метод</span><span class="sxs-lookup"><span data-stu-id="760c1-105">Method</span></span>                         | <span data-ttu-id="760c1-106">Путь REST</span><span class="sxs-lookup"><span data-stu-id="760c1-106">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="760c1-107">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="760c1-107">[Get root site][]</span></span>              | <span data-ttu-id="760c1-108">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="760c1-108">GET /sites/root</span></span>
| <span data-ttu-id="760c1-109">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="760c1-109">[Get site][]</span></span>                   | <span data-ttu-id="760c1-110">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="760c1-110">GET /sites/{site-id}</span></span>
| <span data-ttu-id="760c1-111">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="760c1-111">[Get site by path][]</span></span>           | <span data-ttu-id="760c1-112">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="760c1-112">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="760c1-113">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="760c1-113">[Get site for a group][]</span></span>       | <span data-ttu-id="760c1-114">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="760c1-114">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="760c1-115">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="760c1-115">[Get analytics][]</span></span>              | <span data-ttu-id="760c1-116">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="760c1-116">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="760c1-117">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="760c1-117">[Get activities by interval][]</span></span> | <span data-ttu-id="760c1-118">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="760c1-118">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="760c1-119">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="760c1-119">[List pages][]</span></span>                 | <span data-ttu-id="760c1-120">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="760c1-120">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="760c1-121">[Перечисление корневых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="760c1-121">[List root sites][]</span></span>            | <span data-ttu-id="760c1-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="760c1-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="760c1-123">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="760c1-123">[Search for sites][]</span></span>           | <span data-ttu-id="760c1-124">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="760c1-124">GET /sites?search={query}</span></span>
| <span data-ttu-id="760c1-125">[Отслеживание сайта][]</span><span class="sxs-lookup"><span data-stu-id="760c1-125">[Follow Site][]</span></span>                | <span data-ttu-id="760c1-126">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="760c1-126">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="760c1-127">[Прекращение отслеживания сайта][]</span><span class="sxs-lookup"><span data-stu-id="760c1-127">[Unfollow Site][]</span></span>              | <span data-ttu-id="760c1-128">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="760c1-128">POST /users/{user-id}/followedSites/remove</span></span>

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


## <a name="properties"></a><span data-ttu-id="760c1-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="760c1-140">Properties</span></span>

| <span data-ttu-id="760c1-141">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="760c1-141">Property name</span></span>            | <span data-ttu-id="760c1-142">Тип</span><span class="sxs-lookup"><span data-stu-id="760c1-142">Type</span></span>               | <span data-ttu-id="760c1-143">Описание</span><span class="sxs-lookup"><span data-stu-id="760c1-143">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="760c1-144">**id**</span><span class="sxs-lookup"><span data-stu-id="760c1-144">**id**</span></span>                   | <span data-ttu-id="760c1-145">строка</span><span class="sxs-lookup"><span data-stu-id="760c1-145">string</span></span>             | <span data-ttu-id="760c1-146">[Уникальный идентификатор](#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="760c1-146">The unique identifier of the item.</span></span> <span data-ttu-id="760c1-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="760c1-147">Read-only.</span></span>
| <span data-ttu-id="760c1-148">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="760c1-148">**createdDateTime**</span></span>      | <span data-ttu-id="760c1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760c1-149">DateTimeOffset</span></span>     | <span data-ttu-id="760c1-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="760c1-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="760c1-152">**description**</span><span class="sxs-lookup"><span data-stu-id="760c1-152">**description**</span></span>          | <span data-ttu-id="760c1-153">string</span><span class="sxs-lookup"><span data-stu-id="760c1-153">string</span></span>             | <span data-ttu-id="760c1-154">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="760c1-154">The descriptive text for the site.</span></span>
| <span data-ttu-id="760c1-155">**eTag**</span><span class="sxs-lookup"><span data-stu-id="760c1-155">**eTag**</span></span>                 | <span data-ttu-id="760c1-156">string</span><span class="sxs-lookup"><span data-stu-id="760c1-156">string</span></span>             | <span data-ttu-id="760c1-p103">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="760c1-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="760c1-159">**displayName**</span><span class="sxs-lookup"><span data-stu-id="760c1-159">**displayName**</span></span>          | <span data-ttu-id="760c1-160">string</span><span class="sxs-lookup"><span data-stu-id="760c1-160">string</span></span>             | <span data-ttu-id="760c1-p104">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="760c1-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="760c1-163">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="760c1-163">**lastModifiedDateTime**</span></span> | <span data-ttu-id="760c1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760c1-164">DateTimeOffset</span></span>     | <span data-ttu-id="760c1-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="760c1-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="760c1-167">**name**</span><span class="sxs-lookup"><span data-stu-id="760c1-167">**name**</span></span>                 | <span data-ttu-id="760c1-168">string</span><span class="sxs-lookup"><span data-stu-id="760c1-168">string</span></span>             | <span data-ttu-id="760c1-169">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="760c1-169">The name / title of the item.</span></span>
| <span data-ttu-id="760c1-170">**root**</span><span class="sxs-lookup"><span data-stu-id="760c1-170">**root**</span></span>                 | <span data-ttu-id="760c1-171">[root][]</span><span class="sxs-lookup"><span data-stu-id="760c1-171">[root][]</span></span>           | <span data-ttu-id="760c1-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="760c1-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="760c1-174">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="760c1-174">**sharepointIds**</span></span>        | <span data-ttu-id="760c1-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="760c1-175">[sharepointIds][]</span></span>  | <span data-ttu-id="760c1-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="760c1-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="760c1-178">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="760c1-178">**siteCollection**</span></span>       | <span data-ttu-id="760c1-179">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="760c1-179">[siteCollection][]</span></span> | <span data-ttu-id="760c1-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="760c1-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="760c1-183">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="760c1-183">**webUrl**</span></span>               | <span data-ttu-id="760c1-184">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="760c1-184">string (url)</span></span>       | <span data-ttu-id="760c1-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="760c1-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="760c1-187">Свойство id</span><span class="sxs-lookup"><span data-stu-id="760c1-187">id property</span></span>
<span data-ttu-id="760c1-188">Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="760c1-188">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>
* <span data-ttu-id="760c1-189">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="760c1-189">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="760c1-190">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="760c1-190">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="760c1-191">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="760c1-191">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="760c1-192">Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="760c1-192">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="760c1-193">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="760c1-193">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="760c1-194">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="760c1-194">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="760c1-195">Связи</span><span class="sxs-lookup"><span data-stu-id="760c1-195">Relationships</span></span>

| <span data-ttu-id="760c1-196">Имя связи</span><span class="sxs-lookup"><span data-stu-id="760c1-196">Relationship name</span></span> | <span data-ttu-id="760c1-197">Тип</span><span class="sxs-lookup"><span data-stu-id="760c1-197">Type</span></span>                             | <span data-ttu-id="760c1-198">Описание</span><span class="sxs-lookup"><span data-stu-id="760c1-198">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="760c1-199">**analytics**</span><span class="sxs-lookup"><span data-stu-id="760c1-199">**analytics**</span></span>     | <span data-ttu-id="760c1-200">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="760c1-200">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="760c1-201">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="760c1-201">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="760c1-202">**columns**</span><span class="sxs-lookup"><span data-stu-id="760c1-202">**columns**</span></span>       | <span data-ttu-id="760c1-203">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="760c1-203">Collection([columnDefinition][])</span></span> | <span data-ttu-id="760c1-204">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="760c1-204">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="760c1-205">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="760c1-205">**contentTypes**</span></span>  | <span data-ttu-id="760c1-206">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="760c1-206">Collection([contentType][])</span></span>      | <span data-ttu-id="760c1-207">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="760c1-207">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="760c1-208">**drive**</span><span class="sxs-lookup"><span data-stu-id="760c1-208">**drive**</span></span>         | <span data-ttu-id="760c1-209">[drive][]</span><span class="sxs-lookup"><span data-stu-id="760c1-209">[drive][]</span></span>                        | <span data-ttu-id="760c1-210">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="760c1-210">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="760c1-211">**drives**</span><span class="sxs-lookup"><span data-stu-id="760c1-211">**drives**</span></span>        | <span data-ttu-id="760c1-212">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="760c1-212">Collection([drive][])</span></span>            | <span data-ttu-id="760c1-213">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="760c1-213">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="760c1-214">**items**</span><span class="sxs-lookup"><span data-stu-id="760c1-214">**items**</span></span>         | <span data-ttu-id="760c1-215">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="760c1-215">Collection([baseItem][])</span></span>         | <span data-ttu-id="760c1-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="760c1-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="760c1-218">**lists**</span><span class="sxs-lookup"><span data-stu-id="760c1-218">**lists**</span></span>         | <span data-ttu-id="760c1-219">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="760c1-219">Collection([list][])</span></span>             | <span data-ttu-id="760c1-220">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="760c1-220">The collection of lists under this site.</span></span>
| <span data-ttu-id="760c1-221">**pages**</span><span class="sxs-lookup"><span data-stu-id="760c1-221">**pages**</span></span>         | <span data-ttu-id="760c1-222">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="760c1-222">Collection([sitePage][])</span></span>         | <span data-ttu-id="760c1-223">Коллекция страниц в списке SitePages на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="760c1-223">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="760c1-224">**sites**</span><span class="sxs-lookup"><span data-stu-id="760c1-224">**sites**</span></span>         | <span data-ttu-id="760c1-225">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="760c1-225">Collection([site][])</span></span>             | <span data-ttu-id="760c1-226">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="760c1-226">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="760c1-238">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="760c1-238">JSON representation</span></span>

<span data-ttu-id="760c1-239">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="760c1-239">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="760c1-240">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="760c1-240">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
