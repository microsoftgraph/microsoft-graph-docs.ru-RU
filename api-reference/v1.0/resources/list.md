---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Перечисление
localization_priority: Priority
ms.prod: sharepoint
description: Ресурс list представляет список на сайте.
doc_type: resourcePageType
ms.openlocfilehash: db6fceb1f7806b5356a4e75f1e4fb6a247bd5b00
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108485"
---
# <a name="list-resource"></a><span data-ttu-id="8c6e8-103">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="8c6e8-103">List resource</span></span>

<span data-ttu-id="8c6e8-104">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="8c6e8-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="8c6e8-105">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="8c6e8-106">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="8c6e8-106">Tasks on a list</span></span>

<span data-ttu-id="8c6e8-107">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="8c6e8-108">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="8c6e8-109">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="8c6e8-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="8c6e8-110">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="8c6e8-111">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="8c6e8-111">Common task</span></span>               | <span data-ttu-id="8c6e8-112">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="8c6e8-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="8c6e8-113">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-113">[Get list][]</span></span>              | <span data-ttu-id="8c6e8-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="8c6e8-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="8c6e8-115">[Создание списка][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-115">[Create list][]</span></span>           | <span data-ttu-id="8c6e8-116">POST /lists</span><span class="sxs-lookup"><span data-stu-id="8c6e8-116">POST /lists</span></span>
| <span data-ttu-id="8c6e8-117">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-117">[Enumerate list items][]</span></span>  | <span data-ttu-id="8c6e8-118">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="8c6e8-118">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="8c6e8-119">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-119">[Update list item][]</span></span>      | <span data-ttu-id="8c6e8-120">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="8c6e8-120">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="8c6e8-121">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-121">[Delete list item][]</span></span>      | <span data-ttu-id="8c6e8-122">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="8c6e8-122">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="8c6e8-123">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-123">[Create list item][]</span></span>      | <span data-ttu-id="8c6e8-124">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="8c6e8-124">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="8c6e8-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8c6e8-131">JSON representation</span></span>

<span data-ttu-id="8c6e8-132">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-132">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8c6e8-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c6e8-133">Properties</span></span>

<span data-ttu-id="8c6e8-134">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-134">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="8c6e8-135">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8c6e8-135">Property name</span></span>    | <span data-ttu-id="8c6e8-136">Тип</span><span class="sxs-lookup"><span data-stu-id="8c6e8-136">Type</span></span>                             | <span data-ttu-id="8c6e8-137">Описание</span><span class="sxs-lookup"><span data-stu-id="8c6e8-137">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="8c6e8-138">**displayName**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-138">**displayName**</span></span>  | <span data-ttu-id="8c6e8-139">строка</span><span class="sxs-lookup"><span data-stu-id="8c6e8-139">string</span></span>                           | <span data-ttu-id="8c6e8-140">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-140">The displayable title of the list.</span></span>
| <span data-ttu-id="8c6e8-141">**list**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-141">**list**</span></span>         | <span data-ttu-id="8c6e8-142">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-142">[listInfo][]</span></span>                     | <span data-ttu-id="8c6e8-143">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-143">Provides additional details about the list.</span></span>
| <span data-ttu-id="8c6e8-144">**system**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-144">**system**</span></span>       | <span data-ttu-id="8c6e8-145">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-145">[systemFacet][]</span></span>                  | <span data-ttu-id="8c6e8-146">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-146">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="8c6e8-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-147">Read-only.</span></span>

