---
author: JeremyKelley
ms.date: 09/11/2017
title: Перечисление
localization_priority: Priority
ms.prod: sharepoint
description: Ресурс list представляет список на сайте.
doc_type: resourcePageType
ms.openlocfilehash: 0f7c8600b8a4d8f41e6dd6e6ad4240252c004bbf
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317009"
---
# <a name="list-resource"></a><span data-ttu-id="2f909-103">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="2f909-103">List resource</span></span>

<span data-ttu-id="2f909-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f909-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f909-105">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="2f909-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="2f909-106">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="2f909-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="2f909-107">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="2f909-107">Tasks on a list</span></span>

<span data-ttu-id="2f909-108">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="2f909-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="2f909-109">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="2f909-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="2f909-110">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="2f909-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="2f909-111">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="2f909-111">All examples below are relative to a site, for example, `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="2f909-112">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="2f909-112">Common task</span></span>               | <span data-ttu-id="2f909-113">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="2f909-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="2f909-114">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="2f909-114">[Get list][]</span></span>              | <span data-ttu-id="2f909-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="2f909-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="2f909-116">[Создание списка][]</span><span class="sxs-lookup"><span data-stu-id="2f909-116">[Create list][]</span></span>           | <span data-ttu-id="2f909-117">POST /lists</span><span class="sxs-lookup"><span data-stu-id="2f909-117">POST /lists</span></span>
| <span data-ttu-id="2f909-118">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="2f909-118">[Enumerate list items][]</span></span>  | <span data-ttu-id="2f909-119">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="2f909-119">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="2f909-120">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="2f909-120">[Update list item][]</span></span>      | <span data-ttu-id="2f909-121">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="2f909-121">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="2f909-122">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="2f909-122">[Delete list item][]</span></span>      | <span data-ttu-id="2f909-123">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="2f909-123">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="2f909-124">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="2f909-124">[Create list item][]</span></span>      | <span data-ttu-id="2f909-125">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="2f909-125">POST /lists/{list-id}</span></span>
| <span data-ttu-id="2f909-126">[Получение канала WebSocket][]</span><span class="sxs-lookup"><span data-stu-id="2f909-126">[Get WebSocket channel][]</span></span> | <span data-ttu-id="2f909-127">GET /lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="2f909-127">GET /lists/{list-id}/subscriptions/socketIo</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="2f909-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f909-135">JSON representation</span></span>

<span data-ttu-id="2f909-136">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f909-136">Here is a JSON representation of a **list** resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "items",
    "drive"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type&quot;: &quot;microsoft.graph.list"
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
    "template&quot;: &quot;documentLibrary | genericList | survey | links | announcements | contacts | accessRequest ..."
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
  "webUrl&quot;: &quot;url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="2f909-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f909-137">Properties</span></span>

<span data-ttu-id="2f909-138">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="2f909-138">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="2f909-139">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2f909-139">Property name</span></span>    | <span data-ttu-id="2f909-140">Тип</span><span class="sxs-lookup"><span data-stu-id="2f909-140">Type</span></span>                             | <span data-ttu-id="2f909-141">Описание</span><span class="sxs-lookup"><span data-stu-id="2f909-141">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="2f909-142">**displayName**</span><span class="sxs-lookup"><span data-stu-id="2f909-142">**displayName**</span></span>  | <span data-ttu-id="2f909-143">строка</span><span class="sxs-lookup"><span data-stu-id="2f909-143">string</span></span>                           | <span data-ttu-id="2f909-144">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="2f909-144">The displayable title of the list.</span></span>
| <span data-ttu-id="2f909-145">**list**</span><span class="sxs-lookup"><span data-stu-id="2f909-145">**list**</span></span>         | <span data-ttu-id="2f909-146">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="2f909-146">[listInfo][]</span></span>                     | <span data-ttu-id="2f909-147">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="2f909-147">Provides additional details about the list.</span></span>
| <span data-ttu-id="2f909-148">**system**</span><span class="sxs-lookup"><span data-stu-id="2f909-148">**system**</span></span>       | <span data-ttu-id="2f909-149">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="2f909-149">[systemFacet][]</span></span>                  | <span data-ttu-id="2f909-p103">Если это свойство задано, оно указывает, что данным списком управляет система. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f909-p103">If present, indicates that this is a system-managed list. Read-only.</span></span>

