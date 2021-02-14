---
author: JeremyKelley
ms.date: 09/11/2017
title: Перечисление
localization_priority: Priority
ms.prod: sharepoint
description: Ресурс list представляет список на сайте.
doc_type: resourcePageType
ms.openlocfilehash: 4079320ef785dbdb3c1367fad92cda46eab0b4fa
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239368"
---
# <a name="list-resource"></a><span data-ttu-id="f4047-103">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="f4047-103">List resource</span></span>

<span data-ttu-id="f4047-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4047-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4047-105">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="f4047-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="f4047-106">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="f4047-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="f4047-107">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="f4047-107">Tasks on a list</span></span>

<span data-ttu-id="f4047-108">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="f4047-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="f4047-109">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="f4047-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="f4047-110">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="f4047-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="f4047-111">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="f4047-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="f4047-112">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="f4047-112">Common task</span></span>               | <span data-ttu-id="f4047-113">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="f4047-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="f4047-114">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="f4047-114">[Get list][]</span></span>              | <span data-ttu-id="f4047-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="f4047-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="f4047-116">[Создание списка][]</span><span class="sxs-lookup"><span data-stu-id="f4047-116">[Create list][]</span></span>           | <span data-ttu-id="f4047-117">POST /lists</span><span class="sxs-lookup"><span data-stu-id="f4047-117">POST /lists</span></span>
| <span data-ttu-id="f4047-118">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="f4047-118">[Enumerate list items][]</span></span>  | <span data-ttu-id="f4047-119">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="f4047-119">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="f4047-120">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="f4047-120">[Update list item][]</span></span>      | <span data-ttu-id="f4047-121">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="f4047-121">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="f4047-122">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="f4047-122">[Delete list item][]</span></span>      | <span data-ttu-id="f4047-123">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="f4047-123">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="f4047-124">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="f4047-124">[Create list item][]</span></span>      | <span data-ttu-id="f4047-125">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="f4047-125">POST /lists/{list-id}</span></span>
| <span data-ttu-id="f4047-126">[Получение канала WebSocket][]</span><span class="sxs-lookup"><span data-stu-id="f4047-126">[Get WebSocket channel][]</span></span> | <span data-ttu-id="f4047-127">GET /lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="f4047-127">GET /lists/{list-id}/subscriptions/socketIo</span></span>

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
[Получение канала WebSocket]: ../api/subscriptions-socketio.md
[Get WebSocket channel]: ../api/subscriptions-socketio.md

## <a name="json-representation"></a><span data-ttu-id="f4047-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4047-135">JSON representation</span></span>

<span data-ttu-id="f4047-136">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4047-136">Here is a JSON representation of a **list** resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "items",
    "drive"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.list"
}-->