<span data-ttu-id="8c6e8-148">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-148">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="8c6e8-149">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8c6e8-149">Property name</span></span>            | <span data-ttu-id="8c6e8-150">Тип</span><span class="sxs-lookup"><span data-stu-id="8c6e8-150">Type</span></span>              | <span data-ttu-id="8c6e8-151">Описание</span><span class="sxs-lookup"><span data-stu-id="8c6e8-151">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="8c6e8-152">**id**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-152">**id**</span></span>                   | <span data-ttu-id="8c6e8-153">string</span><span class="sxs-lookup"><span data-stu-id="8c6e8-153">string</span></span>            | <span data-ttu-id="8c6e8-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="8c6e8-156">**name**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-156">**name**</span></span>                 | <span data-ttu-id="8c6e8-157">строка</span><span class="sxs-lookup"><span data-stu-id="8c6e8-157">string</span></span>            | <span data-ttu-id="8c6e8-158">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-158">The name of the item.</span></span>
| <span data-ttu-id="8c6e8-159">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-159">**createdBy**</span></span>            | <span data-ttu-id="8c6e8-160">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-160">[identitySet][]</span></span>   | <span data-ttu-id="8c6e8-161">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-161">Identity of the creator of this item.</span></span> <span data-ttu-id="8c6e8-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-162">Read-only.</span></span>
| <span data-ttu-id="8c6e8-163">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-163">**createdDateTime**</span></span>      | <span data-ttu-id="8c6e8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c6e8-164">DateTimeOffset</span></span>    | <span data-ttu-id="8c6e8-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="8c6e8-167">**description**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-167">**description**</span></span>          | <span data-ttu-id="8c6e8-168">строка</span><span class="sxs-lookup"><span data-stu-id="8c6e8-168">string</span></span>            | <span data-ttu-id="8c6e8-169">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-169">The descriptive text for the item.</span></span>
| <span data-ttu-id="8c6e8-170">**eTag**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-170">**eTag**</span></span>                 | <span data-ttu-id="8c6e8-171">string</span><span class="sxs-lookup"><span data-stu-id="8c6e8-171">string</span></span>            | <span data-ttu-id="8c6e8-p107">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="8c6e8-174">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="8c6e8-174">**lastModifiedBy**</span></span>       | <span data-ttu-id="8c6e8-175">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-175">[identitySet][]</span></span>   | <span data-ttu-id="8c6e8-176">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-176">Identity of the last modifier of this item.</span></span> <span data-ttu-id="8c6e8-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-177">Read-only.</span></span>
| <span data-ttu-id="8c6e8-178">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-178">**lastModifiedDateTime**</span></span> | <span data-ttu-id="8c6e8-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c6e8-179">DateTimeOffset</span></span>    | <span data-ttu-id="8c6e8-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="8c6e8-182">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-182">**parentReference**</span></span>      | <span data-ttu-id="8c6e8-183">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-183">[itemReference][]</span></span> | <span data-ttu-id="8c6e8-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="8c6e8-186">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-186">**sharepointIds**</span></span>        | <span data-ttu-id="8c6e8-187">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-187">[sharepointIds][]</span></span> | <span data-ttu-id="8c6e8-p111">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="8c6e8-190">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-190">**webUrl**</span></span>               | <span data-ttu-id="8c6e8-191">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="8c6e8-191">string (url)</span></span>      | <span data-ttu-id="8c6e8-p112">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="8c6e8-194">Связи</span><span class="sxs-lookup"><span data-stu-id="8c6e8-194">Relationships</span></span>

<span data-ttu-id="8c6e8-195">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-195">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="8c6e8-196">Имя связи</span><span class="sxs-lookup"><span data-stu-id="8c6e8-196">Relationship name</span></span> | <span data-ttu-id="8c6e8-197">Тип</span><span class="sxs-lookup"><span data-stu-id="8c6e8-197">Type</span></span>                             | <span data-ttu-id="8c6e8-198">Описание</span><span class="sxs-lookup"><span data-stu-id="8c6e8-198">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="8c6e8-199">**drive**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-199">**drive**</span></span>         | <span data-ttu-id="8c6e8-200">[drive][]</span><span class="sxs-lookup"><span data-stu-id="8c6e8-200">[drive][]</span></span>                        | <span data-ttu-id="8c6e8-201">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-201">Only present on document libraries.</span></span> <span data-ttu-id="8c6e8-202">Разрешает доступ к списку как к ресурсу [drive][] с объектами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="8c6e8-202">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="8c6e8-203">**items**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-203">**items**</span></span>         | <span data-ttu-id="8c6e8-204">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="8c6e8-204">Collection([listItem][])</span></span>         | <span data-ttu-id="8c6e8-205">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-205">All items contained in the list.</span></span>
| <span data-ttu-id="8c6e8-206">**columns**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-206">**columns**</span></span>       | <span data-ttu-id="8c6e8-207">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="8c6e8-207">Collection([columnDefinition][])</span></span> | <span data-ttu-id="8c6e8-208">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-208">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="8c6e8-209">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="8c6e8-209">**contentTypes**</span></span>  | <span data-ttu-id="8c6e8-210">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="8c6e8-210">Collection([contentType][])</span></span>      | <span data-ttu-id="8c6e8-211">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="8c6e8-211">The collection of content types present in this list.</span></span>

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
