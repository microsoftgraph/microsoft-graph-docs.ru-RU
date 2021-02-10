---
author: JeremyKelley
ms.author: JeremyKelley
title: Ресурс site
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f351ee2a9fe107ede3317a46789810ae2bf24b33
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161371"
---
# <a name="site-resource"></a><span data-ttu-id="ce002-103">Ресурс site</span><span class="sxs-lookup"><span data-stu-id="ce002-103">site resource</span></span>

<span data-ttu-id="ce002-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce002-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ce002-105">Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ce002-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="ce002-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ce002-106">Methods</span></span>

| <span data-ttu-id="ce002-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ce002-107">Method</span></span>                | <span data-ttu-id="ce002-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="ce002-108">Return type</span></span> | <span data-ttu-id="ce002-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ce002-109">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="ce002-110">[Получение корневого сайта][]</span><span class="sxs-lookup"><span data-stu-id="ce002-110">[Get root site][]</span></span>        | <span data-ttu-id="ce002-111">site</span><span class="sxs-lookup"><span data-stu-id="ce002-111">site</span></span> | <span data-ttu-id="ce002-112">Получение доступа к корневому сайту SharePoint внутри клиента.</span><span class="sxs-lookup"><span data-stu-id="ce002-112">Access the root SharePoint site within a tenant.</span></span>
| <span data-ttu-id="ce002-113">[Получение сайта][]</span><span class="sxs-lookup"><span data-stu-id="ce002-113">[Get site][]</span></span>             | <span data-ttu-id="ce002-114">site</span><span class="sxs-lookup"><span data-stu-id="ce002-114">site</span></span> | <span data-ttu-id="ce002-115">Получение доступа к сайту SharePoint с помощью параметра siteId.</span><span class="sxs-lookup"><span data-stu-id="ce002-115">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="ce002-116">[Получение сайта по пути][]</span><span class="sxs-lookup"><span data-stu-id="ce002-116">[Get site by path][]</span></span>     | <span data-ttu-id="ce002-117">site</span><span class="sxs-lookup"><span data-stu-id="ce002-117">site</span></span> | <span data-ttu-id="ce002-118">Получение доступа к корневому сайту SharePoint с использованием относительного пути.</span><span class="sxs-lookup"><span data-stu-id="ce002-118">Access the root SharePoint site with a relative path.</span></span>
| <span data-ttu-id="ce002-119">[Получение сайта для группы][]</span><span class="sxs-lookup"><span data-stu-id="ce002-119">[Get site for a group][]</span></span> | <span data-ttu-id="ce002-120">site</span><span class="sxs-lookup"><span data-stu-id="ce002-120">site</span></span> | <span data-ttu-id="ce002-121">Получение доступа к сайту группы для группы.</span><span class="sxs-lookup"><span data-stu-id="ce002-121">Access the team site for a group.</span></span>
| <span data-ttu-id="ce002-122">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="ce002-122">[Get analytics][]</span></span>              | <span data-ttu-id="ce002-123">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="ce002-123">[itemAnalytics][]</span></span> | <span data-ttu-id="ce002-124">Получение аналитических данных для ресурса.</span><span class="sxs-lookup"><span data-stu-id="ce002-124">Get analytics for this resource.</span></span> 
| <span data-ttu-id="ce002-125">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="ce002-125">[Get activities by interval][]</span></span> | <span data-ttu-id="ce002-126">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="ce002-126">[itemActivityStat][]</span></span> | <span data-ttu-id="ce002-127">Получение коллекции объектов **itemActivityStats** в пределах указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="ce002-127">Get a collection of **itemActivityStats** within the specified time interval.</span></span>
| <span data-ttu-id="ce002-128">[Поиск сайтов][]</span><span class="sxs-lookup"><span data-stu-id="ce002-128">[Search for sites][]</span></span>     | <span data-ttu-id="ce002-129">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="ce002-129">collection of site</span></span> | <span data-ttu-id="ce002-130">Поиск сайтов, соответствующих указанным ключевым словам, в клиенте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ce002-130">Search across a SharePoint tenant for sites that match keywords provided.</span></span>
| <span data-ttu-id="ce002-131">[Отслеживание сайта][]</span><span class="sxs-lookup"><span data-stu-id="ce002-131">[Follow site][]</span></span>          | <span data-ttu-id="ce002-132">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="ce002-132">collection of site</span></span> | <span data-ttu-id="ce002-133">Отслеживание сайта пользователя или нескольких сайтов.</span><span class="sxs-lookup"><span data-stu-id="ce002-133">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="ce002-134">[Прекращение отслеживания сайта][]</span><span class="sxs-lookup"><span data-stu-id="ce002-134">[Unfollow site][]</span></span>        | <span data-ttu-id="ce002-135">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="ce002-135">collection of site</span></span> | <span data-ttu-id="ce002-136">Отслеживание сайта пользователя или нескольких сайтов.</span><span class="sxs-lookup"><span data-stu-id="ce002-136">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="ce002-137">[Перечисление отслеживаемых сайтов][]</span><span class="sxs-lookup"><span data-stu-id="ce002-137">[List followed sites][]</span></span>  | <span data-ttu-id="ce002-138">коллекция сайтов</span><span class="sxs-lookup"><span data-stu-id="ce002-138">collection of site</span></span> | <span data-ttu-id="ce002-139">Перечисление сайтов, отслеживаемых вошедшим пользователем.</span><span class="sxs-lookup"><span data-stu-id="ce002-139">List the sites that have been followed by the signed in user.</span></span>
| <span data-ttu-id="ce002-140">[Получение разрешения][]</span><span class="sxs-lookup"><span data-stu-id="ce002-140">[Get permission][]</span></span>             | <span data-ttu-id="ce002-141">GET /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="ce002-141">GET /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="ce002-142">[Список разрешений][]</span><span class="sxs-lookup"><span data-stu-id="ce002-142">[List permissions][]</span></span>           | <span data-ttu-id="ce002-143">GET /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="ce002-143">GET /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="ce002-144">[Создание разрешений][]</span><span class="sxs-lookup"><span data-stu-id="ce002-144">[Create permissions][]</span></span>         | <span data-ttu-id="ce002-145">POST /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="ce002-145">POST /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="ce002-146">[Удаление разрешения][]</span><span class="sxs-lookup"><span data-stu-id="ce002-146">[Delete permission][]</span></span>         | <span data-ttu-id="ce002-147">DELETE /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="ce002-147">DELETE /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="ce002-148">[Обновление разрешения][]</span><span class="sxs-lookup"><span data-stu-id="ce002-148">[Update permission][]</span></span>         | <span data-ttu-id="ce002-149">PATCH /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="ce002-149">PATCH /sites/{site-id}/permissions/{permission-id}</span></span>

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

