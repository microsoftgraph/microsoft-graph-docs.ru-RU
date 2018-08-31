---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: site
ms.openlocfilehash: 20d31a9cdc0e540c2b2f2d93fedabdc254e9c03e
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265717"
---
# <a name="site-resource"></a><span data-ttu-id="cffb5-102">Ресурс site</span><span class="sxs-lookup"><span data-stu-id="cffb5-102">Site resource</span></span>

<span data-ttu-id="cffb5-103">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cffb5-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="cffb5-104">Задачи</span><span class="sxs-lookup"><span data-stu-id="cffb5-104">Tasks</span></span>

<span data-ttu-id="cffb5-105">Все приведенные ниже примеры относятся к `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="cffb5-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="cffb5-106">Имя задачи</span><span class="sxs-lookup"><span data-stu-id="cffb5-106">Task name</span></span>                | <span data-ttu-id="cffb5-107">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="cffb5-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="cffb5-108">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="cffb5-108">[Get root site][]</span></span>        | <span data-ttu-id="cffb5-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="cffb5-109">GET /sites/root</span></span>
| <span data-ttu-id="cffb5-110">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="cffb5-110">[Get site][]</span></span>             | <span data-ttu-id="cffb5-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="cffb5-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="cffb5-112">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="cffb5-112">[Get site by path][]</span></span>     | <span data-ttu-id="cffb5-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="cffb5-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="cffb5-114">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="cffb5-114">[Get site for a group][]</span></span> | <span data-ttu-id="cffb5-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="cffb5-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="cffb5-116">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="cffb5-116">[Search for sites][]</span></span>     | <span data-ttu-id="cffb5-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="cffb5-117">GET /sites?search={query}</span></span>

[Получение сайта]: ../api/site_get.md
[Get site]: ../api/site_get.md
[Получение корневого сайта]: ../api/site_get.md
[Get root site]: ../api/site_get.md
[Получение сайта по пути]: ../api/site_getbypath.md
[Get site by path]: ../api/site_getbypath.md
[Получение сайта для группы]: ../api/site_get.md
[Get site for a group]: ../api/site_get.md
[Поиск сайтов]: ../api/site_search.md
[Search for sites]: ../api/site_search.md

## <a name="json-representation"></a><span data-ttu-id="cffb5-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cffb5-123">JSON representation</span></span>

<span data-ttu-id="cffb5-124">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cffb5-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="cffb5-125">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="cffb5-125">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="cffb5-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="cffb5-126">Properties</span></span>

| <span data-ttu-id="cffb5-127">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="cffb5-127">Property name</span></span>            | <span data-ttu-id="cffb5-128">Тип</span><span class="sxs-lookup"><span data-stu-id="cffb5-128">Type</span></span>                                | <span data-ttu-id="cffb5-129">Описание</span><span class="sxs-lookup"><span data-stu-id="cffb5-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="cffb5-130">**id**</span><span class="sxs-lookup"><span data-stu-id="cffb5-130">**id**</span></span>                   | <span data-ttu-id="cffb5-131">string</span><span class="sxs-lookup"><span data-stu-id="cffb5-131">string</span></span>                              | <span data-ttu-id="cffb5-p101">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cffb5-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="cffb5-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="cffb5-134">**createdDateTime**</span></span>      | <span data-ttu-id="cffb5-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cffb5-135">DateTimeOffset</span></span>                      | <span data-ttu-id="cffb5-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cffb5-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="cffb5-138">**description**</span><span class="sxs-lookup"><span data-stu-id="cffb5-138">**description**</span></span>          | <span data-ttu-id="cffb5-139">string</span><span class="sxs-lookup"><span data-stu-id="cffb5-139">string</span></span>                              | <span data-ttu-id="cffb5-140">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="cffb5-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="cffb5-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="cffb5-141">**displayName**</span></span>          | <span data-ttu-id="cffb5-142">string</span><span class="sxs-lookup"><span data-stu-id="cffb5-142">string</span></span>                              | <span data-ttu-id="cffb5-p103">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cffb5-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="cffb5-145">**eTag**</span><span class="sxs-lookup"><span data-stu-id="cffb5-145">**eTag**</span></span>                 | <span data-ttu-id="cffb5-146">string</span><span class="sxs-lookup"><span data-stu-id="cffb5-146">string</span></span>                              | <span data-ttu-id="cffb5-p104">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cffb5-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="cffb5-149">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="cffb5-149">**lastModifiedDateTime**</span></span> | <span data-ttu-id="cffb5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cffb5-150">DateTimeOffset</span></span>                      | <span data-ttu-id="cffb5-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cffb5-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="cffb5-153">**name**</span><span class="sxs-lookup"><span data-stu-id="cffb5-153">**name**</span></span>                 | <span data-ttu-id="cffb5-154">string</span><span class="sxs-lookup"><span data-stu-id="cffb5-154">string</span></span>                              | <span data-ttu-id="cffb5-155">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="cffb5-155">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="cffb5-156">**root**</span><span class="sxs-lookup"><span data-stu-id="cffb5-156">**root**</span></span>                 | [<span data-ttu-id="cffb5-157">root</span><span class="sxs-lookup"><span data-stu-id="cffb5-157">root</span></span>](root.md)                     | <span data-ttu-id="cffb5-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cffb5-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="cffb5-160">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="cffb5-160">**sharepointIds**</span></span>        | [<span data-ttu-id="cffb5-161">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="cffb5-161">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="cffb5-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cffb5-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="cffb5-164">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="cffb5-164">**siteCollection**</span></span>       | [<span data-ttu-id="cffb5-165">siteCollection</span><span class="sxs-lookup"><span data-stu-id="cffb5-165">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="cffb5-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cffb5-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="cffb5-169">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="cffb5-169">**webUrl**</span></span>               | <span data-ttu-id="cffb5-170">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="cffb5-170">string (url)</span></span>                        | <span data-ttu-id="cffb5-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cffb5-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="cffb5-173">Связи</span><span class="sxs-lookup"><span data-stu-id="cffb5-173">Relationships</span></span>

| <span data-ttu-id="cffb5-174">Имя связи</span><span class="sxs-lookup"><span data-stu-id="cffb5-174">Relationship name</span></span> | <span data-ttu-id="cffb5-175">Тип</span><span class="sxs-lookup"><span data-stu-id="cffb5-175">Type</span></span>                             | <span data-ttu-id="cffb5-176">Описание</span><span class="sxs-lookup"><span data-stu-id="cffb5-176">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="cffb5-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="cffb5-177">**columns**</span></span>       | <span data-ttu-id="cffb5-178">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="cffb5-178">Collection([columnDefinition][])</span></span> | <span data-ttu-id="cffb5-179">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="cffb5-179">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="cffb5-180">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="cffb5-180">**contentTypes**</span></span>  | <span data-ttu-id="cffb5-181">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="cffb5-181">Collection([contentType][])</span></span>      | <span data-ttu-id="cffb5-182">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="cffb5-182">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="cffb5-183">**drive**</span><span class="sxs-lookup"><span data-stu-id="cffb5-183">**drive**</span></span>         | <span data-ttu-id="cffb5-184">[drive][]</span><span class="sxs-lookup"><span data-stu-id="cffb5-184">[drive][]</span></span>                        | <span data-ttu-id="cffb5-185">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="cffb5-185">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="cffb5-186">**drives**</span><span class="sxs-lookup"><span data-stu-id="cffb5-186">**drives**</span></span>        | <span data-ttu-id="cffb5-187">Коллекция([drive][])</span><span class="sxs-lookup"><span data-stu-id="cffb5-187">Collection([drive][])</span></span>            | <span data-ttu-id="cffb5-188">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="cffb5-188">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="cffb5-189">**items**</span><span class="sxs-lookup"><span data-stu-id="cffb5-189">**items**</span></span>         | <span data-ttu-id="cffb5-190">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="cffb5-190">Collection([baseItem][])</span></span>         | <span data-ttu-id="cffb5-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="cffb5-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="cffb5-193">**lists**</span><span class="sxs-lookup"><span data-stu-id="cffb5-193">**lists**</span></span>         | <span data-ttu-id="cffb5-194">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="cffb5-194">Collection([list][])</span></span>             | <span data-ttu-id="cffb5-195">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="cffb5-195">The collection of lists under this site.</span></span>
| <span data-ttu-id="cffb5-196">**sites**</span><span class="sxs-lookup"><span data-stu-id="cffb5-196">**sites**</span></span>         | <span data-ttu-id="cffb5-197">Коллекция([site][])</span><span class="sxs-lookup"><span data-stu-id="cffb5-197">Collection([site][])</span></span>             | <span data-ttu-id="cffb5-198">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="cffb5-198">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="cffb5-199">**onenote**</span><span class="sxs-lookup"><span data-stu-id="cffb5-199">**onenote**</span></span>       | <span data-ttu-id="cffb5-200">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="cffb5-200">[onenote][]</span></span>                      | <span data-ttu-id="cffb5-201">Вызывает службу OneNote для выполнения операций, связанных с записными книжками.</span><span class="sxs-lookup"><span data-stu-id="cffb5-201">Calls the OneNote service for notebook related operations.</span></span>

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
