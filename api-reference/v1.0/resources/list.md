---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Перечисление
localization_priority: Priority
ms.prod: sharepoint
description: Ресурс list представляет список на сайте.
doc_type: resourcePageType
ms.openlocfilehash: af970267f4aebcac986659324a30238a8510c010
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447586"
---
# <a name="list-resource"></a><span data-ttu-id="20887-103">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="20887-103">List resource</span></span>

<span data-ttu-id="20887-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20887-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20887-105">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="20887-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="20887-106">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="20887-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="20887-107">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="20887-107">Tasks on a list</span></span>

<span data-ttu-id="20887-108">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="20887-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="20887-109">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="20887-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="20887-110">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="20887-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="20887-111">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="20887-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="20887-112">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="20887-112">Common task</span></span>               | <span data-ttu-id="20887-113">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="20887-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="20887-114">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="20887-114">[Get list][]</span></span>              | <span data-ttu-id="20887-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="20887-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="20887-116">[Создание списка][]</span><span class="sxs-lookup"><span data-stu-id="20887-116">[Create list][]</span></span>           | <span data-ttu-id="20887-117">POST /lists</span><span class="sxs-lookup"><span data-stu-id="20887-117">POST /lists</span></span>
| <span data-ttu-id="20887-118">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="20887-118">[Enumerate list items][]</span></span>  | <span data-ttu-id="20887-119">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="20887-119">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="20887-120">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="20887-120">[Update list item][]</span></span>      | <span data-ttu-id="20887-121">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="20887-121">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="20887-122">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="20887-122">[Delete list item][]</span></span>      | <span data-ttu-id="20887-123">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="20887-123">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="20887-124">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="20887-124">[Create list item][]</span></span>      | <span data-ttu-id="20887-125">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="20887-125">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="20887-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="20887-132">JSON representation</span></span>

<span data-ttu-id="20887-133">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20887-133">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="20887-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="20887-134">Properties</span></span>

<span data-ttu-id="20887-135">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="20887-135">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="20887-136">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="20887-136">Property name</span></span>    | <span data-ttu-id="20887-137">Тип</span><span class="sxs-lookup"><span data-stu-id="20887-137">Type</span></span>                             | <span data-ttu-id="20887-138">Описание</span><span class="sxs-lookup"><span data-stu-id="20887-138">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="20887-139">**displayName**</span><span class="sxs-lookup"><span data-stu-id="20887-139">**displayName**</span></span>  | <span data-ttu-id="20887-140">строка</span><span class="sxs-lookup"><span data-stu-id="20887-140">string</span></span>                           | <span data-ttu-id="20887-141">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="20887-141">The displayable title of the list.</span></span>
| <span data-ttu-id="20887-142">**list**</span><span class="sxs-lookup"><span data-stu-id="20887-142">**list**</span></span>         | <span data-ttu-id="20887-143">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="20887-143">[listInfo][]</span></span>                     | <span data-ttu-id="20887-144">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="20887-144">Provides additional details about the list.</span></span>
| <span data-ttu-id="20887-145">**system**</span><span class="sxs-lookup"><span data-stu-id="20887-145">**system**</span></span>       | <span data-ttu-id="20887-146">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="20887-146">[systemFacet][]</span></span>                  | <span data-ttu-id="20887-147">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="20887-147">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="20887-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20887-148">Read-only.</span></span>