```json
{
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template": "documentLibrary | genericList | survey | links | announcements | contacts | accessRequest ..."
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
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="f4047-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4047-137">Properties</span></span>

<span data-ttu-id="f4047-138">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="f4047-138">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="f4047-139">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f4047-139">Property name</span></span>    | <span data-ttu-id="f4047-140">Тип</span><span class="sxs-lookup"><span data-stu-id="f4047-140">Type</span></span>                             | <span data-ttu-id="f4047-141">Описание</span><span class="sxs-lookup"><span data-stu-id="f4047-141">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="f4047-142">**displayName**</span><span class="sxs-lookup"><span data-stu-id="f4047-142">**displayName**</span></span>  | <span data-ttu-id="f4047-143">строка</span><span class="sxs-lookup"><span data-stu-id="f4047-143">string</span></span>                           | <span data-ttu-id="f4047-144">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="f4047-144">The displayable title of the list.</span></span>
| <span data-ttu-id="f4047-145">**list**</span><span class="sxs-lookup"><span data-stu-id="f4047-145">**list**</span></span>         | <span data-ttu-id="f4047-146">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="f4047-146">[listInfo][]</span></span>                     | <span data-ttu-id="f4047-147">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="f4047-147">Provides additional details about the list.</span></span>
| <span data-ttu-id="f4047-148">**system**</span><span class="sxs-lookup"><span data-stu-id="f4047-148">**system**</span></span>       | <span data-ttu-id="f4047-149">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="f4047-149">[systemFacet][]</span></span>                  | <span data-ttu-id="f4047-150">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="f4047-150">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="f4047-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4047-151">Read-only.</span></span>

<span data-ttu-id="f4047-152">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="f4047-152">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="f4047-153">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f4047-153">Property name</span></span>            | <span data-ttu-id="f4047-154">Тип</span><span class="sxs-lookup"><span data-stu-id="f4047-154">Type</span></span>              | <span data-ttu-id="f4047-155">Описание</span><span class="sxs-lookup"><span data-stu-id="f4047-155">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="f4047-156">**id**</span><span class="sxs-lookup"><span data-stu-id="f4047-156">**id**</span></span>                   | <span data-ttu-id="f4047-157">string</span><span class="sxs-lookup"><span data-stu-id="f4047-157">string</span></span>            | <span data-ttu-id="f4047-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4047-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="f4047-160">**name**</span><span class="sxs-lookup"><span data-stu-id="f4047-160">**name**</span></span>                 | <span data-ttu-id="f4047-161">строка</span><span class="sxs-lookup"><span data-stu-id="f4047-161">string</span></span>            | <span data-ttu-id="f4047-162">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="f4047-162">The name of the item.</span></span>
| <span data-ttu-id="f4047-163">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="f4047-163">**createdBy**</span></span>            | <span data-ttu-id="f4047-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f4047-164">[identitySet][]</span></span>   | <span data-ttu-id="f4047-165">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="f4047-165">Identity of the creator of this item.</span></span> <span data-ttu-id="f4047-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4047-166">Read-only.</span></span>
| <span data-ttu-id="f4047-167">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="f4047-167">**createdDateTime**</span></span>      | <span data-ttu-id="f4047-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4047-168">DateTimeOffset</span></span>    | <span data-ttu-id="f4047-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4047-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="f4047-171">**description**</span><span class="sxs-lookup"><span data-stu-id="f4047-171">**description**</span></span>          | <span data-ttu-id="f4047-172">строка</span><span class="sxs-lookup"><span data-stu-id="f4047-172">string</span></span>            | <span data-ttu-id="f4047-173">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="f4047-173">The descriptive text for the item.</span></span>
| <span data-ttu-id="f4047-174">**eTag**</span><span class="sxs-lookup"><span data-stu-id="f4047-174">**eTag**</span></span>                 | <span data-ttu-id="f4047-175">string</span><span class="sxs-lookup"><span data-stu-id="f4047-175">string</span></span>            | <span data-ttu-id="f4047-p107">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4047-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="f4047-178">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="f4047-178">**lastModifiedBy**</span></span>       | <span data-ttu-id="f4047-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f4047-179">[identitySet][]</span></span>   | <span data-ttu-id="f4047-180">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="f4047-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="f4047-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4047-181">Read-only.</span></span>
| <span data-ttu-id="f4047-182">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f4047-182">**lastModifiedDateTime**</span></span> | <span data-ttu-id="f4047-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4047-183">DateTimeOffset</span></span>    | <span data-ttu-id="f4047-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4047-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f4047-186">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="f4047-186">**parentReference**</span></span>      | <span data-ttu-id="f4047-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="f4047-187">[itemReference][]</span></span> | <span data-ttu-id="f4047-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="f4047-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="f4047-190">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="f4047-190">**sharepointIds**</span></span>        | <span data-ttu-id="f4047-191">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f4047-191">[sharepointIds][]</span></span> | <span data-ttu-id="f4047-p111">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4047-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="f4047-194">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="f4047-194">**webUrl**</span></span>               | <span data-ttu-id="f4047-195">string (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="f4047-195">string (url)</span></span>      | <span data-ttu-id="f4047-p112">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4047-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="f4047-198">Связи</span><span class="sxs-lookup"><span data-stu-id="f4047-198">Relationships</span></span>

<span data-ttu-id="f4047-199">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="f4047-199">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="f4047-200">Имя связи</span><span class="sxs-lookup"><span data-stu-id="f4047-200">Relationship name</span></span> | <span data-ttu-id="f4047-201">Тип</span><span class="sxs-lookup"><span data-stu-id="f4047-201">Type</span></span>                             | <span data-ttu-id="f4047-202">Описание</span><span class="sxs-lookup"><span data-stu-id="f4047-202">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="f4047-203">**drive**</span><span class="sxs-lookup"><span data-stu-id="f4047-203">**drive**</span></span>         | <span data-ttu-id="f4047-204">[drive][]</span><span class="sxs-lookup"><span data-stu-id="f4047-204">[drive][]</span></span>                        | <span data-ttu-id="f4047-205">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="f4047-205">Only present on document libraries.</span></span> <span data-ttu-id="f4047-206">Разрешает доступ к списку как к ресурсу [drive][] с объектами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="f4047-206">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="f4047-207">**items**</span><span class="sxs-lookup"><span data-stu-id="f4047-207">**items**</span></span>         | <span data-ttu-id="f4047-208">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="f4047-208">Collection([listItem][])</span></span>         | <span data-ttu-id="f4047-209">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="f4047-209">All items contained in the list.</span></span>
| <span data-ttu-id="f4047-210">**columns**</span><span class="sxs-lookup"><span data-stu-id="f4047-210">**columns**</span></span>       | <span data-ttu-id="f4047-211">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="f4047-211">Collection([columnDefinition][])</span></span> | <span data-ttu-id="f4047-212">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="f4047-212">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="f4047-213">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="f4047-213">**contentTypes**</span></span>  | <span data-ttu-id="f4047-214">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="f4047-214">Collection([contentType][])</span></span>      | <span data-ttu-id="f4047-215">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="f4047-215">The collection of content types present in this list.</span></span>
| <span data-ttu-id="f4047-216">**subscriptions**</span><span class="sxs-lookup"><span data-stu-id="f4047-216">**subscriptions**</span></span> | <span data-ttu-id="f4047-217">Коллекция ([subscription][])</span><span class="sxs-lookup"><span data-stu-id="f4047-217">Collection([subscription][])</span></span>     | <span data-ttu-id="f4047-218">Набор подписок на список.</span><span class="sxs-lookup"><span data-stu-id="f4047-218">The set of subscriptions on the list.</span></span>

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[sharepointIds]: sharepointids.md
[site]: site.md
[systemFacet]: systemfacet.md
[subscription]: subscription.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  }
} -->

