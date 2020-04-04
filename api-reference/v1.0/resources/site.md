---
author: JeremyKelley
ms.author: JeremyKelley
title: Ресурс site
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 7ba96c6cc62bd6efbff8e0efb6062104d994090c
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108552"
---
# <a name="site-resource"></a><span data-ttu-id="9d9ca-103">Ресурс site</span><span class="sxs-lookup"><span data-stu-id="9d9ca-103">site resource</span></span>

<span data-ttu-id="9d9ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d9ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d9ca-105">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="9d9ca-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9d9ca-106">Methods</span></span>

| <span data-ttu-id="9d9ca-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9d9ca-107">Method</span></span>                | <span data-ttu-id="9d9ca-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="9d9ca-108">Return type</span></span> | <span data-ttu-id="9d9ca-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9d9ca-109">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="9d9ca-110">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-110">[Get root site][]</span></span>        | <span data-ttu-id="9d9ca-111">site</span><span class="sxs-lookup"><span data-stu-id="9d9ca-111">site</span></span> | <span data-ttu-id="9d9ca-112">Получение доступа к корневому сайту SharePoint внутри клиента.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-112">Access the root SharePoint site within a tenant.</span></span>
| <span data-ttu-id="9d9ca-113">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-113">[Get site][]</span></span>             | <span data-ttu-id="9d9ca-114">site</span><span class="sxs-lookup"><span data-stu-id="9d9ca-114">site</span></span> | <span data-ttu-id="9d9ca-115">Получение доступа к сайту SharePoint с помощью параметра siteId.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-115">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="9d9ca-116">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-116">[Get site by path][]</span></span>     | <span data-ttu-id="9d9ca-117">site</span><span class="sxs-lookup"><span data-stu-id="9d9ca-117">site</span></span> | <span data-ttu-id="9d9ca-118">Получение доступа к корневому сайту SharePoint с использованием относительного пути.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-118">Access the root SharePoint site with a relative path.</span></span>
| <span data-ttu-id="9d9ca-119">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-119">[Get site for a group][]</span></span> | <span data-ttu-id="9d9ca-120">site</span><span class="sxs-lookup"><span data-stu-id="9d9ca-120">site</span></span> | <span data-ttu-id="9d9ca-121">Получение доступа к сайту группы для группы.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-121">Access the team site for a group.</span></span>
| <span data-ttu-id="9d9ca-122">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-122">[Get analytics][]</span></span>              | <span data-ttu-id="9d9ca-123">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-123">[itemAnalytics][]</span></span> | <span data-ttu-id="9d9ca-124">Получение аналитических данных для ресурса.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-124">Get analytics for this resource.</span></span> 
| <span data-ttu-id="9d9ca-125">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-125">[Get activities by interval][]</span></span> | <span data-ttu-id="9d9ca-126">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-126">[itemActivityStat][]</span></span> | <span data-ttu-id="9d9ca-127">Получение коллекции объектов **itemActivityStats** в пределах указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-127">Get a collection of **itemActivityStats** within the specified time interval.</span></span>
| <span data-ttu-id="9d9ca-128">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-128">[Search for sites][]</span></span>     | <span data-ttu-id="9d9ca-129">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="9d9ca-129">collection of site</span></span> | <span data-ttu-id="9d9ca-130">Поиск сайтов, соответствующих указанным ключевым словам, в клиенте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-130">Search across a SharePoint tenant for sites that match keywords provided.</span></span>
| <span data-ttu-id="9d9ca-131">[Отслеживание сайта][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-131">[Follow Site][]</span></span>          | <span data-ttu-id="9d9ca-132">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="9d9ca-132">collection of site</span></span> | <span data-ttu-id="9d9ca-133">Отслеживание сайта пользователя или нескольких сайтов.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-133">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="9d9ca-134">[Прекращение отслеживания сайта][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-134">[Unfollow Site][]</span></span>        | <span data-ttu-id="9d9ca-135">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="9d9ca-135">collection of site</span></span> | <span data-ttu-id="9d9ca-136">Отслеживание сайта пользователя или нескольких сайтов.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-136">Follow a user's site or multiple sites.</span></span>

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

## <a name="properties"></a><span data-ttu-id="9d9ca-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d9ca-147">Properties</span></span>

| <span data-ttu-id="9d9ca-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d9ca-148">Property</span></span>            | <span data-ttu-id="9d9ca-149">Тип</span><span class="sxs-lookup"><span data-stu-id="9d9ca-149">Type</span></span>                                | <span data-ttu-id="9d9ca-150">Описание</span><span class="sxs-lookup"><span data-stu-id="9d9ca-150">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9d9ca-151">**id**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-151">**id**</span></span>                   | <span data-ttu-id="9d9ca-152">string</span><span class="sxs-lookup"><span data-stu-id="9d9ca-152">string</span></span>                              | <span data-ttu-id="9d9ca-p101">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="9d9ca-155">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-155">**createdDateTime**</span></span>      | <span data-ttu-id="9d9ca-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d9ca-156">DateTimeOffset</span></span>                      | <span data-ttu-id="9d9ca-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="9d9ca-159">**description**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-159">**description**</span></span>          | <span data-ttu-id="9d9ca-160">string</span><span class="sxs-lookup"><span data-stu-id="9d9ca-160">string</span></span>                              | <span data-ttu-id="9d9ca-161">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-161">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="9d9ca-162">**displayName**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-162">**displayName**</span></span>          | <span data-ttu-id="9d9ca-163">string</span><span class="sxs-lookup"><span data-stu-id="9d9ca-163">string</span></span>                              | <span data-ttu-id="9d9ca-p103">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="9d9ca-166">**eTag**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-166">**eTag**</span></span>                 | <span data-ttu-id="9d9ca-167">string</span><span class="sxs-lookup"><span data-stu-id="9d9ca-167">string</span></span>                              | <span data-ttu-id="9d9ca-p104">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="9d9ca-170">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-170">**lastModifiedDateTime**</span></span> | <span data-ttu-id="9d9ca-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d9ca-171">DateTimeOffset</span></span>                      | <span data-ttu-id="9d9ca-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="9d9ca-174">**name**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-174">**name**</span></span>                 | <span data-ttu-id="9d9ca-175">string</span><span class="sxs-lookup"><span data-stu-id="9d9ca-175">string</span></span>                              | <span data-ttu-id="9d9ca-176">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-176">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="9d9ca-177">**root**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-177">**root**</span></span>                 | [<span data-ttu-id="9d9ca-178">root</span><span class="sxs-lookup"><span data-stu-id="9d9ca-178">root</span></span>](root.md)                     | <span data-ttu-id="9d9ca-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="9d9ca-181">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-181">**sharepointIds**</span></span>        | [<span data-ttu-id="9d9ca-182">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="9d9ca-182">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="9d9ca-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="9d9ca-185">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-185">**siteCollection**</span></span>       | [<span data-ttu-id="9d9ca-186">siteCollection</span><span class="sxs-lookup"><span data-stu-id="9d9ca-186">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="9d9ca-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="9d9ca-190">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-190">**webUrl**</span></span>               | <span data-ttu-id="9d9ca-191">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="9d9ca-191">string (url)</span></span>                        | <span data-ttu-id="9d9ca-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

### <a name="id-property"></a><span data-ttu-id="9d9ca-194">Свойство id</span><span class="sxs-lookup"><span data-stu-id="9d9ca-194">id property</span></span>
<span data-ttu-id="9d9ca-195">Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="9d9ca-195">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="9d9ca-196">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="9d9ca-196">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="9d9ca-197">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="9d9ca-197">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="9d9ca-198">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="9d9ca-198">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="9d9ca-199">Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-199">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="9d9ca-200">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-200">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="9d9ca-201">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-201">`/groups/{group-id}/sites/root`: The group's team site.</span></span>
  
## <a name="relationships"></a><span data-ttu-id="9d9ca-202">Отношения</span><span class="sxs-lookup"><span data-stu-id="9d9ca-202">Relationships</span></span>

| <span data-ttu-id="9d9ca-203">Связь</span><span class="sxs-lookup"><span data-stu-id="9d9ca-203">Relationship</span></span>      | <span data-ttu-id="9d9ca-204">Тип</span><span class="sxs-lookup"><span data-stu-id="9d9ca-204">Type</span></span>                             | <span data-ttu-id="9d9ca-205">Описание</span><span class="sxs-lookup"><span data-stu-id="9d9ca-205">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="9d9ca-206">**analytics**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-206">**analytics**</span></span>     | <span data-ttu-id="9d9ca-207">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-207">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="9d9ca-208">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-208">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="9d9ca-209">**columns**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-209">**columns**</span></span>       | <span data-ttu-id="9d9ca-210">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="9d9ca-210">Collection([columnDefinition][])</span></span> | <span data-ttu-id="9d9ca-211">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-211">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="9d9ca-212">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-212">**contentTypes**</span></span>  | <span data-ttu-id="9d9ca-213">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="9d9ca-213">Collection([contentType][])</span></span>      | <span data-ttu-id="9d9ca-214">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-214">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="9d9ca-215">**drive**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-215">**drive**</span></span>         | <span data-ttu-id="9d9ca-216">[drive][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-216">[drive][]</span></span>                        | <span data-ttu-id="9d9ca-217">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-217">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="9d9ca-218">**drives**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-218">**drives**</span></span>        | <span data-ttu-id="9d9ca-219">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="9d9ca-219">Collection([drive][])</span></span>            | <span data-ttu-id="9d9ca-220">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-220">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="9d9ca-221">**items**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-221">**items**</span></span>         | <span data-ttu-id="9d9ca-222">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="9d9ca-222">Collection([baseItem][])</span></span>         | <span data-ttu-id="9d9ca-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="9d9ca-225">**lists**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-225">**lists**</span></span>         | <span data-ttu-id="9d9ca-226">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="9d9ca-226">Collection([list][])</span></span>             | <span data-ttu-id="9d9ca-227">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-227">The collection of lists under this site.</span></span>
| <span data-ttu-id="9d9ca-228">**sites**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-228">**sites**</span></span>         | <span data-ttu-id="9d9ca-229">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="9d9ca-229">Collection([site][])</span></span>             | <span data-ttu-id="9d9ca-230">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-230">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="9d9ca-231">**onenote**</span><span class="sxs-lookup"><span data-stu-id="9d9ca-231">**onenote**</span></span>       | <span data-ttu-id="9d9ca-232">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="9d9ca-232">[onenote][]</span></span>                      | <span data-ttu-id="9d9ca-233">Вызывает службу OneNote для выполнения операций, связанных с записными книжками.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-233">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="9d9ca-242">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d9ca-242">JSON representation</span></span>

<span data-ttu-id="9d9ca-243">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-243">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="9d9ca-244">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-244">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
