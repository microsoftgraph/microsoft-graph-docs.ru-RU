---
author: JeremyKelley
description: Ресурс list представляет список на сайте.
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 634ac31e5fa5de3700c238b4a931e5b43455e801
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331243"
---
# <a name="list-resource"></a><span data-ttu-id="ccdbc-103">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="ccdbc-103">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccdbc-104">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="ccdbc-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="ccdbc-105">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="ccdbc-106">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="ccdbc-106">Tasks on a list</span></span>

<span data-ttu-id="ccdbc-107">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="ccdbc-108">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="ccdbc-109">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="ccdbc-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="ccdbc-110">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="ccdbc-111">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="ccdbc-111">Common task</span></span>               | <span data-ttu-id="ccdbc-112">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="ccdbc-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="ccdbc-113">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-113">[Get list][]</span></span>              | <span data-ttu-id="ccdbc-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="ccdbc-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="ccdbc-115">[Создание списка][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-115">[Create list][]</span></span>           | <span data-ttu-id="ccdbc-116">POST /lists</span><span class="sxs-lookup"><span data-stu-id="ccdbc-116">POST /lists</span></span>
| <span data-ttu-id="ccdbc-117">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-117">[Enumerate list items][]</span></span>  | <span data-ttu-id="ccdbc-118">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="ccdbc-118">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="ccdbc-119">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-119">[Update list item][]</span></span>      | <span data-ttu-id="ccdbc-120">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ccdbc-120">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="ccdbc-121">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-121">[Delete list item][]</span></span>      | <span data-ttu-id="ccdbc-122">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ccdbc-122">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="ccdbc-123">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-123">[Create list item][]</span></span>      | <span data-ttu-id="ccdbc-124">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="ccdbc-124">POST /lists/{list-id}</span></span>
| <span data-ttu-id="ccdbc-125">[Получение последних действий][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-125">[Get recent activities][]</span></span> | <span data-ttu-id="ccdbc-126">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="ccdbc-126">GET /lists/{list-id}/activities</span></span>
| <span data-ttu-id="ccdbc-127">[Получение канала WebSocket][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-127">[Get WebSocket channel][]</span></span> | <span data-ttu-id="ccdbc-128">ПОЛУЧЕНИЕ/Листс/{лист-ИД}/субскриптионс/соккетио</span><span class="sxs-lookup"><span data-stu-id="ccdbc-128">GET /lists/{list-id}/subscriptions/socketIo</span></span>

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
[Получение канала WebSocket]: ../api/driveitem-subscriptions-socketio.md
[Get WebSocket channel]: ../api/driveitem-subscriptions-socketio.md

## <a name="json-representation"></a><span data-ttu-id="ccdbc-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ccdbc-137">JSON representation</span></span>

<span data-ttu-id="ccdbc-138">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-138">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ccdbc-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="ccdbc-139">Properties</span></span>

<span data-ttu-id="ccdbc-140">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-140">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="ccdbc-141">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ccdbc-141">Property name</span></span>    | <span data-ttu-id="ccdbc-142">Тип</span><span class="sxs-lookup"><span data-stu-id="ccdbc-142">Type</span></span>                             | <span data-ttu-id="ccdbc-143">Описание</span><span class="sxs-lookup"><span data-stu-id="ccdbc-143">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="ccdbc-144">**columns**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-144">**columns**</span></span>      | <span data-ttu-id="ccdbc-145">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="ccdbc-145">Collection([columnDefinition][])</span></span> | <span data-ttu-id="ccdbc-146">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-146">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="ccdbc-147">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-147">**contentTypes**</span></span> | <span data-ttu-id="ccdbc-148">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="ccdbc-148">Collection([contentType][])</span></span>      | <span data-ttu-id="ccdbc-149">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-149">The collection of content types present in this list.</span></span>
| <span data-ttu-id="ccdbc-150">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-150">**displayName**</span></span>  | <span data-ttu-id="ccdbc-151">строка</span><span class="sxs-lookup"><span data-stu-id="ccdbc-151">string</span></span>                           | <span data-ttu-id="ccdbc-152">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-152">The displayable title of the list.</span></span>
| <span data-ttu-id="ccdbc-153">**list**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-153">**list**</span></span>         | <span data-ttu-id="ccdbc-154">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-154">[listInfo][]</span></span>                     | <span data-ttu-id="ccdbc-155">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-155">Provides additional details about the list.</span></span>
| <span data-ttu-id="ccdbc-156">**system**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-156">**system**</span></span>       | <span data-ttu-id="ccdbc-157">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-157">[systemFacet][]</span></span>                  | <span data-ttu-id="ccdbc-158">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-158">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="ccdbc-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-159">Read-only.</span></span>

<span data-ttu-id="ccdbc-160">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="ccdbc-161">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ccdbc-161">Property name</span></span>            | <span data-ttu-id="ccdbc-162">Тип</span><span class="sxs-lookup"><span data-stu-id="ccdbc-162">Type</span></span>             | <span data-ttu-id="ccdbc-163">Описание</span><span class="sxs-lookup"><span data-stu-id="ccdbc-163">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="ccdbc-164">**id**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-164">**id**</span></span>                   | <span data-ttu-id="ccdbc-165">string</span><span class="sxs-lookup"><span data-stu-id="ccdbc-165">string</span></span>           | <span data-ttu-id="ccdbc-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="ccdbc-168">**name**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-168">**name**</span></span>                 | <span data-ttu-id="ccdbc-169">string</span><span class="sxs-lookup"><span data-stu-id="ccdbc-169">string</span></span>           | <span data-ttu-id="ccdbc-170">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-170">The name of the item.</span></span>
| <span data-ttu-id="ccdbc-171">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-171">**createdBy**</span></span>            | <span data-ttu-id="ccdbc-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-172">[identitySet][]</span></span>  | <span data-ttu-id="ccdbc-173">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-173">Identity of the creator of this item.</span></span> <span data-ttu-id="ccdbc-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-174">Read-only.</span></span>
| <span data-ttu-id="ccdbc-175">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-175">**createdDateTime**</span></span>      | <span data-ttu-id="ccdbc-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccdbc-176">DateTimeOffset</span></span>   | <span data-ttu-id="ccdbc-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ccdbc-179">**description**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-179">**description**</span></span>          | <span data-ttu-id="ccdbc-180">строка</span><span class="sxs-lookup"><span data-stu-id="ccdbc-180">string</span></span>           | <span data-ttu-id="ccdbc-181">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-181">The descriptive text for the item.</span></span>
| <span data-ttu-id="ccdbc-182">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="ccdbc-182">**lastModifiedBy**</span></span>       | <span data-ttu-id="ccdbc-183">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-183">[identitySet][]</span></span>  | <span data-ttu-id="ccdbc-184">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-184">Identity of the last modifier of this item.</span></span> <span data-ttu-id="ccdbc-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-185">Read-only.</span></span>
| <span data-ttu-id="ccdbc-186">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-186">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ccdbc-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccdbc-187">DateTimeOffset</span></span>   | <span data-ttu-id="ccdbc-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ccdbc-190">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-190">**webUrl**</span></span>               | <span data-ttu-id="ccdbc-191">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="ccdbc-191">string (url)</span></span>     | <span data-ttu-id="ccdbc-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="ccdbc-194">Связи</span><span class="sxs-lookup"><span data-stu-id="ccdbc-194">Relationships</span></span>

<span data-ttu-id="ccdbc-195">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-195">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="ccdbc-196">Имя связи</span><span class="sxs-lookup"><span data-stu-id="ccdbc-196">Relationship name</span></span> | <span data-ttu-id="ccdbc-197">Тип</span><span class="sxs-lookup"><span data-stu-id="ccdbc-197">Type</span></span>                        | <span data-ttu-id="ccdbc-198">Описание</span><span class="sxs-lookup"><span data-stu-id="ccdbc-198">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="ccdbc-199">**activities**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-199">**activities**</span></span>    | <span data-ttu-id="ccdbc-200">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-200">[itemActivity][] collection</span></span> | <span data-ttu-id="ccdbc-201">Последние действия, выполненные в списке.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-201">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="ccdbc-202">**drive**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-202">**drive**</span></span>         | <span data-ttu-id="ccdbc-203">[drive][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-203">[drive][]</span></span>                   | <span data-ttu-id="ccdbc-204">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-204">Only present on document libraries.</span></span> <span data-ttu-id="ccdbc-205">Разрешает доступ к списку как к ресурсу [drive][] с объектами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="ccdbc-205">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="ccdbc-206">**items**</span><span class="sxs-lookup"><span data-stu-id="ccdbc-206">**items**</span></span>         | <span data-ttu-id="ccdbc-207">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="ccdbc-207">Collection([listItem][])</span></span>    | <span data-ttu-id="ccdbc-208">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-208">All items contained in the list.</span></span>
| <span data-ttu-id="ccdbc-209">subscriptions</span><span class="sxs-lookup"><span data-stu-id="ccdbc-209">subscriptions</span></span>      | <span data-ttu-id="ccdbc-210">Коллекция [subscription][]</span><span class="sxs-lookup"><span data-stu-id="ccdbc-210">[subscription][] collection</span></span> | <span data-ttu-id="ccdbc-211">Набор подписок в списке.</span><span class="sxs-lookup"><span data-stu-id="ccdbc-211">The set of subscriptions on the list.</span></span>

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
