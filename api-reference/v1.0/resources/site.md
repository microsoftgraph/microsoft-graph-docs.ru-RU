---
author: JeremyKelley
ms.author: JeremyKelley
title: Ресурс site
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 43e321ef3b04124095257a6bf6b9d218ac080a3d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086447"
---
# <a name="site-resource"></a><span data-ttu-id="e1e5d-103">Ресурс site</span><span class="sxs-lookup"><span data-stu-id="e1e5d-103">site resource</span></span>

<span data-ttu-id="e1e5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1e5d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1e5d-105">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="e1e5d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e1e5d-106">Methods</span></span>

| <span data-ttu-id="e1e5d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e1e5d-107">Method</span></span>                | <span data-ttu-id="e1e5d-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="e1e5d-108">Return type</span></span> | <span data-ttu-id="e1e5d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e1e5d-109">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="e1e5d-110">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-110">[Get root site][]</span></span>        | <span data-ttu-id="e1e5d-111">site</span><span class="sxs-lookup"><span data-stu-id="e1e5d-111">site</span></span> | <span data-ttu-id="e1e5d-112">Получение доступа к корневому сайту SharePoint внутри клиента.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-112">Access the root SharePoint site within a tenant.</span></span>
| <span data-ttu-id="e1e5d-113">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-113">[Get site][]</span></span>             | <span data-ttu-id="e1e5d-114">site</span><span class="sxs-lookup"><span data-stu-id="e1e5d-114">site</span></span> | <span data-ttu-id="e1e5d-115">Получение доступа к сайту SharePoint с помощью параметра siteId.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-115">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="e1e5d-116">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-116">[Get site by path][]</span></span>     | <span data-ttu-id="e1e5d-117">site</span><span class="sxs-lookup"><span data-stu-id="e1e5d-117">site</span></span> | <span data-ttu-id="e1e5d-118">Получение доступа к корневому сайту SharePoint с использованием относительного пути.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-118">Access the root SharePoint site with a relative path.</span></span>
| <span data-ttu-id="e1e5d-119">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-119">[Get site for a group][]</span></span> | <span data-ttu-id="e1e5d-120">site</span><span class="sxs-lookup"><span data-stu-id="e1e5d-120">site</span></span> | <span data-ttu-id="e1e5d-121">Получение доступа к сайту группы для группы.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-121">Access the team site for a group.</span></span>
| <span data-ttu-id="e1e5d-122">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-122">[Get analytics][]</span></span>              | <span data-ttu-id="e1e5d-123">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-123">[itemAnalytics][]</span></span> | <span data-ttu-id="e1e5d-124">Получение аналитических данных для ресурса.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-124">Get analytics for this resource.</span></span> 
| <span data-ttu-id="e1e5d-125">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-125">[Get activities by interval][]</span></span> | <span data-ttu-id="e1e5d-126">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-126">[itemActivityStat][]</span></span> | <span data-ttu-id="e1e5d-127">Получение коллекции объектов **itemActivityStats** в пределах указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-127">Get a collection of **itemActivityStats** within the specified time interval.</span></span>
| <span data-ttu-id="e1e5d-128">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-128">[Search for sites][]</span></span>     | <span data-ttu-id="e1e5d-129">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="e1e5d-129">collection of site</span></span> | <span data-ttu-id="e1e5d-130">Поиск сайтов, соответствующих указанным ключевым словам, в клиенте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-130">Search across a SharePoint tenant for sites that match keywords provided.</span></span>
| <span data-ttu-id="e1e5d-131">[Отслеживание сайта][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-131">[Follow site][]</span></span>          | <span data-ttu-id="e1e5d-132">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="e1e5d-132">collection of site</span></span> | <span data-ttu-id="e1e5d-133">Отслеживание сайта пользователя или нескольких сайтов.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-133">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="e1e5d-134">[Прекращение отслеживания сайта][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-134">[Unfollow site][]</span></span>        | <span data-ttu-id="e1e5d-135">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="e1e5d-135">collection of site</span></span> | <span data-ttu-id="e1e5d-136">Отслеживание сайта пользователя или нескольких сайтов.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-136">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="e1e5d-137">[Перечисление отслеживаемых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-137">[List followed sites][]</span></span>  | <span data-ttu-id="e1e5d-138">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="e1e5d-138">collection of site</span></span> | <span data-ttu-id="e1e5d-139">Перечисление сайтов, отслеживаемых вошедшим пользователем.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-139">List the sites that have been followed by the signed in user.</span></span>

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
[Отслеживание сайта]: ../api/site-follow.md
[Follow site]: ../api/site-follow.md
[Прекращение отслеживания сайта]: ../api/site-unfollow.md
[Unfollow site]: ../api/site-unfollow.md
[Перечисление отслеживаемых сайтов]: ../api/sites-list-followed.md
[List followed sites]: ../api/sites-list-followed.md

## <a name="properties"></a><span data-ttu-id="e1e5d-151">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1e5d-151">Properties</span></span>

| <span data-ttu-id="e1e5d-152">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1e5d-152">Property</span></span>            | <span data-ttu-id="e1e5d-153">Тип</span><span class="sxs-lookup"><span data-stu-id="e1e5d-153">Type</span></span>                                | <span data-ttu-id="e1e5d-154">Описание</span><span class="sxs-lookup"><span data-stu-id="e1e5d-154">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e1e5d-155">**id**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-155">**id**</span></span>                   | <span data-ttu-id="e1e5d-156">string</span><span class="sxs-lookup"><span data-stu-id="e1e5d-156">string</span></span>                              | <span data-ttu-id="e1e5d-p101">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="e1e5d-159">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-159">**createdDateTime**</span></span>      | <span data-ttu-id="e1e5d-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1e5d-160">DateTimeOffset</span></span>                      | <span data-ttu-id="e1e5d-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="e1e5d-163">**description**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-163">**description**</span></span>          | <span data-ttu-id="e1e5d-164">string</span><span class="sxs-lookup"><span data-stu-id="e1e5d-164">string</span></span>                              | <span data-ttu-id="e1e5d-165">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-165">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="e1e5d-166">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-166">**displayName**</span></span>          | <span data-ttu-id="e1e5d-167">string</span><span class="sxs-lookup"><span data-stu-id="e1e5d-167">string</span></span>                              | <span data-ttu-id="e1e5d-p103">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="e1e5d-170">**eTag**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-170">**eTag**</span></span>                 | <span data-ttu-id="e1e5d-171">string</span><span class="sxs-lookup"><span data-stu-id="e1e5d-171">string</span></span>                              | <span data-ttu-id="e1e5d-p104">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="e1e5d-174">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-174">**lastModifiedDateTime**</span></span> | <span data-ttu-id="e1e5d-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1e5d-175">DateTimeOffset</span></span>                      | <span data-ttu-id="e1e5d-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="e1e5d-178">**name**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-178">**name**</span></span>                 | <span data-ttu-id="e1e5d-179">string</span><span class="sxs-lookup"><span data-stu-id="e1e5d-179">string</span></span>                              | <span data-ttu-id="e1e5d-180">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-180">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="e1e5d-181">**root**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-181">**root**</span></span>                 | [<span data-ttu-id="e1e5d-182">root</span><span class="sxs-lookup"><span data-stu-id="e1e5d-182">root</span></span>](root.md)                     | <span data-ttu-id="e1e5d-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="e1e5d-185">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-185">**sharepointIds**</span></span>        | [<span data-ttu-id="e1e5d-186">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="e1e5d-186">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="e1e5d-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="e1e5d-189">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-189">**siteCollection**</span></span>       | [<span data-ttu-id="e1e5d-190">siteCollection</span><span class="sxs-lookup"><span data-stu-id="e1e5d-190">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="e1e5d-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="e1e5d-194">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-194">**webUrl**</span></span>               | <span data-ttu-id="e1e5d-195">string (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="e1e5d-195">string (url)</span></span>                        | <span data-ttu-id="e1e5d-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

### <a name="id-property"></a><span data-ttu-id="e1e5d-198">Свойство id</span><span class="sxs-lookup"><span data-stu-id="e1e5d-198">id property</span></span>
<span data-ttu-id="e1e5d-199">Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="e1e5d-199">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="e1e5d-200">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="e1e5d-200">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="e1e5d-201">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="e1e5d-201">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="e1e5d-202">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="e1e5d-202">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="e1e5d-203">Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-203">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="e1e5d-204">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-204">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="e1e5d-205">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-205">`/groups/{group-id}/sites/root`: The group's team site.</span></span>
  
## <a name="relationships"></a><span data-ttu-id="e1e5d-206">Отношения</span><span class="sxs-lookup"><span data-stu-id="e1e5d-206">Relationships</span></span>

| <span data-ttu-id="e1e5d-207">Связь</span><span class="sxs-lookup"><span data-stu-id="e1e5d-207">Relationship</span></span>      | <span data-ttu-id="e1e5d-208">Тип</span><span class="sxs-lookup"><span data-stu-id="e1e5d-208">Type</span></span>                             | <span data-ttu-id="e1e5d-209">Описание</span><span class="sxs-lookup"><span data-stu-id="e1e5d-209">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="e1e5d-210">**analytics**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-210">**analytics**</span></span>     | <span data-ttu-id="e1e5d-211">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-211">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="e1e5d-212">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-212">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="e1e5d-213">**columns**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-213">**columns**</span></span>       | <span data-ttu-id="e1e5d-214">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="e1e5d-214">Collection([columnDefinition][])</span></span> | <span data-ttu-id="e1e5d-215">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-215">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="e1e5d-216">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-216">**contentTypes**</span></span>  | <span data-ttu-id="e1e5d-217">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="e1e5d-217">Collection([contentType][])</span></span>      | <span data-ttu-id="e1e5d-218">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-218">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="e1e5d-219">**drive**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-219">**drive**</span></span>         | <span data-ttu-id="e1e5d-220">[drive][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-220">[drive][]</span></span>                        | <span data-ttu-id="e1e5d-221">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-221">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="e1e5d-222">**drives**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-222">**drives**</span></span>        | <span data-ttu-id="e1e5d-223">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="e1e5d-223">Collection([drive][])</span></span>            | <span data-ttu-id="e1e5d-224">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-224">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="e1e5d-225">**items**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-225">**items**</span></span>         | <span data-ttu-id="e1e5d-226">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="e1e5d-226">Collection([baseItem][])</span></span>         | <span data-ttu-id="e1e5d-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="e1e5d-229">**lists**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-229">**lists**</span></span>         | <span data-ttu-id="e1e5d-230">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="e1e5d-230">Collection([list][])</span></span>             | <span data-ttu-id="e1e5d-231">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-231">The collection of lists under this site.</span></span>
| <span data-ttu-id="e1e5d-232">**sites**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-232">**sites**</span></span>         | <span data-ttu-id="e1e5d-233">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="e1e5d-233">Collection([site][])</span></span>             | <span data-ttu-id="e1e5d-234">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-234">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="e1e5d-235">**onenote**</span><span class="sxs-lookup"><span data-stu-id="e1e5d-235">**onenote**</span></span>       | <span data-ttu-id="e1e5d-236">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="e1e5d-236">[onenote][]</span></span>                      | <span data-ttu-id="e1e5d-237">Вызывает службу OneNote для выполнения операций, связанных с записными книжками.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-237">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="e1e5d-246">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1e5d-246">JSON representation</span></span>

<span data-ttu-id="e1e5d-247">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-247">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="e1e5d-248">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="e1e5d-248">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