<span data-ttu-id="20887-149">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="20887-149">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="20887-150">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="20887-150">Property name</span></span>            | <span data-ttu-id="20887-151">Тип</span><span class="sxs-lookup"><span data-stu-id="20887-151">Type</span></span>              | <span data-ttu-id="20887-152">Описание</span><span class="sxs-lookup"><span data-stu-id="20887-152">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="20887-153">**id**</span><span class="sxs-lookup"><span data-stu-id="20887-153">**id**</span></span>                   | <span data-ttu-id="20887-154">string</span><span class="sxs-lookup"><span data-stu-id="20887-154">string</span></span>            | <span data-ttu-id="20887-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20887-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="20887-157">**name**</span><span class="sxs-lookup"><span data-stu-id="20887-157">**name**</span></span>                 | <span data-ttu-id="20887-158">строка</span><span class="sxs-lookup"><span data-stu-id="20887-158">string</span></span>            | <span data-ttu-id="20887-159">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="20887-159">The name of the item.</span></span>
| <span data-ttu-id="20887-160">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="20887-160">**createdBy**</span></span>            | <span data-ttu-id="20887-161">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="20887-161">[identitySet][]</span></span>   | <span data-ttu-id="20887-162">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="20887-162">Identity of the creator of this item.</span></span> <span data-ttu-id="20887-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20887-163">Read-only.</span></span>
| <span data-ttu-id="20887-164">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="20887-164">**createdDateTime**</span></span>      | <span data-ttu-id="20887-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20887-165">DateTimeOffset</span></span>    | <span data-ttu-id="20887-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20887-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="20887-168">**description**</span><span class="sxs-lookup"><span data-stu-id="20887-168">**description**</span></span>          | <span data-ttu-id="20887-169">строка</span><span class="sxs-lookup"><span data-stu-id="20887-169">string</span></span>            | <span data-ttu-id="20887-170">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="20887-170">The descriptive text for the item.</span></span>
| <span data-ttu-id="20887-171">**eTag**</span><span class="sxs-lookup"><span data-stu-id="20887-171">**eTag**</span></span>                 | <span data-ttu-id="20887-172">string</span><span class="sxs-lookup"><span data-stu-id="20887-172">string</span></span>            | <span data-ttu-id="20887-p107">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20887-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="20887-175">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="20887-175">**lastModifiedBy**</span></span>       | <span data-ttu-id="20887-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="20887-176">[identitySet][]</span></span>   | <span data-ttu-id="20887-177">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="20887-177">Identity of the last modifier of this item.</span></span> <span data-ttu-id="20887-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20887-178">Read-only.</span></span>
| <span data-ttu-id="20887-179">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="20887-179">**lastModifiedDateTime**</span></span> | <span data-ttu-id="20887-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20887-180">DateTimeOffset</span></span>    | <span data-ttu-id="20887-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20887-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="20887-183">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="20887-183">**parentReference**</span></span>      | <span data-ttu-id="20887-184">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="20887-184">[itemReference][]</span></span> | <span data-ttu-id="20887-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="20887-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="20887-187">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="20887-187">**sharepointIds**</span></span>        | <span data-ttu-id="20887-188">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="20887-188">[sharepointIds][]</span></span> | <span data-ttu-id="20887-p111">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20887-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="20887-191">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="20887-191">**webUrl**</span></span>               | <span data-ttu-id="20887-192">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="20887-192">string (url)</span></span>      | <span data-ttu-id="20887-p112">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20887-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="20887-195">Связи</span><span class="sxs-lookup"><span data-stu-id="20887-195">Relationships</span></span>

<span data-ttu-id="20887-196">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="20887-196">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="20887-197">Имя связи</span><span class="sxs-lookup"><span data-stu-id="20887-197">Relationship name</span></span> | <span data-ttu-id="20887-198">Тип</span><span class="sxs-lookup"><span data-stu-id="20887-198">Type</span></span>                             | <span data-ttu-id="20887-199">Описание</span><span class="sxs-lookup"><span data-stu-id="20887-199">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="20887-200">**drive**</span><span class="sxs-lookup"><span data-stu-id="20887-200">**drive**</span></span>         | <span data-ttu-id="20887-201">[drive][]</span><span class="sxs-lookup"><span data-stu-id="20887-201">[drive][]</span></span>                        | <span data-ttu-id="20887-202">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="20887-202">Only present on document libraries.</span></span> <span data-ttu-id="20887-203">Разрешает доступ к списку как к ресурсу [drive][] с объектами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="20887-203">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="20887-204">**items**</span><span class="sxs-lookup"><span data-stu-id="20887-204">**items**</span></span>         | <span data-ttu-id="20887-205">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="20887-205">Collection([listItem][])</span></span>         | <span data-ttu-id="20887-206">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="20887-206">All items contained in the list.</span></span>
| <span data-ttu-id="20887-207">**columns**</span><span class="sxs-lookup"><span data-stu-id="20887-207">**columns**</span></span>       | <span data-ttu-id="20887-208">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="20887-208">Collection([columnDefinition][])</span></span> | <span data-ttu-id="20887-209">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="20887-209">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="20887-210">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="20887-210">**contentTypes**</span></span>  | <span data-ttu-id="20887-211">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="20887-211">Collection([contentType][])</span></span>      | <span data-ttu-id="20887-212">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="20887-212">The collection of content types present in this list.</span></span>

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
