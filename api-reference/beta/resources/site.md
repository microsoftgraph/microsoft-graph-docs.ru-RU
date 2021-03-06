---
author: JeremyKelley
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 587014aa0c9dbe4c05c0e3b946c3f6e44b7cb821
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442802"
---
# <a name="site-resource-type"></a><span data-ttu-id="92d99-103">Тип ресурса site</span><span class="sxs-lookup"><span data-stu-id="92d99-103">site resource type</span></span>

<span data-ttu-id="92d99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92d99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92d99-105">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="92d99-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="92d99-106">Методы</span><span class="sxs-lookup"><span data-stu-id="92d99-106">Methods</span></span>

| <span data-ttu-id="92d99-107">Метод</span><span class="sxs-lookup"><span data-stu-id="92d99-107">Method</span></span>                         | <span data-ttu-id="92d99-108">Путь REST</span><span class="sxs-lookup"><span data-stu-id="92d99-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="92d99-109">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="92d99-109">[Get root site][]</span></span>              | <span data-ttu-id="92d99-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="92d99-110">GET /sites/root</span></span>
| <span data-ttu-id="92d99-111">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="92d99-111">[Get site][]</span></span>                   | <span data-ttu-id="92d99-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="92d99-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="92d99-113">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="92d99-113">[Get site by path][]</span></span>           | <span data-ttu-id="92d99-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="92d99-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="92d99-115">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="92d99-115">[Get site for a group][]</span></span>       | <span data-ttu-id="92d99-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="92d99-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="92d99-117">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="92d99-117">[Get analytics][]</span></span>              | <span data-ttu-id="92d99-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="92d99-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="92d99-119">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="92d99-119">[Get activities by interval][]</span></span> | <span data-ttu-id="92d99-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="92d99-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="92d99-121">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="92d99-121">[List pages][]</span></span>                 | <span data-ttu-id="92d99-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="92d99-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="92d99-123">[Перечисление корневых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="92d99-123">[List root sites][]</span></span>            | <span data-ttu-id="92d99-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="92d99-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="92d99-125">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="92d99-125">[Search for sites][]</span></span>           | <span data-ttu-id="92d99-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="92d99-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="92d99-127">[Отслеживание сайта][]</span><span class="sxs-lookup"><span data-stu-id="92d99-127">[Follow site][]</span></span>                | <span data-ttu-id="92d99-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="92d99-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="92d99-129">[Прекращение отслеживания сайта][]</span><span class="sxs-lookup"><span data-stu-id="92d99-129">[Unfollow site][]</span></span>              | <span data-ttu-id="92d99-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="92d99-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="92d99-131">[Перечисление отслеживаемых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="92d99-131">[List followed sites][]</span></span>        | <span data-ttu-id="92d99-132">GET /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="92d99-132">GET /me/followedSites</span></span>
| <span data-ttu-id="92d99-133">[Получение разрешения][]</span><span class="sxs-lookup"><span data-stu-id="92d99-133">[Get permission][]</span></span>             | <span data-ttu-id="92d99-134">GET /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="92d99-134">GET /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="92d99-135">[Список разрешений][]</span><span class="sxs-lookup"><span data-stu-id="92d99-135">[List permissions][]</span></span>           | <span data-ttu-id="92d99-136">GET /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="92d99-136">GET /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="92d99-137">[Создание разрешений][]</span><span class="sxs-lookup"><span data-stu-id="92d99-137">[Create permissions][]</span></span>         | <span data-ttu-id="92d99-138">POST /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="92d99-138">POST /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="92d99-139">[Удаление разрешения][]</span><span class="sxs-lookup"><span data-stu-id="92d99-139">[Delete permission][]</span></span>         | <span data-ttu-id="92d99-140">DELETE /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="92d99-140">DELETE /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="92d99-141">[Обновление разрешения][]</span><span class="sxs-lookup"><span data-stu-id="92d99-141">[Update permission][]</span></span>         | <span data-ttu-id="92d99-142">PATCH /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="92d99-142">PATCH /sites/{site-id}/permissions/{permission-id}</span></span>

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
[Получение разрешения]: ../api/site-get-permission.md
[Get permission]: ../api/site-get-permission.md
[Список разрешений]: ../api/site-list-permissions.md
[List permissions]: ../api/site-list-permissions.md
[Создание разрешений]: ../api/site-post-permissions.md
[Create permissions]: ../api/site-post-permissions.md
[Удаление разрешения]: ../api/site-delete-permission.md
[Delete permission]: ../api/site-delete-permission.md
[Обновление разрешения]: ../api/site-update-permission.md
[Update permission]: ../api/site-update-permission.md


## <a name="properties"></a><span data-ttu-id="92d99-160">Свойства</span><span class="sxs-lookup"><span data-stu-id="92d99-160">Properties</span></span>

| <span data-ttu-id="92d99-161">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="92d99-161">Property name</span></span>            | <span data-ttu-id="92d99-162">Тип</span><span class="sxs-lookup"><span data-stu-id="92d99-162">Type</span></span>               | <span data-ttu-id="92d99-163">Описание</span><span class="sxs-lookup"><span data-stu-id="92d99-163">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="92d99-164">**id**</span><span class="sxs-lookup"><span data-stu-id="92d99-164">**id**</span></span>                   | <span data-ttu-id="92d99-165">string</span><span class="sxs-lookup"><span data-stu-id="92d99-165">string</span></span>             | <span data-ttu-id="92d99-166">[Уникальный идентификатор](#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="92d99-166">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="92d99-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d99-167">Read-only.</span></span>
| <span data-ttu-id="92d99-168">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="92d99-168">**createdDateTime**</span></span>      | <span data-ttu-id="92d99-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92d99-169">DateTimeOffset</span></span>     | <span data-ttu-id="92d99-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d99-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="92d99-172">**description**</span><span class="sxs-lookup"><span data-stu-id="92d99-172">**description**</span></span>          | <span data-ttu-id="92d99-173">string</span><span class="sxs-lookup"><span data-stu-id="92d99-173">string</span></span>             | <span data-ttu-id="92d99-174">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="92d99-174">The descriptive text for the site.</span></span>
| <span data-ttu-id="92d99-175">**eTag**</span><span class="sxs-lookup"><span data-stu-id="92d99-175">**eTag**</span></span>                 | <span data-ttu-id="92d99-176">string</span><span class="sxs-lookup"><span data-stu-id="92d99-176">string</span></span>             | <span data-ttu-id="92d99-p103">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d99-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="92d99-179">**displayName**</span><span class="sxs-lookup"><span data-stu-id="92d99-179">**displayName**</span></span>          | <span data-ttu-id="92d99-180">string</span><span class="sxs-lookup"><span data-stu-id="92d99-180">string</span></span>             | <span data-ttu-id="92d99-p104">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d99-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="92d99-183">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="92d99-183">**lastModifiedDateTime**</span></span> | <span data-ttu-id="92d99-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92d99-184">DateTimeOffset</span></span>     | <span data-ttu-id="92d99-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d99-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="92d99-187">**name**</span><span class="sxs-lookup"><span data-stu-id="92d99-187">**name**</span></span>                 | <span data-ttu-id="92d99-188">string</span><span class="sxs-lookup"><span data-stu-id="92d99-188">string</span></span>             | <span data-ttu-id="92d99-189">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="92d99-189">The name / title of the item.</span></span>
| <span data-ttu-id="92d99-190">**root**</span><span class="sxs-lookup"><span data-stu-id="92d99-190">**root**</span></span>                 | <span data-ttu-id="92d99-191">[root][]</span><span class="sxs-lookup"><span data-stu-id="92d99-191">[root][]</span></span>           | <span data-ttu-id="92d99-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d99-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="92d99-194">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="92d99-194">**sharepointIds**</span></span>        | <span data-ttu-id="92d99-195">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="92d99-195">[sharepointIds][]</span></span>  | <span data-ttu-id="92d99-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d99-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="92d99-198">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="92d99-198">**siteCollection**</span></span>       | <span data-ttu-id="92d99-199">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="92d99-199">[siteCollection][]</span></span> | <span data-ttu-id="92d99-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d99-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="92d99-203">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="92d99-203">**webUrl**</span></span>               | <span data-ttu-id="92d99-204">string (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="92d99-204">string (url)</span></span>       | <span data-ttu-id="92d99-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d99-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="92d99-207">Свойство id</span><span class="sxs-lookup"><span data-stu-id="92d99-207">id property</span></span>
<span data-ttu-id="92d99-208">Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="92d99-208">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="92d99-209">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="92d99-209">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="92d99-210">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="92d99-210">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="92d99-211">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="92d99-211">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="92d99-212">Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="92d99-212">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="92d99-213">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="92d99-213">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="92d99-214">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="92d99-214">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="92d99-215">Связи</span><span class="sxs-lookup"><span data-stu-id="92d99-215">Relationships</span></span>

| <span data-ttu-id="92d99-216">Имя связи</span><span class="sxs-lookup"><span data-stu-id="92d99-216">Relationship name</span></span> | <span data-ttu-id="92d99-217">Тип</span><span class="sxs-lookup"><span data-stu-id="92d99-217">Type</span></span>                             | <span data-ttu-id="92d99-218">Описание</span><span class="sxs-lookup"><span data-stu-id="92d99-218">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="92d99-219">**analytics**</span><span class="sxs-lookup"><span data-stu-id="92d99-219">**analytics**</span></span>     | <span data-ttu-id="92d99-220">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="92d99-220">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="92d99-221">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="92d99-221">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="92d99-222">**columns**</span><span class="sxs-lookup"><span data-stu-id="92d99-222">**columns**</span></span>       | <span data-ttu-id="92d99-223">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="92d99-223">Collection([columnDefinition][])</span></span> | <span data-ttu-id="92d99-224">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="92d99-224">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="92d99-225">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="92d99-225">**contentTypes**</span></span>  | <span data-ttu-id="92d99-226">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="92d99-226">Collection([contentType][])</span></span>      | <span data-ttu-id="92d99-227">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="92d99-227">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="92d99-228">**drive**</span><span class="sxs-lookup"><span data-stu-id="92d99-228">**drive**</span></span>         | <span data-ttu-id="92d99-229">[drive][]</span><span class="sxs-lookup"><span data-stu-id="92d99-229">[drive][]</span></span>                        | <span data-ttu-id="92d99-230">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="92d99-230">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="92d99-231">**drives**</span><span class="sxs-lookup"><span data-stu-id="92d99-231">**drives**</span></span>        | <span data-ttu-id="92d99-232">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="92d99-232">Collection([drive][])</span></span>            | <span data-ttu-id="92d99-233">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="92d99-233">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="92d99-234">**items**</span><span class="sxs-lookup"><span data-stu-id="92d99-234">**items**</span></span>         | <span data-ttu-id="92d99-235">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="92d99-235">Collection([baseItem][])</span></span>         | <span data-ttu-id="92d99-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="92d99-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="92d99-238">**lists**</span><span class="sxs-lookup"><span data-stu-id="92d99-238">**lists**</span></span>         | <span data-ttu-id="92d99-239">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="92d99-239">Collection([list][])</span></span>             | <span data-ttu-id="92d99-240">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="92d99-240">The collection of lists under this site.</span></span>
| <span data-ttu-id="92d99-241">**pages**</span><span class="sxs-lookup"><span data-stu-id="92d99-241">**pages**</span></span>         | <span data-ttu-id="92d99-242">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="92d99-242">Collection([sitePage][])</span></span>         | <span data-ttu-id="92d99-243">Коллекция страниц в списке SitePages на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="92d99-243">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="92d99-244">**permissions**</span><span class="sxs-lookup"><span data-stu-id="92d99-244">**permissions**</span></span>   | <span data-ttu-id="92d99-245">Collection([permission][])</span><span class="sxs-lookup"><span data-stu-id="92d99-245">Collection([permission][])</span></span>         | <span data-ttu-id="92d99-246">Разрешения, связанные с сайтом.</span><span class="sxs-lookup"><span data-stu-id="92d99-246">The permissions associated with the site.</span></span> <span data-ttu-id="92d99-247">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="92d99-247">Nullable.</span></span>
| <span data-ttu-id="92d99-248">**sites**</span><span class="sxs-lookup"><span data-stu-id="92d99-248">**sites**</span></span>         | <span data-ttu-id="92d99-249">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="92d99-249">Collection([site][])</span></span>             | <span data-ttu-id="92d99-250">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="92d99-250">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="92d99-251">**externalColumns**</span><span class="sxs-lookup"><span data-stu-id="92d99-251">**externalColumns**</span></span>     | <span data-ttu-id="92d99-252">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="92d99-252">Collection([columnDefinition][])</span></span>  | <span data-ttu-id="92d99-253">Коллекция определений столбцов, доступных на сайте, на которые ссылаются сайты в родительской иерархии текущего сайта.</span><span class="sxs-lookup"><span data-stu-id="92d99-253">The collection of column definitions available in the site that are referenced from the sites in the parent hierarchy of the current site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[permission]: permission.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="92d99-266">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92d99-266">JSON representation</span></span>

<span data-ttu-id="92d99-267">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92d99-267">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="92d99-268">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="92d99-268">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "permissions",
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
  "permissions": [ { "@odata.type": "microsoft.graph.permission" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "externalColumns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
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