## <a name="properties"></a><span data-ttu-id="ce002-166">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce002-166">Properties</span></span>

| <span data-ttu-id="ce002-167">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce002-167">Property</span></span>            | <span data-ttu-id="ce002-168">Тип</span><span class="sxs-lookup"><span data-stu-id="ce002-168">Type</span></span>                                | <span data-ttu-id="ce002-169">Описание</span><span class="sxs-lookup"><span data-stu-id="ce002-169">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ce002-170">**id**</span><span class="sxs-lookup"><span data-stu-id="ce002-170">**id**</span></span>                   | <span data-ttu-id="ce002-171">string</span><span class="sxs-lookup"><span data-stu-id="ce002-171">string</span></span>                              | <span data-ttu-id="ce002-p101">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce002-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="ce002-174">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ce002-174">**createdDateTime**</span></span>      | <span data-ttu-id="ce002-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce002-175">DateTimeOffset</span></span>                      | <span data-ttu-id="ce002-p102">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce002-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="ce002-178">**description**</span><span class="sxs-lookup"><span data-stu-id="ce002-178">**description**</span></span>          | <span data-ttu-id="ce002-179">string</span><span class="sxs-lookup"><span data-stu-id="ce002-179">string</span></span>                              | <span data-ttu-id="ce002-180">Текст с описанием сайта.</span><span class="sxs-lookup"><span data-stu-id="ce002-180">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="ce002-181">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ce002-181">**displayName**</span></span>          | <span data-ttu-id="ce002-182">string</span><span class="sxs-lookup"><span data-stu-id="ce002-182">string</span></span>                              | <span data-ttu-id="ce002-p103">Полное название сайта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce002-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="ce002-185">**eTag**</span><span class="sxs-lookup"><span data-stu-id="ce002-185">**eTag**</span></span>                 | <span data-ttu-id="ce002-186">string</span><span class="sxs-lookup"><span data-stu-id="ce002-186">string</span></span>                              | <span data-ttu-id="ce002-p104">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce002-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="ce002-189">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ce002-189">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ce002-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce002-190">DateTimeOffset</span></span>                      | <span data-ttu-id="ce002-p105">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce002-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="ce002-193">**name**</span><span class="sxs-lookup"><span data-stu-id="ce002-193">**name**</span></span>                 | <span data-ttu-id="ce002-194">string</span><span class="sxs-lookup"><span data-stu-id="ce002-194">string</span></span>                              | <span data-ttu-id="ce002-195">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="ce002-195">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="ce002-196">**root**</span><span class="sxs-lookup"><span data-stu-id="ce002-196">**root**</span></span>                 | [<span data-ttu-id="ce002-197">root</span><span class="sxs-lookup"><span data-stu-id="ce002-197">root</span></span>](root.md)                     | <span data-ttu-id="ce002-p106">Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce002-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="ce002-200">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="ce002-200">**sharepointIds**</span></span>        | [<span data-ttu-id="ce002-201">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ce002-201">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="ce002-p107">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce002-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="ce002-204">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="ce002-204">**siteCollection**</span></span>       | [<span data-ttu-id="ce002-205">siteCollection</span><span class="sxs-lookup"><span data-stu-id="ce002-205">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="ce002-p108">Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce002-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="ce002-209">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="ce002-209">**webUrl**</span></span>               | <span data-ttu-id="ce002-210">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="ce002-210">string (url)</span></span>                        | <span data-ttu-id="ce002-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce002-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

### <a name="id-property"></a><span data-ttu-id="ce002-213">Свойство id</span><span class="sxs-lookup"><span data-stu-id="ce002-213">id property</span></span>
<span data-ttu-id="ce002-214">Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="ce002-214">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="ce002-215">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="ce002-215">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="ce002-216">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="ce002-216">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="ce002-217">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="ce002-217">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="ce002-218">Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="ce002-218">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="ce002-219">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="ce002-219">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="ce002-220">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="ce002-220">`/groups/{group-id}/sites/root`: The group's team site.</span></span>
  
## <a name="relationships"></a><span data-ttu-id="ce002-221">Связи</span><span class="sxs-lookup"><span data-stu-id="ce002-221">Relationships</span></span>

| <span data-ttu-id="ce002-222">Связь</span><span class="sxs-lookup"><span data-stu-id="ce002-222">Relationship</span></span>      | <span data-ttu-id="ce002-223">Тип</span><span class="sxs-lookup"><span data-stu-id="ce002-223">Type</span></span>                             | <span data-ttu-id="ce002-224">Описание</span><span class="sxs-lookup"><span data-stu-id="ce002-224">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="ce002-225">**analytics**</span><span class="sxs-lookup"><span data-stu-id="ce002-225">**analytics**</span></span>     | <span data-ttu-id="ce002-226">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="ce002-226">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="ce002-227">Аналитические данные о действиях просмотра, выполненных на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ce002-227">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="ce002-228">**columns**</span><span class="sxs-lookup"><span data-stu-id="ce002-228">**columns**</span></span>       | <span data-ttu-id="ce002-229">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="ce002-229">Collection([columnDefinition][])</span></span> | <span data-ttu-id="ce002-230">Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ce002-230">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="ce002-231">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="ce002-231">**contentTypes**</span></span>  | <span data-ttu-id="ce002-232">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="ce002-232">Collection([contentType][])</span></span>      | <span data-ttu-id="ce002-233">Коллекция типов контента, определенных для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="ce002-233">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="ce002-234">**drive**</span><span class="sxs-lookup"><span data-stu-id="ce002-234">**drive**</span></span>         | <span data-ttu-id="ce002-235">[drive][]</span><span class="sxs-lookup"><span data-stu-id="ce002-235">[drive][]</span></span>                        | <span data-ttu-id="ce002-236">Диск по умолчанию (библиотека документов) для этого сайта.</span><span class="sxs-lookup"><span data-stu-id="ce002-236">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="ce002-237">**drives**</span><span class="sxs-lookup"><span data-stu-id="ce002-237">**drives**</span></span>        | <span data-ttu-id="ce002-238">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="ce002-238">Collection([drive][])</span></span>            | <span data-ttu-id="ce002-239">Коллекция дисков (библиотек документов) на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ce002-239">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="ce002-240">**items**</span><span class="sxs-lookup"><span data-stu-id="ce002-240">**items**</span></span>         | <span data-ttu-id="ce002-241">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="ce002-241">Collection([baseItem][])</span></span>         | <span data-ttu-id="ce002-p110">Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="ce002-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="ce002-244">**lists**</span><span class="sxs-lookup"><span data-stu-id="ce002-244">**lists**</span></span>         | <span data-ttu-id="ce002-245">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="ce002-245">Collection([list][])</span></span>             | <span data-ttu-id="ce002-246">Коллекция списков на этом сайте.</span><span class="sxs-lookup"><span data-stu-id="ce002-246">The collection of lists under this site.</span></span>
| <span data-ttu-id="ce002-247">**permissions**</span><span class="sxs-lookup"><span data-stu-id="ce002-247">**permissions**</span></span>   | <span data-ttu-id="ce002-248">Collection([permission][])</span><span class="sxs-lookup"><span data-stu-id="ce002-248">Collection([permission][])</span></span>         | <span data-ttu-id="ce002-249">Разрешения, связанные с сайтом.</span><span class="sxs-lookup"><span data-stu-id="ce002-249">The permissions associated with the site.</span></span> <span data-ttu-id="ce002-250">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="ce002-250">Nullable.</span></span>
| <span data-ttu-id="ce002-251">**sites**</span><span class="sxs-lookup"><span data-stu-id="ce002-251">**sites**</span></span>         | <span data-ttu-id="ce002-252">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="ce002-252">Collection([site][])</span></span>             | <span data-ttu-id="ce002-253">Коллекция дочерних сайтов этого сайта.</span><span class="sxs-lookup"><span data-stu-id="ce002-253">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="ce002-254">**onenote**</span><span class="sxs-lookup"><span data-stu-id="ce002-254">**onenote**</span></span>       | <span data-ttu-id="ce002-255">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="ce002-255">[onenote][]</span></span>                      | <span data-ttu-id="ce002-256">Вызывает службу OneNote для выполнения операций, связанных с записными книжками.</span><span class="sxs-lookup"><span data-stu-id="ce002-256">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[permission]: permission.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="ce002-266">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce002-266">JSON representation</span></span>

<span data-ttu-id="ce002-267">Ниже показано представление ресурса **site** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce002-267">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="ce002-268">Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="ce002-268">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