<span data-ttu-id="2f909-152">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="2f909-152">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="2f909-153">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2f909-153">Property name</span></span>            | <span data-ttu-id="2f909-154">Тип</span><span class="sxs-lookup"><span data-stu-id="2f909-154">Type</span></span>              | <span data-ttu-id="2f909-155">Описание</span><span class="sxs-lookup"><span data-stu-id="2f909-155">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="2f909-156">**id**</span><span class="sxs-lookup"><span data-stu-id="2f909-156">**id**</span></span>                   | <span data-ttu-id="2f909-157">string</span><span class="sxs-lookup"><span data-stu-id="2f909-157">string</span></span>            | <span data-ttu-id="2f909-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f909-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="2f909-160">**name**</span><span class="sxs-lookup"><span data-stu-id="2f909-160">**name**</span></span>                 | <span data-ttu-id="2f909-161">строка</span><span class="sxs-lookup"><span data-stu-id="2f909-161">string</span></span>            | <span data-ttu-id="2f909-162">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="2f909-162">The name of the item.</span></span>
| <span data-ttu-id="2f909-163">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="2f909-163">**createdBy**</span></span>            | <span data-ttu-id="2f909-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2f909-164">[identitySet][]</span></span>   | <span data-ttu-id="2f909-p105">Удостоверение создателя данного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f909-p105">Identity of the creator of this item. Read-only.</span></span>
| <span data-ttu-id="2f909-167">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="2f909-167">**createdDateTime**</span></span>      | <span data-ttu-id="2f909-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f909-168">DateTimeOffset</span></span>    | <span data-ttu-id="2f909-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f909-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="2f909-171">**description**</span><span class="sxs-lookup"><span data-stu-id="2f909-171">**description**</span></span>          | <span data-ttu-id="2f909-172">строка</span><span class="sxs-lookup"><span data-stu-id="2f909-172">string</span></span>            | <span data-ttu-id="2f909-173">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="2f909-173">The descriptive text for the item.</span></span>
| <span data-ttu-id="2f909-174">**eTag**</span><span class="sxs-lookup"><span data-stu-id="2f909-174">**eTag**</span></span>                 | <span data-ttu-id="2f909-175">string</span><span class="sxs-lookup"><span data-stu-id="2f909-175">string</span></span>            | <span data-ttu-id="2f909-p107">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f909-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="2f909-178">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="2f909-178">**lastModifiedBy**</span></span>       | <span data-ttu-id="2f909-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2f909-179">[identitySet][]</span></span>   | <span data-ttu-id="2f909-p108">Удостоверение пользователя, который последним изменил данный элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f909-p108">Identity of the last modifier of this item. Read-only.</span></span>
| <span data-ttu-id="2f909-182">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="2f909-182">**lastModifiedDateTime**</span></span> | <span data-ttu-id="2f909-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f909-183">DateTimeOffset</span></span>    | <span data-ttu-id="2f909-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f909-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="2f909-186">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="2f909-186">**parentReference**</span></span>      | <span data-ttu-id="2f909-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="2f909-187">[itemReference][]</span></span> | <span data-ttu-id="2f909-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="2f909-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="2f909-190">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="2f909-190">**sharepointIds**</span></span>        | <span data-ttu-id="2f909-191">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="2f909-191">[sharepointIds][]</span></span> | <span data-ttu-id="2f909-p111">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f909-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="2f909-194">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="2f909-194">**webUrl**</span></span>               | <span data-ttu-id="2f909-195">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="2f909-195">string (url)</span></span>      | <span data-ttu-id="2f909-p112">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f909-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="2f909-198">Связи</span><span class="sxs-lookup"><span data-stu-id="2f909-198">Relationships</span></span>

<span data-ttu-id="2f909-199">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="2f909-199">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="2f909-200">Имя связи</span><span class="sxs-lookup"><span data-stu-id="2f909-200">Relationship name</span></span> | <span data-ttu-id="2f909-201">Тип</span><span class="sxs-lookup"><span data-stu-id="2f909-201">Type</span></span>                             | <span data-ttu-id="2f909-202">Описание</span><span class="sxs-lookup"><span data-stu-id="2f909-202">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="2f909-203">**drive**</span><span class="sxs-lookup"><span data-stu-id="2f909-203">**drive**</span></span>         | <span data-ttu-id="2f909-204">[drive][]</span><span class="sxs-lookup"><span data-stu-id="2f909-204">[drive][]</span></span>                        | <span data-ttu-id="2f909-205">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="2f909-205">Only present on document libraries.</span></span> <span data-ttu-id="2f909-206">Разрешает доступ к списку как к ресурсу [drive][] с объектами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="2f909-206">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="2f909-207">**items**</span><span class="sxs-lookup"><span data-stu-id="2f909-207">**items**</span></span>         | <span data-ttu-id="2f909-208">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="2f909-208">Collection([listItem][])</span></span>         | <span data-ttu-id="2f909-209">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="2f909-209">All items contained in the list.</span></span>
| <span data-ttu-id="2f909-210">**columns**</span><span class="sxs-lookup"><span data-stu-id="2f909-210">**columns**</span></span>       | <span data-ttu-id="2f909-211">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="2f909-211">Collection([columnDefinition][])</span></span> | <span data-ttu-id="2f909-212">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="2f909-212">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="2f909-213">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="2f909-213">**contentTypes**</span></span>  | <span data-ttu-id="2f909-214">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="2f909-214">Collection([contentType][])</span></span>      | <span data-ttu-id="2f909-215">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="2f909-215">The collection of content types present in this list.</span></span>
| <span data-ttu-id="2f909-216">**subscriptions**</span><span class="sxs-lookup"><span data-stu-id="2f909-216">**subscriptions**</span></span> | <span data-ttu-id="2f909-217">Коллекция ([subscription][])</span><span class="sxs-lookup"><span data-stu-id="2f909-217">Collection([subscription][])</span></span>     | <span data-ttu-id="2f909-218">Набор подписок на список.</span><span class="sxs-lookup"><span data-stu-id="2f909-218">The set of subscriptions on the list.</span></span>

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
    "Lists&quot;: &quot;#"
  }
} -->

