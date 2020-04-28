---
author: JeremyKelley
description: Ресурс list представляет список на сайте.
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 861e3c0b90c68ebf7a4a554e94097f790182727e
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43109049"
---
# <a name="list-resource"></a><span data-ttu-id="b123d-103">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="b123d-103">List resource</span></span>

<span data-ttu-id="b123d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b123d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b123d-105">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="b123d-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="b123d-106">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="b123d-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="b123d-107">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="b123d-107">Tasks on a list</span></span>

<span data-ttu-id="b123d-108">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="b123d-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="b123d-109">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="b123d-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="b123d-110">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="b123d-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="b123d-111">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="b123d-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="b123d-112">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="b123d-112">Common task</span></span>               | <span data-ttu-id="b123d-113">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="b123d-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="b123d-114">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="b123d-114">[Get list][]</span></span>              | <span data-ttu-id="b123d-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="b123d-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="b123d-116">[Создание списка][]</span><span class="sxs-lookup"><span data-stu-id="b123d-116">[Create list][]</span></span>           | <span data-ttu-id="b123d-117">POST /lists</span><span class="sxs-lookup"><span data-stu-id="b123d-117">POST /lists</span></span>
| <span data-ttu-id="b123d-118">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="b123d-118">[Enumerate list items][]</span></span>  | <span data-ttu-id="b123d-119">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="b123d-119">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="b123d-120">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="b123d-120">[Update list item][]</span></span>      | <span data-ttu-id="b123d-121">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b123d-121">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="b123d-122">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="b123d-122">[Delete list item][]</span></span>      | <span data-ttu-id="b123d-123">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b123d-123">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="b123d-124">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="b123d-124">[Create list item][]</span></span>      | <span data-ttu-id="b123d-125">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="b123d-125">POST /lists/{list-id}</span></span>
| <span data-ttu-id="b123d-126">[Получение последних действий][]</span><span class="sxs-lookup"><span data-stu-id="b123d-126">[Get recent activities][]</span></span> | <span data-ttu-id="b123d-127">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="b123d-127">GET /lists/{list-id}/activities</span></span>
| <span data-ttu-id="b123d-128">[Получение канала WebSocket][]</span><span class="sxs-lookup"><span data-stu-id="b123d-128">[Get WebSocket channel][]</span></span> | <span data-ttu-id="b123d-129">GET /lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="b123d-129">GET /lists/{list-id}/subscriptions/socketIo</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="b123d-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b123d-138">JSON representation</span></span>

<span data-ttu-id="b123d-139">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b123d-139">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b123d-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="b123d-140">Properties</span></span>

<span data-ttu-id="b123d-141">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="b123d-141">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="b123d-142">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b123d-142">Property name</span></span>    | <span data-ttu-id="b123d-143">Тип</span><span class="sxs-lookup"><span data-stu-id="b123d-143">Type</span></span>                             | <span data-ttu-id="b123d-144">Описание</span><span class="sxs-lookup"><span data-stu-id="b123d-144">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="b123d-145">**columns**</span><span class="sxs-lookup"><span data-stu-id="b123d-145">**columns**</span></span>      | <span data-ttu-id="b123d-146">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="b123d-146">Collection([columnDefinition][])</span></span> | <span data-ttu-id="b123d-147">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="b123d-147">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="b123d-148">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="b123d-148">**contentTypes**</span></span> | <span data-ttu-id="b123d-149">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="b123d-149">Collection([contentType][])</span></span>      | <span data-ttu-id="b123d-150">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="b123d-150">The collection of content types present in this list.</span></span>
| <span data-ttu-id="b123d-151">**displayName**</span><span class="sxs-lookup"><span data-stu-id="b123d-151">**displayName**</span></span>  | <span data-ttu-id="b123d-152">строка</span><span class="sxs-lookup"><span data-stu-id="b123d-152">string</span></span>                           | <span data-ttu-id="b123d-153">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="b123d-153">The displayable title of the list.</span></span>
| <span data-ttu-id="b123d-154">**list**</span><span class="sxs-lookup"><span data-stu-id="b123d-154">**list**</span></span>         | <span data-ttu-id="b123d-155">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="b123d-155">[listInfo][]</span></span>                     | <span data-ttu-id="b123d-156">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="b123d-156">Provides additional details about the list.</span></span>
| <span data-ttu-id="b123d-157">**system**</span><span class="sxs-lookup"><span data-stu-id="b123d-157">**system**</span></span>       | <span data-ttu-id="b123d-158">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="b123d-158">[systemFacet][]</span></span>                  | <span data-ttu-id="b123d-159">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="b123d-159">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="b123d-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b123d-160">Read-only.</span></span>

