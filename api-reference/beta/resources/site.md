---
author: JeremyKelley
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 152100311e85dc905e14ca6f434a9a9fbe1d87fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155848"
---
# <a name="site-resource-type"></a><span data-ttu-id="f364c-103">Тип ресурса site</span><span class="sxs-lookup"><span data-stu-id="f364c-103">site resource type</span></span>

<span data-ttu-id="f364c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f364c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f364c-105">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f364c-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="f364c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f364c-106">Methods</span></span>

| <span data-ttu-id="f364c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f364c-107">Method</span></span>                         | <span data-ttu-id="f364c-108">Путь REST</span><span class="sxs-lookup"><span data-stu-id="f364c-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="f364c-109">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="f364c-109">[Get root site][]</span></span>              | <span data-ttu-id="f364c-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="f364c-110">GET /sites/root</span></span>
| <span data-ttu-id="f364c-111">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="f364c-111">[Get site][]</span></span>                   | <span data-ttu-id="f364c-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="f364c-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="f364c-113">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="f364c-113">[Get site by path][]</span></span>           | <span data-ttu-id="f364c-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="f364c-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="f364c-115">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="f364c-115">[Get site for a group][]</span></span>       | <span data-ttu-id="f364c-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="f364c-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="f364c-117">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="f364c-117">[Get analytics][]</span></span>              | <span data-ttu-id="f364c-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="f364c-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="f364c-119">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="f364c-119">[Get activities by interval][]</span></span> | <span data-ttu-id="f364c-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="f364c-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="f364c-121">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="f364c-121">[List pages][]</span></span>                 | <span data-ttu-id="f364c-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="f364c-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="f364c-123">[Перечисление корневых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="f364c-123">[List root sites][]</span></span>            | <span data-ttu-id="f364c-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="f364c-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="f364c-125">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="f364c-125">[Search for sites][]</span></span>           | <span data-ttu-id="f364c-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="f364c-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="f364c-127">[Отслеживание сайта][]</span><span class="sxs-lookup"><span data-stu-id="f364c-127">[Follow site][]</span></span>                | <span data-ttu-id="f364c-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="f364c-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="f364c-129">[Прекращение отслеживания сайта][]</span><span class="sxs-lookup"><span data-stu-id="f364c-129">[Unfollow site][]</span></span>              | <span data-ttu-id="f364c-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="f364c-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="f364c-131">[Перечисление отслеживаемых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="f364c-131">[List followed sites][]</span></span>        | <span data-ttu-id="f364c-132">GET /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="f364c-132">GET /me/followedSites</span></span>
| <span data-ttu-id="f364c-133">[Получение разрешения][]</span><span class="sxs-lookup"><span data-stu-id="f364c-133">[Get permission][]</span></span>             | <span data-ttu-id="f364c-134">GET /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="f364c-134">GET /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="f364c-135">[Список разрешений][]</span><span class="sxs-lookup"><span data-stu-id="f364c-135">[List permissions][]</span></span>           | <span data-ttu-id="f364c-136">GET /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="f364c-136">GET /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="f364c-137">[Создание разрешений][]</span><span class="sxs-lookup"><span data-stu-id="f364c-137">[Create permissions][]</span></span>         | <span data-ttu-id="f364c-138">POST /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="f364c-138">POST /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="f364c-139">[Удаление разрешения][]</span><span class="sxs-lookup"><span data-stu-id="f364c-139">[Delete permission][]</span></span>         | <span data-ttu-id="f364c-140">DELETE /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="f364c-140">DELETE /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="f364c-141">[Обновление разрешения][]</span><span class="sxs-lookup"><span data-stu-id="f364c-141">[Update permission][]</span></span>         | <span data-ttu-id="f364c-142">PATCH /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="f364c-142">PATCH /sites/{site-id}/permissions/{permission-id}</span></span>

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


## <a name="properties"></a><span data-ttu-id="f364c-160">Свойства</span><span class="sxs-lookup"><span data-stu-id="f364c-160">Properties</span></span>

| <span data-ttu-id="f364c-161">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f364c-161">Property name</span></span>            | <span data-ttu-id="f364c-162">Тип</span><span class="sxs-lookup"><span data-stu-id="f364c-162">Type</span></span>               | <span data-ttu-id="f364c-163">Описание</span><span class="sxs-lookup"><span data-stu-id="f364c-163">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="f364c-164">**id**</span><span class="sxs-lookup"><span data-stu-id="f364c-164">**id**</span></span>                   | <span data-ttu-id="f364c-165">string</span><span class="sxs-lookup"><span data-stu-id="f364c-165">string</span></span>             | <span data-ttu-id="f364c-166">[Уникальный идентификатор](#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="f364c-166">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="f364c-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f364c-167">Read-only.</span></span>
| <span data-ttu-id="f364c-168">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="f364c-168">**createdDateTime**</span></span>      | <span data-ttu-id="f364c-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f364c-169">DateTimeOffset</span></span>     | <span data-ttu-id="f364c-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f364c-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="f364c-172">**description**</span><span class="sxs-lookup"><span data-stu-id="f364c-172">**description**</span></span>          | <span data-ttu-id="f364c-173">string</span><span class="sxs-lookup"><span data-stu-id="f364c-173">string</span></span>             | <span data-ttu-id="f364c-174">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="f364c-174">The descriptive text for the site.</span></span>
| <span data-ttu-id="f364c-175">**eTag**</span><span class="sxs-lookup"><span data-stu-id="f364c-175">**eTag**</span></span>                 | <span data-ttu-id="f364c-176">string</span><span class="sxs-lookup"><span data-stu-id="f364c-176">string</span></span>             | <span data-ttu-id="f364c-p103">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f364c-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="f364c-179">**displayName**</span><span class="sxs-lookup"><span data-stu-id="f364c-179">**displayName**</span></span>          | <span data-ttu-id="f364c-180">string</span><span class="sxs-lookup"><span data-stu-id="f364c-180">string</span></span>             | <span data-ttu-id="f364c-p104">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f364c-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="f364c-183">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f364c-183">**lastModifiedDateTime**</span></span> | <span data-ttu-id="f364c-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f364c-184">DateTimeOffset</span></span>     | <span data-ttu-id="f364c-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f364c-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f364c-187">**name**</span><span class="sxs-lookup"><span data-stu-id="f364c-187">**name**</span></span>                 | <span data-ttu-id="f364c-188">string</span><span class="sxs-lookup"><span data-stu-id="f364c-188">string</span></span>             | <span data-ttu-id="f364c-189">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="f364c-189">The name / title of the item.</span></span>
| <span data-ttu-id="f364c-190">**root**</span><span class="sxs-lookup"><span data-stu-id="f364c-190">**root**</span></span>                 | <span data-ttu-id="f364c-191">[root][]</span><span class="sxs-lookup"><span data-stu-id="f364c-191">[root][]</span></span>           | <span data-ttu-id="f364c-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f364c-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="f364c-194">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="f364c-194">**sharepointIds**</span></span>        | <span data-ttu-id="f364c-195">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f364c-195">[sharepointIds][]</span></span>  | <span data-ttu-id="f364c-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f364c-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="f364c-198">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="f364c-198">**siteCollection**</span></span>       | <span data-ttu-id="f364c-199">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="f364c-199">[siteCollection][]</span></span> | <span data-ttu-id="f364c-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f364c-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="f364c-203">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="f364c-203">**webUrl**</span></span>               | <span data-ttu-id="f364c-204">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="f364c-204">string (url)</span></span>       | <span data-ttu-id="f364c-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f364c-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="f364c-207">Свойство id</span><span class="sxs-lookup"><span data-stu-id="f364c-207">id property</span></span>
<span data-ttu-id="f364c-208">Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="f364c-208">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="f364c-209">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="f364c-209">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="f364c-210">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="f364c-210">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="f364c-211">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="f364c-211">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="f364c-212">Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="f364c-212">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="f364c-213">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="f364c-213">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="f364c-214">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="f364c-214">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="f364c-215">Связи</span><span class="sxs-lookup"><span data-stu-id="f364c-215">Relationships</span></span>

| <span data-ttu-id="f364c-216">Имя связи</span><span class="sxs-lookup"><span data-stu-id="f364c-216">Relationship name</span></span> | <span data-ttu-id="f364c-217">Тип</span><span class="sxs-lookup"><span data-stu-id="f364c-217">Type</span></span>                             | <span data-ttu-id="f364c-218">Описание</span><span class="sxs-lookup"><span data-stu-id="f364c-218">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="f364c-219">**analytics**</span><span class="sxs-lookup"><span data-stu-id="f364c-219">**analytics**</span></span>     | <span data-ttu-id="f364c-220">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="f364c-220">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="f364c-221">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f364c-221">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="f364c-222">**columns**</span><span class="sxs-lookup"><span data-stu-id="f364c-222">**columns**</span></span>       | <span data-ttu-id="f364c-223">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="f364c-223">Collection([columnDefinition][])</span></span> | <span data-ttu-id="f364c-224">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f364c-224">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="f364c-225">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="f364c-225">**contentTypes**</span></span>  | <span data-ttu-id="f364c-226">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="f364c-226">Collection([contentType][])</span></span>      | <span data-ttu-id="f364c-227">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="f364c-227">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="f364c-228">**drive**</span><span class="sxs-lookup"><span data-stu-id="f364c-228">**drive**</span></span>         | <span data-ttu-id="f364c-229">[drive][]</span><span class="sxs-lookup"><span data-stu-id="f364c-229">[drive][]</span></span>                        | <span data-ttu-id="f364c-230">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="f364c-230">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="f364c-231">**drives**</span><span class="sxs-lookup"><span data-stu-id="f364c-231">**drives**</span></span>        | <span data-ttu-id="f364c-232">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="f364c-232">Collection([drive][])</span></span>            | <span data-ttu-id="f364c-233">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f364c-233">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="f364c-234">**items**</span><span class="sxs-lookup"><span data-stu-id="f364c-234">**items**</span></span>         | <span data-ttu-id="f364c-235">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="f364c-235">Collection([baseItem][])</span></span>         | <span data-ttu-id="f364c-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="f364c-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="f364c-238">**lists**</span><span class="sxs-lookup"><span data-stu-id="f364c-238">**lists**</span></span>         | <span data-ttu-id="f364c-239">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="f364c-239">Collection([list][])</span></span>             | <span data-ttu-id="f364c-240">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f364c-240">The collection of lists under this site.</span></span>
| <span data-ttu-id="f364c-241">**pages**</span><span class="sxs-lookup"><span data-stu-id="f364c-241">**pages**</span></span>         | <span data-ttu-id="f364c-242">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="f364c-242">Collection([sitePage][])</span></span>         | <span data-ttu-id="f364c-243">Коллекция страниц в списке SitePages на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="f364c-243">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="f364c-244">**permissions**</span><span class="sxs-lookup"><span data-stu-id="f364c-244">**permissions**</span></span>   | <span data-ttu-id="f364c-245">Collection([permission][])</span><span class="sxs-lookup"><span data-stu-id="f364c-245">Collection([permission][])</span></span>         | <span data-ttu-id="f364c-246">Разрешения, связанные с сайтом.</span><span class="sxs-lookup"><span data-stu-id="f364c-246">The permissions associated with the site.</span></span> <span data-ttu-id="f364c-247">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="f364c-247">Nullable.</span></span>
| <span data-ttu-id="f364c-248">**sites**</span><span class="sxs-lookup"><span data-stu-id="f364c-248">**sites**</span></span>         | <span data-ttu-id="f364c-249">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="f364c-249">Collection([site][])</span></span>             | <span data-ttu-id="f364c-250">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="f364c-250">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="f364c-263">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f364c-263">JSON representation</span></span>

<span data-ttu-id="f364c-264">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f364c-264">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="f364c-265">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="f364c-265">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
