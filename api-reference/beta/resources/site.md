---
author: JeremyKelley
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: a8cab7859c68224acc734a88f941a952ca82798b
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51472116"
---
# <a name="site-resource-type"></a><span data-ttu-id="6ab89-103">Тип ресурса site</span><span class="sxs-lookup"><span data-stu-id="6ab89-103">site resource type</span></span>

<span data-ttu-id="6ab89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ab89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ab89-105">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6ab89-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="6ab89-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6ab89-106">Methods</span></span>

| <span data-ttu-id="6ab89-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6ab89-107">Method</span></span>                         | <span data-ttu-id="6ab89-108">Путь REST</span><span class="sxs-lookup"><span data-stu-id="6ab89-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="6ab89-109">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-109">[Get root site][]</span></span>              | <span data-ttu-id="6ab89-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="6ab89-110">GET /sites/root</span></span>
| <span data-ttu-id="6ab89-111">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-111">[Get site][]</span></span>                   | <span data-ttu-id="6ab89-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="6ab89-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="6ab89-113">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-113">[Get site by path][]</span></span>           | <span data-ttu-id="6ab89-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="6ab89-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="6ab89-115">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-115">[Get site for a group][]</span></span>       | <span data-ttu-id="6ab89-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="6ab89-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="6ab89-117">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-117">[Get analytics][]</span></span>              | <span data-ttu-id="6ab89-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="6ab89-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="6ab89-119">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-119">[Get activities by interval][]</span></span> | <span data-ttu-id="6ab89-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="6ab89-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="6ab89-121">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-121">[List pages][]</span></span>                 | <span data-ttu-id="6ab89-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="6ab89-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="6ab89-123">[Перечисление корневых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-123">[List root sites][]</span></span>            | <span data-ttu-id="6ab89-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="6ab89-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="6ab89-125">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-125">[Search for sites][]</span></span>           | <span data-ttu-id="6ab89-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="6ab89-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="6ab89-127">[Отслеживание сайта][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-127">[Follow site][]</span></span>                | <span data-ttu-id="6ab89-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="6ab89-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="6ab89-129">[Прекращение отслеживания сайта][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-129">[Unfollow site][]</span></span>              | <span data-ttu-id="6ab89-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="6ab89-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="6ab89-131">[Перечисление отслеживаемых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-131">[List followed sites][]</span></span>        | <span data-ttu-id="6ab89-132">GET /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="6ab89-132">GET /me/followedSites</span></span>
| <span data-ttu-id="6ab89-133">[Получение разрешения][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-133">[Get permission][]</span></span>             | <span data-ttu-id="6ab89-134">GET /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="6ab89-134">GET /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="6ab89-135">[Список разрешений][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-135">[List permissions][]</span></span>           | <span data-ttu-id="6ab89-136">GET /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="6ab89-136">GET /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="6ab89-137">[Создание разрешений][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-137">[Create permissions][]</span></span>         | <span data-ttu-id="6ab89-138">POST /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="6ab89-138">POST /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="6ab89-139">[Удаление разрешения][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-139">[Delete permission][]</span></span>         | <span data-ttu-id="6ab89-140">DELETE /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="6ab89-140">DELETE /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="6ab89-141">[Обновление разрешения][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-141">[Update permission][]</span></span>         | <span data-ttu-id="6ab89-142">PATCH /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="6ab89-142">PATCH /sites/{site-id}/permissions/{permission-id}</span></span>
|<span data-ttu-id="6ab89-143">[Перечисление типов контента][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-143">[List content types][]</span></span>          | <span data-ttu-id="6ab89-144">GET /sites/{site-id}/contentTypes</span><span class="sxs-lookup"><span data-stu-id="6ab89-144">GET /sites/{site-id}/contentTypes</span></span>
|<span data-ttu-id="6ab89-145">[Создание contentType][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-145">[Create contentType][]</span></span>        | <span data-ttu-id="6ab89-146">POST /sites/{site-id}/contentTypes</span><span class="sxs-lookup"><span data-stu-id="6ab89-146">POST /sites/{site-id}/contentTypes</span></span>
|<span data-ttu-id="6ab89-147">[Перечисление столбцов][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-147">[List columns][]</span></span>               | <span data-ttu-id="6ab89-148">GET /sites/{site-id}/columns</span><span class="sxs-lookup"><span data-stu-id="6ab89-148">GET /sites/{site-id}/columns</span></span>
|<span data-ttu-id="6ab89-149">[Создание столбца][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-149">[Create column][]</span></span>              | <span data-ttu-id="6ab89-150">POST /sites/{site-id}/columns</span><span class="sxs-lookup"><span data-stu-id="6ab89-150">POST /sites/{site-id}/columns</span></span>

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
[Перечисление типов контента]: ../api/site-list-contenttypes.md
[List content types]: ../api/site-list-contenttypes.md
[Создание contentType]: ../api/site-post-contenttypes.md
[Create contentType]: ../api/site-post-contenttypes.md
[Перечисление столбцов]: ../api/site-list-columns.md
[List columns]: ../api/site-list-columns.md
[Создание столбца]: ../api/site-post-columns.md
[Create column]: ../api/site-post-columns.md


## <a name="properties"></a><span data-ttu-id="6ab89-172">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ab89-172">Properties</span></span>

| <span data-ttu-id="6ab89-173">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6ab89-173">Property name</span></span>            | <span data-ttu-id="6ab89-174">Тип</span><span class="sxs-lookup"><span data-stu-id="6ab89-174">Type</span></span>               | <span data-ttu-id="6ab89-175">Описание</span><span class="sxs-lookup"><span data-stu-id="6ab89-175">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="6ab89-176">**id**</span><span class="sxs-lookup"><span data-stu-id="6ab89-176">**id**</span></span>                   | <span data-ttu-id="6ab89-177">string</span><span class="sxs-lookup"><span data-stu-id="6ab89-177">string</span></span>             | <span data-ttu-id="6ab89-178">[Уникальный идентификатор](#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="6ab89-178">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="6ab89-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ab89-179">Read-only.</span></span>
| <span data-ttu-id="6ab89-180">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="6ab89-180">**createdDateTime**</span></span>      | <span data-ttu-id="6ab89-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ab89-181">DateTimeOffset</span></span>     | <span data-ttu-id="6ab89-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ab89-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="6ab89-184">**description**</span><span class="sxs-lookup"><span data-stu-id="6ab89-184">**description**</span></span>          | <span data-ttu-id="6ab89-185">string</span><span class="sxs-lookup"><span data-stu-id="6ab89-185">string</span></span>             | <span data-ttu-id="6ab89-186">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="6ab89-186">The descriptive text for the site.</span></span>
| <span data-ttu-id="6ab89-187">**eTag**</span><span class="sxs-lookup"><span data-stu-id="6ab89-187">**eTag**</span></span>                 | <span data-ttu-id="6ab89-188">string</span><span class="sxs-lookup"><span data-stu-id="6ab89-188">string</span></span>             | <span data-ttu-id="6ab89-p103">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ab89-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="6ab89-191">**displayName**</span><span class="sxs-lookup"><span data-stu-id="6ab89-191">**displayName**</span></span>          | <span data-ttu-id="6ab89-192">string</span><span class="sxs-lookup"><span data-stu-id="6ab89-192">string</span></span>             | <span data-ttu-id="6ab89-p104">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ab89-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="6ab89-195">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="6ab89-195">**lastModifiedDateTime**</span></span> | <span data-ttu-id="6ab89-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ab89-196">DateTimeOffset</span></span>     | <span data-ttu-id="6ab89-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ab89-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="6ab89-199">**name**</span><span class="sxs-lookup"><span data-stu-id="6ab89-199">**name**</span></span>                 | <span data-ttu-id="6ab89-200">string</span><span class="sxs-lookup"><span data-stu-id="6ab89-200">string</span></span>             | <span data-ttu-id="6ab89-201">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="6ab89-201">The name / title of the item.</span></span>
| <span data-ttu-id="6ab89-202">**root**</span><span class="sxs-lookup"><span data-stu-id="6ab89-202">**root**</span></span>                 | <span data-ttu-id="6ab89-203">[root][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-203">[root][]</span></span>           | <span data-ttu-id="6ab89-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ab89-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="6ab89-206">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="6ab89-206">**sharepointIds**</span></span>        | <span data-ttu-id="6ab89-207">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-207">[sharepointIds][]</span></span>  | <span data-ttu-id="6ab89-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ab89-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="6ab89-210">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="6ab89-210">**siteCollection**</span></span>       | <span data-ttu-id="6ab89-211">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-211">[siteCollection][]</span></span> | <span data-ttu-id="6ab89-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ab89-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="6ab89-215">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="6ab89-215">**webUrl**</span></span>               | <span data-ttu-id="6ab89-216">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="6ab89-216">string (url)</span></span>       | <span data-ttu-id="6ab89-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ab89-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="6ab89-219">Свойство id</span><span class="sxs-lookup"><span data-stu-id="6ab89-219">id property</span></span>
<span data-ttu-id="6ab89-220">Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="6ab89-220">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="6ab89-221">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="6ab89-221">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="6ab89-222">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="6ab89-222">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="6ab89-223">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="6ab89-223">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="6ab89-224">Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="6ab89-224">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="6ab89-225">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="6ab89-225">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="6ab89-226">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="6ab89-226">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="6ab89-227">Связи</span><span class="sxs-lookup"><span data-stu-id="6ab89-227">Relationships</span></span>

| <span data-ttu-id="6ab89-228">Имя связи</span><span class="sxs-lookup"><span data-stu-id="6ab89-228">Relationship name</span></span> | <span data-ttu-id="6ab89-229">Тип</span><span class="sxs-lookup"><span data-stu-id="6ab89-229">Type</span></span>                             | <span data-ttu-id="6ab89-230">Описание</span><span class="sxs-lookup"><span data-stu-id="6ab89-230">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="6ab89-231">**analytics**</span><span class="sxs-lookup"><span data-stu-id="6ab89-231">**analytics**</span></span>     | <span data-ttu-id="6ab89-232">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-232">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="6ab89-233">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="6ab89-233">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="6ab89-234">**columns**</span><span class="sxs-lookup"><span data-stu-id="6ab89-234">**columns**</span></span>       | <span data-ttu-id="6ab89-235">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="6ab89-235">Collection([columnDefinition][])</span></span> | <span data-ttu-id="6ab89-236">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="6ab89-236">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="6ab89-237">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="6ab89-237">**contentTypes**</span></span>  | <span data-ttu-id="6ab89-238">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="6ab89-238">Collection([contentType][])</span></span>      | <span data-ttu-id="6ab89-239">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="6ab89-239">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="6ab89-240">**drive**</span><span class="sxs-lookup"><span data-stu-id="6ab89-240">**drive**</span></span>         | <span data-ttu-id="6ab89-241">[drive][]</span><span class="sxs-lookup"><span data-stu-id="6ab89-241">[drive][]</span></span>                        | <span data-ttu-id="6ab89-242">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="6ab89-242">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="6ab89-243">**drives**</span><span class="sxs-lookup"><span data-stu-id="6ab89-243">**drives**</span></span>        | <span data-ttu-id="6ab89-244">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="6ab89-244">Collection([drive][])</span></span>            | <span data-ttu-id="6ab89-245">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="6ab89-245">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="6ab89-246">**items**</span><span class="sxs-lookup"><span data-stu-id="6ab89-246">**items**</span></span>         | <span data-ttu-id="6ab89-247">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="6ab89-247">Collection([baseItem][])</span></span>         | <span data-ttu-id="6ab89-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="6ab89-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="6ab89-250">**lists**</span><span class="sxs-lookup"><span data-stu-id="6ab89-250">**lists**</span></span>         | <span data-ttu-id="6ab89-251">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="6ab89-251">Collection([list][])</span></span>             | <span data-ttu-id="6ab89-252">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="6ab89-252">The collection of lists under this site.</span></span>
| <span data-ttu-id="6ab89-253">**pages**</span><span class="sxs-lookup"><span data-stu-id="6ab89-253">**pages**</span></span>         | <span data-ttu-id="6ab89-254">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="6ab89-254">Collection([sitePage][])</span></span>         | <span data-ttu-id="6ab89-255">Коллекция страниц в списке SitePages на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="6ab89-255">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="6ab89-256">**permissions**</span><span class="sxs-lookup"><span data-stu-id="6ab89-256">**permissions**</span></span>   | <span data-ttu-id="6ab89-257">Collection([permission][])</span><span class="sxs-lookup"><span data-stu-id="6ab89-257">Collection([permission][])</span></span>         | <span data-ttu-id="6ab89-258">Разрешения, связанные с сайтом.</span><span class="sxs-lookup"><span data-stu-id="6ab89-258">The permissions associated with the site.</span></span> <span data-ttu-id="6ab89-259">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="6ab89-259">Nullable.</span></span>
| <span data-ttu-id="6ab89-260">**sites**</span><span class="sxs-lookup"><span data-stu-id="6ab89-260">**sites**</span></span>         | <span data-ttu-id="6ab89-261">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="6ab89-261">Collection([site][])</span></span>             | <span data-ttu-id="6ab89-262">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="6ab89-262">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="6ab89-263">**termStore**</span><span class="sxs-lookup"><span data-stu-id="6ab89-263">**termStore**</span></span>     | <span data-ttu-id="6ab89-264">[microsoft.graph.termStore.store]</span><span class="sxs-lookup"><span data-stu-id="6ab89-264">[microsoft.graph.termStore.store]</span></span>  | <span data-ttu-id="6ab89-265">TermStore на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="6ab89-265">The termStore under this site.</span></span>
| <span data-ttu-id="6ab89-266">**externalColumns**</span><span class="sxs-lookup"><span data-stu-id="6ab89-266">**externalColumns**</span></span>     | <span data-ttu-id="6ab89-267">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="6ab89-267">Collection([columnDefinition][])</span></span>  | <span data-ttu-id="6ab89-268">Коллекция определений столбцов, доступных на сайте, на которые ссылаются сайты в родительской иерархии текущего сайта.</span><span class="sxs-lookup"><span data-stu-id="6ab89-268">The collection of column definitions available in the site that are referenced from the sites in the parent hierarchy of the current site.</span></span>

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
[microsoft.graph.termStore.store]: termstore-store.md

## <a name="json-representation"></a><span data-ttu-id="6ab89-282">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ab89-282">JSON representation</span></span>

<span data-ttu-id="6ab89-283">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ab89-283">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="6ab89-284">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="6ab89-284">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "termStore": { "@odata.type": "microsoft.graph.termStore.store" },
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