<span data-ttu-id="b123d-161">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="b123d-161">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="b123d-162">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b123d-162">Property name</span></span>            | <span data-ttu-id="b123d-163">Тип</span><span class="sxs-lookup"><span data-stu-id="b123d-163">Type</span></span>             | <span data-ttu-id="b123d-164">Описание</span><span class="sxs-lookup"><span data-stu-id="b123d-164">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="b123d-165">**id**</span><span class="sxs-lookup"><span data-stu-id="b123d-165">**id**</span></span>                   | <span data-ttu-id="b123d-166">string</span><span class="sxs-lookup"><span data-stu-id="b123d-166">string</span></span>           | <span data-ttu-id="b123d-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b123d-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="b123d-169">**name**</span><span class="sxs-lookup"><span data-stu-id="b123d-169">**name**</span></span>                 | <span data-ttu-id="b123d-170">string</span><span class="sxs-lookup"><span data-stu-id="b123d-170">string</span></span>           | <span data-ttu-id="b123d-171">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="b123d-171">The name of the item.</span></span>
| <span data-ttu-id="b123d-172">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="b123d-172">**createdBy**</span></span>            | <span data-ttu-id="b123d-173">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b123d-173">[identitySet][]</span></span>  | <span data-ttu-id="b123d-174">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="b123d-174">Identity of the creator of this item.</span></span> <span data-ttu-id="b123d-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b123d-175">Read-only.</span></span>
| <span data-ttu-id="b123d-176">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="b123d-176">**createdDateTime**</span></span>      | <span data-ttu-id="b123d-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b123d-177">DateTimeOffset</span></span>   | <span data-ttu-id="b123d-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b123d-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="b123d-180">**description**</span><span class="sxs-lookup"><span data-stu-id="b123d-180">**description**</span></span>          | <span data-ttu-id="b123d-181">строка</span><span class="sxs-lookup"><span data-stu-id="b123d-181">string</span></span>           | <span data-ttu-id="b123d-182">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="b123d-182">The descriptive text for the item.</span></span>
| <span data-ttu-id="b123d-183">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="b123d-183">**lastModifiedBy**</span></span>       | <span data-ttu-id="b123d-184">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b123d-184">[identitySet][]</span></span>  | <span data-ttu-id="b123d-185">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="b123d-185">Identity of the last modifier of this item.</span></span> <span data-ttu-id="b123d-186">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b123d-186">Read-only.</span></span>
| <span data-ttu-id="b123d-187">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b123d-187">**lastModifiedDateTime**</span></span> | <span data-ttu-id="b123d-188">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b123d-188">DateTimeOffset</span></span>   | <span data-ttu-id="b123d-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b123d-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="b123d-191">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="b123d-191">**webUrl**</span></span>               | <span data-ttu-id="b123d-192">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="b123d-192">string (url)</span></span>     | <span data-ttu-id="b123d-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b123d-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="b123d-195">Связи</span><span class="sxs-lookup"><span data-stu-id="b123d-195">Relationships</span></span>

<span data-ttu-id="b123d-196">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="b123d-196">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="b123d-197">Имя связи</span><span class="sxs-lookup"><span data-stu-id="b123d-197">Relationship name</span></span> | <span data-ttu-id="b123d-198">Тип</span><span class="sxs-lookup"><span data-stu-id="b123d-198">Type</span></span>                        | <span data-ttu-id="b123d-199">Описание</span><span class="sxs-lookup"><span data-stu-id="b123d-199">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="b123d-200">**activities**</span><span class="sxs-lookup"><span data-stu-id="b123d-200">**activities**</span></span>    | <span data-ttu-id="b123d-201">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="b123d-201">[itemActivity][] collection</span></span> | <span data-ttu-id="b123d-202">Последние действия, выполненные в списке.</span><span class="sxs-lookup"><span data-stu-id="b123d-202">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="b123d-203">**drive**</span><span class="sxs-lookup"><span data-stu-id="b123d-203">**drive**</span></span>         | <span data-ttu-id="b123d-204">[drive][]</span><span class="sxs-lookup"><span data-stu-id="b123d-204">[drive][]</span></span>                   | <span data-ttu-id="b123d-205">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="b123d-205">Only present on document libraries.</span></span> <span data-ttu-id="b123d-206">Разрешает доступ к списку как к ресурсу [drive][] с объектами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="b123d-206">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="b123d-207">**items**</span><span class="sxs-lookup"><span data-stu-id="b123d-207">**items**</span></span>         | <span data-ttu-id="b123d-208">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="b123d-208">Collection([listItem][])</span></span>    | <span data-ttu-id="b123d-209">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="b123d-209">All items contained in the list.</span></span>
| <span data-ttu-id="b123d-210">subscriptions</span><span class="sxs-lookup"><span data-stu-id="b123d-210">subscriptions</span></span>      | <span data-ttu-id="b123d-211">Коллекция [subscription][]</span><span class="sxs-lookup"><span data-stu-id="b123d-211">[subscription][] collection</span></span> | <span data-ttu-id="b123d-212">Набор подписок на список.</span><span class="sxs-lookup"><span data-stu-id="b123d-212">The set of subscriptions on the list.</span></span>

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
