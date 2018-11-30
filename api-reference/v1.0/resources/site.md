---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: site
ms.openlocfilehash: ae8962dfa38c3c6f3e06ccb687eb42a4a8262f1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028508"
---
# <a name="site-resource"></a><span data-ttu-id="60948-102">Ресурс site</span><span class="sxs-lookup"><span data-stu-id="60948-102">Site resource</span></span>

<span data-ttu-id="60948-103">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="60948-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="60948-104">Задачи</span><span class="sxs-lookup"><span data-stu-id="60948-104">Tasks</span></span>

<span data-ttu-id="60948-105">Все приведенные ниже примеры относятся к `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="60948-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="60948-106">Имя задачи</span><span class="sxs-lookup"><span data-stu-id="60948-106">Task name</span></span>                | <span data-ttu-id="60948-107">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="60948-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="60948-108">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="60948-108">[Get root site][]</span></span>        | <span data-ttu-id="60948-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="60948-109">GET /sites/root</span></span>
| <span data-ttu-id="60948-110">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="60948-110">[Get site][]</span></span>             | <span data-ttu-id="60948-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="60948-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="60948-112">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="60948-112">[Get site by path][]</span></span>     | <span data-ttu-id="60948-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="60948-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="60948-114">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="60948-114">[Get site for a group][]</span></span> | <span data-ttu-id="60948-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="60948-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="60948-116">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="60948-116">[Search for sites][]</span></span>     | <span data-ttu-id="60948-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="60948-117">GET /sites?search={query}</span></span>

[Получение сайта]: ../api/site-get.md
[Get site]: ../api/site-get.md
[Получение корневого сайта]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[Получение сайта по пути]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[Получение сайта для группы]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[Поиск сайтов]: ../api/site-search.md
[Search for sites]: ../api/site-search.md

## <a name="json-representation"></a><span data-ttu-id="60948-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60948-123">JSON representation</span></span>

<span data-ttu-id="60948-124">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60948-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="60948-125">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="60948-125">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="60948-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="60948-126">Properties</span></span>

| <span data-ttu-id="60948-127">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="60948-127">Property name</span></span>            | <span data-ttu-id="60948-128">Тип</span><span class="sxs-lookup"><span data-stu-id="60948-128">Type</span></span>                                | <span data-ttu-id="60948-129">Описание</span><span class="sxs-lookup"><span data-stu-id="60948-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="60948-130">**id**</span><span class="sxs-lookup"><span data-stu-id="60948-130">**id**</span></span>                   | <span data-ttu-id="60948-131">строка</span><span class="sxs-lookup"><span data-stu-id="60948-131">string</span></span>                              | <span data-ttu-id="60948-p101">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60948-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="60948-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="60948-134">**createdDateTime**</span></span>      | <span data-ttu-id="60948-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60948-135">DateTimeOffset</span></span>                      | <span data-ttu-id="60948-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60948-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="60948-138">**description**</span><span class="sxs-lookup"><span data-stu-id="60948-138">**description**</span></span>          | <span data-ttu-id="60948-139">строка</span><span class="sxs-lookup"><span data-stu-id="60948-139">string</span></span>                              | <span data-ttu-id="60948-140">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="60948-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="60948-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="60948-141">**displayName**</span></span>          | <span data-ttu-id="60948-142">строка</span><span class="sxs-lookup"><span data-stu-id="60948-142">string</span></span>                              | <span data-ttu-id="60948-p103">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60948-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="60948-145">**eTag**;</span><span class="sxs-lookup"><span data-stu-id="60948-145">**eTag**</span></span>                 | <span data-ttu-id="60948-146">string</span><span class="sxs-lookup"><span data-stu-id="60948-146">string</span></span>                              | <span data-ttu-id="60948-p104">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60948-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="60948-149">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="60948-149">**lastModifiedDateTime**</span></span> | <span data-ttu-id="60948-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60948-150">DateTimeOffset</span></span>                      | <span data-ttu-id="60948-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60948-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="60948-153">**name**</span><span class="sxs-lookup"><span data-stu-id="60948-153">**name**</span></span>                 | <span data-ttu-id="60948-154">строка</span><span class="sxs-lookup"><span data-stu-id="60948-154">string</span></span>                              | <span data-ttu-id="60948-155">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="60948-155">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="60948-156">**root**</span><span class="sxs-lookup"><span data-stu-id="60948-156">**root**</span></span>                 | [<span data-ttu-id="60948-157">root</span><span class="sxs-lookup"><span data-stu-id="60948-157">root</span></span>](root.md)                     | <span data-ttu-id="60948-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60948-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="60948-160">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="60948-160">**sharepointIds**</span></span>        | [<span data-ttu-id="60948-161">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="60948-161">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="60948-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60948-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="60948-164">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="60948-164">**siteCollection**</span></span>       | [<span data-ttu-id="60948-165">siteCollection</span><span class="sxs-lookup"><span data-stu-id="60948-165">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="60948-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60948-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="60948-169">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="60948-169">**webUrl**</span></span>               | <span data-ttu-id="60948-170">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="60948-170">string (url)</span></span>                        | <span data-ttu-id="60948-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60948-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="60948-173">Связи</span><span class="sxs-lookup"><span data-stu-id="60948-173">Relationships</span></span>

| <span data-ttu-id="60948-174">Имя связи</span><span class="sxs-lookup"><span data-stu-id="60948-174">Relationship name</span></span> | <span data-ttu-id="60948-175">Тип</span><span class="sxs-lookup"><span data-stu-id="60948-175">Type</span></span>                             | <span data-ttu-id="60948-176">Описание</span><span class="sxs-lookup"><span data-stu-id="60948-176">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="60948-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="60948-177">**columns**</span></span>       | <span data-ttu-id="60948-178">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="60948-178">Collection([columnDefinition][])</span></span> | <span data-ttu-id="60948-179">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="60948-179">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="60948-180">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="60948-180">**contentTypes**</span></span>  | <span data-ttu-id="60948-181">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="60948-181">Collection([contentType][])</span></span>      | <span data-ttu-id="60948-182">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="60948-182">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="60948-183">**drive**</span><span class="sxs-lookup"><span data-stu-id="60948-183">**drive**</span></span>         | <span data-ttu-id="60948-184">[drive][]</span><span class="sxs-lookup"><span data-stu-id="60948-184">[drive][]</span></span>                        | <span data-ttu-id="60948-185">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="60948-185">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="60948-186">**drives**</span><span class="sxs-lookup"><span data-stu-id="60948-186">**drives**</span></span>        | <span data-ttu-id="60948-187">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="60948-187">Collection([drive][])</span></span>            | <span data-ttu-id="60948-188">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="60948-188">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="60948-189">**items**</span><span class="sxs-lookup"><span data-stu-id="60948-189">**items**</span></span>         | <span data-ttu-id="60948-190">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="60948-190">Collection([baseItem][])</span></span>         | <span data-ttu-id="60948-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="60948-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="60948-193">**lists**</span><span class="sxs-lookup"><span data-stu-id="60948-193">**lists**</span></span>         | <span data-ttu-id="60948-194">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="60948-194">Collection([list][])</span></span>             | <span data-ttu-id="60948-195">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="60948-195">The collection of lists under this site.</span></span>
| <span data-ttu-id="60948-196">**sites**</span><span class="sxs-lookup"><span data-stu-id="60948-196">**sites**</span></span>         | <span data-ttu-id="60948-197">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="60948-197">Collection([site][])</span></span>             | <span data-ttu-id="60948-198">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="60948-198">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="60948-199">**onenote**</span><span class="sxs-lookup"><span data-stu-id="60948-199">**onenote**</span></span>       | <span data-ttu-id="60948-200">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="60948-200">[onenote][]</span></span>                      | <span data-ttu-id="60948-201">Вызывает службу OneNote для выполнения операций, связанных с записными книжками.</span><span class="sxs-lookup"><span data-stu-id="60948-201">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
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
