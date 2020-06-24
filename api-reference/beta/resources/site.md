---
author: JeremyKelley
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: fc6a7472da2676d0266d964b7bdddee976d5ac8c
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864226"
---
# <a name="site-resource-type"></a><span data-ttu-id="ab2e3-103">Тип ресурса site</span><span class="sxs-lookup"><span data-stu-id="ab2e3-103">site resource type</span></span>

<span data-ttu-id="ab2e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab2e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab2e3-105">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="ab2e3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ab2e3-106">Methods</span></span>

| <span data-ttu-id="ab2e3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ab2e3-107">Method</span></span>                         | <span data-ttu-id="ab2e3-108">Путь REST</span><span class="sxs-lookup"><span data-stu-id="ab2e3-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="ab2e3-109">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-109">[Get root site][]</span></span>              | <span data-ttu-id="ab2e3-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="ab2e3-110">GET /sites/root</span></span>
| <span data-ttu-id="ab2e3-111">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-111">[Get site][]</span></span>                   | <span data-ttu-id="ab2e3-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="ab2e3-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="ab2e3-113">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-113">[Get site by path][]</span></span>           | <span data-ttu-id="ab2e3-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="ab2e3-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="ab2e3-115">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-115">[Get site for a group][]</span></span>       | <span data-ttu-id="ab2e3-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="ab2e3-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="ab2e3-117">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-117">[Get analytics][]</span></span>              | <span data-ttu-id="ab2e3-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="ab2e3-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="ab2e3-119">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-119">[Get activities by interval][]</span></span> | <span data-ttu-id="ab2e3-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="ab2e3-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="ab2e3-121">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-121">[List pages][]</span></span>                 | <span data-ttu-id="ab2e3-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="ab2e3-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="ab2e3-123">[Перечисление корневых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-123">[List root sites][]</span></span>            | <span data-ttu-id="ab2e3-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="ab2e3-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="ab2e3-125">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-125">[Search for sites][]</span></span>           | <span data-ttu-id="ab2e3-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="ab2e3-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="ab2e3-127">[Отслеживание сайта][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-127">[Follow site][]</span></span>                | <span data-ttu-id="ab2e3-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="ab2e3-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="ab2e3-129">[Прекращение отслеживания сайта][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-129">[Unfollow site][]</span></span>              | <span data-ttu-id="ab2e3-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="ab2e3-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="ab2e3-131">[Перечисление отслеживаемых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-131">[List followed sites][]</span></span>        | <span data-ttu-id="ab2e3-132">GET /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="ab2e3-132">GET /me/followedSites</span></span>

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
[Перечисление отслеживаемых сайтов]: ../api/sites-list-followed.md
[List followed sites]: ../api/sites-list-followed.md


## <a name="properties"></a><span data-ttu-id="ab2e3-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab2e3-145">Properties</span></span>

| <span data-ttu-id="ab2e3-146">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ab2e3-146">Property name</span></span>            | <span data-ttu-id="ab2e3-147">Тип</span><span class="sxs-lookup"><span data-stu-id="ab2e3-147">Type</span></span>               | <span data-ttu-id="ab2e3-148">Описание</span><span class="sxs-lookup"><span data-stu-id="ab2e3-148">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="ab2e3-149">**id**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-149">**id**</span></span>                   | <span data-ttu-id="ab2e3-150">string</span><span class="sxs-lookup"><span data-stu-id="ab2e3-150">string</span></span>             | <span data-ttu-id="ab2e3-151">[Уникальный идентификатор](#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-151">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="ab2e3-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-152">Read-only.</span></span>
| <span data-ttu-id="ab2e3-153">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-153">**createdDateTime**</span></span>      | <span data-ttu-id="ab2e3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab2e3-154">DateTimeOffset</span></span>     | <span data-ttu-id="ab2e3-155">The date and time the item was created.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-155">The date and time the item was created.</span></span> <span data-ttu-id="ab2e3-156">Read-only.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-156">Read-only.</span></span>
| <span data-ttu-id="ab2e3-157">**description**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-157">**description**</span></span>          | <span data-ttu-id="ab2e3-158">string</span><span class="sxs-lookup"><span data-stu-id="ab2e3-158">string</span></span>             | <span data-ttu-id="ab2e3-159">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-159">The descriptive text for the site.</span></span>
| <span data-ttu-id="ab2e3-160">**eTag**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-160">**eTag**</span></span>                 | <span data-ttu-id="ab2e3-161">string</span><span class="sxs-lookup"><span data-stu-id="ab2e3-161">string</span></span>             | <span data-ttu-id="ab2e3-162">ETag for the item.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-162">ETag for the item.</span></span> <span data-ttu-id="ab2e3-163">Read-only.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-163">Read-only.</span></span>                                                                  |
| <span data-ttu-id="ab2e3-164">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-164">**displayName**</span></span>          | <span data-ttu-id="ab2e3-165">string</span><span class="sxs-lookup"><span data-stu-id="ab2e3-165">string</span></span>             | <span data-ttu-id="ab2e3-166">The full title for the site.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-166">The full title for the site.</span></span> <span data-ttu-id="ab2e3-167">Read-only.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-167">Read-only.</span></span>
| <span data-ttu-id="ab2e3-168">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-168">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ab2e3-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab2e3-169">DateTimeOffset</span></span>     | <span data-ttu-id="ab2e3-170">The date and time the item was last modified.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-170">The date and time the item was last modified.</span></span> <span data-ttu-id="ab2e3-171">Read-only.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-171">Read-only.</span></span>
| <span data-ttu-id="ab2e3-172">**name**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-172">**name**</span></span>                 | <span data-ttu-id="ab2e3-173">string</span><span class="sxs-lookup"><span data-stu-id="ab2e3-173">string</span></span>             | <span data-ttu-id="ab2e3-174">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-174">The name / title of the item.</span></span>
| <span data-ttu-id="ab2e3-175">**root**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-175">**root**</span></span>                 | <span data-ttu-id="ab2e3-176">[root][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-176">[root][]</span></span>           | <span data-ttu-id="ab2e3-177">If present, indicates that this is the root site in the site collection.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-177">If present, indicates that this is the root site in the site collection.</span></span> <span data-ttu-id="ab2e3-178">Read-only.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-178">Read-only.</span></span>
| <span data-ttu-id="ab2e3-179">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-179">**sharepointIds**</span></span>        | <span data-ttu-id="ab2e3-180">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-180">[sharepointIds][]</span></span>  | <span data-ttu-id="ab2e3-181">Returns identifiers useful for SharePoint REST compatibility.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-181">Returns identifiers useful for SharePoint REST compatibility.</span></span> <span data-ttu-id="ab2e3-182">Read-only.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-182">Read-only.</span></span>
| <span data-ttu-id="ab2e3-183">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-183">**siteCollection**</span></span>       | <span data-ttu-id="ab2e3-184">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-184">[siteCollection][]</span></span> | <span data-ttu-id="ab2e3-185">Provides details about the site's site collection.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-185">Provides details about the site's site collection.</span></span> <span data-ttu-id="ab2e3-186">Available only on the root site.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-186">Available only on the root site.</span></span> <span data-ttu-id="ab2e3-187">Read-only.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-187">Read-only.</span></span>
| <span data-ttu-id="ab2e3-188">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-188">**webUrl**</span></span>               | <span data-ttu-id="ab2e3-189">string (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="ab2e3-189">string (url)</span></span>       | <span data-ttu-id="ab2e3-190">URL that displays the item in the browser.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-190">URL that displays the item in the browser.</span></span> <span data-ttu-id="ab2e3-191">Read-only.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-191">Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="ab2e3-192">Свойство id</span><span class="sxs-lookup"><span data-stu-id="ab2e3-192">id property</span></span>
<span data-ttu-id="ab2e3-193">Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="ab2e3-193">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="ab2e3-194">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="ab2e3-194">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="ab2e3-195">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="ab2e3-195">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="ab2e3-196">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="ab2e3-196">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="ab2e3-197">Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-197">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="ab2e3-198">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-198">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="ab2e3-199">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-199">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="ab2e3-200">Связи</span><span class="sxs-lookup"><span data-stu-id="ab2e3-200">Relationships</span></span>

| <span data-ttu-id="ab2e3-201">Имя связи</span><span class="sxs-lookup"><span data-stu-id="ab2e3-201">Relationship name</span></span> | <span data-ttu-id="ab2e3-202">Тип</span><span class="sxs-lookup"><span data-stu-id="ab2e3-202">Type</span></span>                             | <span data-ttu-id="ab2e3-203">Описание</span><span class="sxs-lookup"><span data-stu-id="ab2e3-203">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="ab2e3-204">**analytics**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-204">**analytics**</span></span>     | <span data-ttu-id="ab2e3-205">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-205">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="ab2e3-206">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-206">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="ab2e3-207">**columns**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-207">**columns**</span></span>       | <span data-ttu-id="ab2e3-208">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="ab2e3-208">Collection([columnDefinition][])</span></span> | <span data-ttu-id="ab2e3-209">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-209">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="ab2e3-210">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-210">**contentTypes**</span></span>  | <span data-ttu-id="ab2e3-211">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="ab2e3-211">Collection([contentType][])</span></span>      | <span data-ttu-id="ab2e3-212">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-212">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="ab2e3-213">**drive**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-213">**drive**</span></span>         | <span data-ttu-id="ab2e3-214">[drive][]</span><span class="sxs-lookup"><span data-stu-id="ab2e3-214">[drive][]</span></span>                        | <span data-ttu-id="ab2e3-215">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-215">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="ab2e3-216">**drives**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-216">**drives**</span></span>        | <span data-ttu-id="ab2e3-217">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="ab2e3-217">Collection([drive][])</span></span>            | <span data-ttu-id="ab2e3-218">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-218">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="ab2e3-219">**items**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-219">**items**</span></span>         | <span data-ttu-id="ab2e3-220">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="ab2e3-220">Collection([baseItem][])</span></span>         | <span data-ttu-id="ab2e3-221">Used to address any item contained in this site.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-221">Used to address any item contained in this site.</span></span> <span data-ttu-id="ab2e3-222">This collection cannot be enumerated.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-222">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="ab2e3-223">**lists**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-223">**lists**</span></span>         | <span data-ttu-id="ab2e3-224">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="ab2e3-224">Collection([list][])</span></span>             | <span data-ttu-id="ab2e3-225">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-225">The collection of lists under this site.</span></span>
| <span data-ttu-id="ab2e3-226">**pages**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-226">**pages**</span></span>         | <span data-ttu-id="ab2e3-227">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="ab2e3-227">Collection([sitePage][])</span></span>         | <span data-ttu-id="ab2e3-228">Коллекция страниц в списке SitePages на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-228">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="ab2e3-229">**sites**</span><span class="sxs-lookup"><span data-stu-id="ab2e3-229">**sites**</span></span>         | <span data-ttu-id="ab2e3-230">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="ab2e3-230">Collection([site][])</span></span>             | <span data-ttu-id="ab2e3-231">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-231">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="ab2e3-243">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab2e3-243">JSON representation</span></span>

<span data-ttu-id="ab2e3-244">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-244">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="ab2e3-245">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="ab2e3-245">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
