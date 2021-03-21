---
author: JeremyKelley
description: Ресурс list представляет список на сайте.
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9bc255a0bcddadbbf9190decc2d429eb88e91e67
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964563"
---
# <a name="list-resource"></a><span data-ttu-id="3cb20-103">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="3cb20-103">List resource</span></span>

<span data-ttu-id="3cb20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cb20-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cb20-105">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="3cb20-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="3cb20-106">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="3cb20-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="3cb20-107">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="3cb20-107">Tasks on a list</span></span>

<span data-ttu-id="3cb20-108">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="3cb20-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="3cb20-109">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="3cb20-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="3cb20-110">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="3cb20-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="3cb20-111">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="3cb20-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="3cb20-112">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="3cb20-112">Common task</span></span>               | <span data-ttu-id="3cb20-113">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="3cb20-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="3cb20-114">[Получить списки на сайте][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-114">[Get lists in a site][]</span></span>   | <span data-ttu-id="3cb20-115">GET /sites/{site-id}/lists</span><span class="sxs-lookup"><span data-stu-id="3cb20-115">GET /sites/{site-id}/lists</span></span>
| <span data-ttu-id="3cb20-116">[Создание списка][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-116">[Create list][]</span></span>           | <span data-ttu-id="3cb20-117">POST /lists</span><span class="sxs-lookup"><span data-stu-id="3cb20-117">POST /lists</span></span>
| <span data-ttu-id="3cb20-118">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-118">[Get list][]</span></span>              | <span data-ttu-id="3cb20-119">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="3cb20-119">GET /lists/{list-id}</span></span>
| <span data-ttu-id="3cb20-120">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-120">[Enumerate list items][]</span></span>  | <span data-ttu-id="3cb20-121">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="3cb20-121">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="3cb20-122">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-122">[Update list item][]</span></span>      | <span data-ttu-id="3cb20-123">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="3cb20-123">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="3cb20-124">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-124">[Delete list item][]</span></span>      | <span data-ttu-id="3cb20-125">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="3cb20-125">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="3cb20-126">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-126">[Create list item][]</span></span>      | <span data-ttu-id="3cb20-127">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="3cb20-127">POST /lists/{list-id}</span></span>
| <span data-ttu-id="3cb20-128">[Получение последних действий][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-128">[Get recent activities][]</span></span> | <span data-ttu-id="3cb20-129">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="3cb20-129">GET /lists/{list-id}/activities</span></span>
| <span data-ttu-id="3cb20-130">[Получение канала WebSocket][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-130">[Get WebSocket channel][]</span></span> | <span data-ttu-id="3cb20-131">GET /lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="3cb20-131">GET /lists/{list-id}/subscriptions/socketIo</span></span>
|<span data-ttu-id="3cb20-132">[Типы содержимого списка][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-132">[List content types][]</span></span>          | <span data-ttu-id="3cb20-133">GET /lists/{list-id}/contentTypes</span><span class="sxs-lookup"><span data-stu-id="3cb20-133">GET /lists/{list-id}/contentTypes</span></span>
|<span data-ttu-id="3cb20-134">[Добавление копии типа контента с сайта][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-134">[Add copy of content type from site][]</span></span> | <span data-ttu-id="3cb20-135">POST /lists/{list-id}/contentTypes/addCopy</span><span class="sxs-lookup"><span data-stu-id="3cb20-135">POST /lists/{list-id}/contentTypes/addCopy</span></span>
|<span data-ttu-id="3cb20-136">[Список столбцов][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-136">[List columns][]</span></span>               | <span data-ttu-id="3cb20-137">GET /lists/{list-id}/columns</span><span class="sxs-lookup"><span data-stu-id="3cb20-137">GET /lists/{list-id}/columns</span></span>
|<span data-ttu-id="3cb20-138">[Создание столбца][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-138">[Create column][]</span></span>              | <span data-ttu-id="3cb20-139">POST /lists/{list-id}/columns</span><span class="sxs-lookup"><span data-stu-id="3cb20-139">POST /lists/{list-id}/columns</span></span>

[Получить списки на сайте]: ../api/list-list.md
[Get lists in a site]: ../api/list-list.md
[Получение списка]: ../api/list-get.md
[Get list]: ../api/list-get.md
[Создание списка]: ../api/list-create.md
[Create list]: ../api/list-create.md
[Перечисление элементов списка]: ../api/listitem-list.md
[Enumerate list items]: ../api/listitem-list.md
[Обновление элемента списка]: ../api/listitem-update.md
[Update list item]: ../api/listitem-update.md
[Удаление элемента списка]: ../api/listitem-delete.md
[Delete list item]: ../api/listitem-delete.md
[Создание элемента в списке]: ../api/listitem-create.md
[Create list item]: ../api/listitem-create.md
[Получение последних действий]: ../api/activities-list.md
[Get recent activities]: ../api/activities-list.md
[Получение канала WebSocket]: ../api/subscriptions-socketio.md
[Get WebSocket channel]: ../api/subscriptions-socketio.md
[Типы содержимого списка]: ../api/list-list-contenttypes.md
[List content types]: ../api/list-list-contenttypes.md
[Добавление копии типа контента с сайта]: ../api/contenttype-addCopy.md
[Add copy of content type from site]: ../api/contenttype-addCopy.md
[Список столбцов]: ../api/list-list-columns.md
[List columns]: ../api/list-list-columns.md
[Создание столбца]: ../api/list-post-columns.md
[Create column]: ../api/list-post-columns.md
## <a name="json-representation"></a><span data-ttu-id="3cb20-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3cb20-153">JSON representation</span></span>

<span data-ttu-id="3cb20-154">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cb20-154">Here is a JSON representation of a **list** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template": "documentLibrary | genericList | survey | links | announcements | contacts ..."
  },
  "system": false,
  "subscriptions": [ {"@odata.type": "microsoft.graph.subscription"} ],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of list",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of list",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="3cb20-155">Свойства</span><span class="sxs-lookup"><span data-stu-id="3cb20-155">Properties</span></span>

<span data-ttu-id="3cb20-156">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="3cb20-156">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="3cb20-157">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="3cb20-157">Property name</span></span>    | <span data-ttu-id="3cb20-158">Тип</span><span class="sxs-lookup"><span data-stu-id="3cb20-158">Type</span></span>                             | <span data-ttu-id="3cb20-159">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb20-159">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="3cb20-160">**columns**</span><span class="sxs-lookup"><span data-stu-id="3cb20-160">**columns**</span></span>      | <span data-ttu-id="3cb20-161">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="3cb20-161">Collection([columnDefinition][])</span></span> | <span data-ttu-id="3cb20-162">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="3cb20-162">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="3cb20-163">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="3cb20-163">**contentTypes**</span></span> | <span data-ttu-id="3cb20-164">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="3cb20-164">Collection([contentType][])</span></span>      | <span data-ttu-id="3cb20-165">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="3cb20-165">The collection of content types present in this list.</span></span>
| <span data-ttu-id="3cb20-166">**displayName**</span><span class="sxs-lookup"><span data-stu-id="3cb20-166">**displayName**</span></span>  | <span data-ttu-id="3cb20-167">строка</span><span class="sxs-lookup"><span data-stu-id="3cb20-167">string</span></span>                           | <span data-ttu-id="3cb20-168">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="3cb20-168">The displayable title of the list.</span></span>
| <span data-ttu-id="3cb20-169">**list**</span><span class="sxs-lookup"><span data-stu-id="3cb20-169">**list**</span></span>         | <span data-ttu-id="3cb20-170">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-170">[listInfo][]</span></span>                     | <span data-ttu-id="3cb20-171">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="3cb20-171">Provides additional details about the list.</span></span>
| <span data-ttu-id="3cb20-172">**system**</span><span class="sxs-lookup"><span data-stu-id="3cb20-172">**system**</span></span>       | <span data-ttu-id="3cb20-173">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-173">[systemFacet][]</span></span>                  | <span data-ttu-id="3cb20-174">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="3cb20-174">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="3cb20-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cb20-175">Read-only.</span></span>

<span data-ttu-id="3cb20-176">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="3cb20-176">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="3cb20-177">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="3cb20-177">Property name</span></span>            | <span data-ttu-id="3cb20-178">Тип</span><span class="sxs-lookup"><span data-stu-id="3cb20-178">Type</span></span>             | <span data-ttu-id="3cb20-179">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb20-179">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="3cb20-180">**id**</span><span class="sxs-lookup"><span data-stu-id="3cb20-180">**id**</span></span>                   | <span data-ttu-id="3cb20-181">string</span><span class="sxs-lookup"><span data-stu-id="3cb20-181">string</span></span>           | <span data-ttu-id="3cb20-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cb20-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="3cb20-184">**name**</span><span class="sxs-lookup"><span data-stu-id="3cb20-184">**name**</span></span>                 | <span data-ttu-id="3cb20-185">строка</span><span class="sxs-lookup"><span data-stu-id="3cb20-185">string</span></span>           | <span data-ttu-id="3cb20-186">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="3cb20-186">The name of the item.</span></span>
| <span data-ttu-id="3cb20-187">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="3cb20-187">**createdBy**</span></span>            | <span data-ttu-id="3cb20-188">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-188">[identitySet][]</span></span>  | <span data-ttu-id="3cb20-189">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="3cb20-189">Identity of the creator of this item.</span></span> <span data-ttu-id="3cb20-190">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cb20-190">Read-only.</span></span>
| <span data-ttu-id="3cb20-191">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="3cb20-191">**createdDateTime**</span></span>      | <span data-ttu-id="3cb20-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cb20-192">DateTimeOffset</span></span>   | <span data-ttu-id="3cb20-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cb20-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="3cb20-195">**description**</span><span class="sxs-lookup"><span data-stu-id="3cb20-195">**description**</span></span>          | <span data-ttu-id="3cb20-196">строка</span><span class="sxs-lookup"><span data-stu-id="3cb20-196">string</span></span>           | <span data-ttu-id="3cb20-197">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="3cb20-197">The descriptive text for the item.</span></span>
| <span data-ttu-id="3cb20-198">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="3cb20-198">**lastModifiedBy**</span></span>       | <span data-ttu-id="3cb20-199">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-199">[identitySet][]</span></span>  | <span data-ttu-id="3cb20-200">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="3cb20-200">Identity of the last modifier of this item.</span></span> <span data-ttu-id="3cb20-201">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cb20-201">Read-only.</span></span>
| <span data-ttu-id="3cb20-202">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="3cb20-202">**lastModifiedDateTime**</span></span> | <span data-ttu-id="3cb20-203">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cb20-203">DateTimeOffset</span></span>   | <span data-ttu-id="3cb20-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cb20-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="3cb20-206">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="3cb20-206">**webUrl**</span></span>               | <span data-ttu-id="3cb20-207">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="3cb20-207">string (url)</span></span>     | <span data-ttu-id="3cb20-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cb20-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="3cb20-210">Связи</span><span class="sxs-lookup"><span data-stu-id="3cb20-210">Relationships</span></span>

<span data-ttu-id="3cb20-211">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="3cb20-211">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="3cb20-212">Имя связи</span><span class="sxs-lookup"><span data-stu-id="3cb20-212">Relationship name</span></span> | <span data-ttu-id="3cb20-213">Тип</span><span class="sxs-lookup"><span data-stu-id="3cb20-213">Type</span></span>                        | <span data-ttu-id="3cb20-214">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb20-214">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="3cb20-215">**activities**</span><span class="sxs-lookup"><span data-stu-id="3cb20-215">**activities**</span></span>    | <span data-ttu-id="3cb20-216">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-216">[itemActivity][] collection</span></span> | <span data-ttu-id="3cb20-217">Последние действия, выполненные в списке.</span><span class="sxs-lookup"><span data-stu-id="3cb20-217">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="3cb20-218">**drive**</span><span class="sxs-lookup"><span data-stu-id="3cb20-218">**drive**</span></span>         | <span data-ttu-id="3cb20-219">[drive][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-219">[drive][]</span></span>                   | <span data-ttu-id="3cb20-220">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="3cb20-220">Only present on document libraries.</span></span> <span data-ttu-id="3cb20-221">Разрешает доступ к списку как к ресурсу [drive][] с объектами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="3cb20-221">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="3cb20-222">**items**</span><span class="sxs-lookup"><span data-stu-id="3cb20-222">**items**</span></span>         | <span data-ttu-id="3cb20-223">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="3cb20-223">Collection([listItem][])</span></span>    | <span data-ttu-id="3cb20-224">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="3cb20-224">All items contained in the list.</span></span>
| <span data-ttu-id="3cb20-225">subscriptions</span><span class="sxs-lookup"><span data-stu-id="3cb20-225">subscriptions</span></span>      | <span data-ttu-id="3cb20-226">Коллекция [subscription][]</span><span class="sxs-lookup"><span data-stu-id="3cb20-226">[subscription][] collection</span></span> | <span data-ttu-id="3cb20-227">Набор подписок на список.</span><span class="sxs-lookup"><span data-stu-id="3cb20-227">The set of subscriptions on the list.</span></span>

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[site]: site.md
[systemFacet]: systemfacet.md
[subscription]: subscription.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  },
  "suppressions": []
}
-->


