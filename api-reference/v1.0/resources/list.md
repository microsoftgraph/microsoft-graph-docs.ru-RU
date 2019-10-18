---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Перечисление
localization_priority: Priority
ms.prod: sharepoint
description: Ресурс list представляет список на сайте.
doc_type: resourcePageType
ms.openlocfilehash: 51821bb20188c004af3f2aca868c3cfd953ce19c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036409"
---
# <a name="list-resource"></a><span data-ttu-id="eec69-103">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="eec69-103">List resource</span></span>

<span data-ttu-id="eec69-104">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="eec69-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="eec69-105">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="eec69-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="eec69-106">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="eec69-106">Tasks on a list</span></span>

<span data-ttu-id="eec69-107">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="eec69-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="eec69-108">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="eec69-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="eec69-109">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="eec69-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="eec69-110">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="eec69-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="eec69-111">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="eec69-111">Common task</span></span>               | <span data-ttu-id="eec69-112">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="eec69-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="eec69-113">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="eec69-113">[Get list][]</span></span>              | <span data-ttu-id="eec69-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="eec69-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="eec69-115">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="eec69-115">[Enumerate list items][]</span></span>  | <span data-ttu-id="eec69-116">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="eec69-116">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="eec69-117">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="eec69-117">[Update list item][]</span></span>      | <span data-ttu-id="eec69-118">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="eec69-118">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="eec69-119">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="eec69-119">[Delete list item][]</span></span>      | <span data-ttu-id="eec69-120">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="eec69-120">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="eec69-121">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="eec69-121">[Create list item][]</span></span>      | <span data-ttu-id="eec69-122">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="eec69-122">POST /lists/{list-id}</span></span>

[Получение списка]: ../api/list-get.md
[Get list]: ../api/list-get.md
[Перечисление элементов списка]: ../api/listitem-list.md
[Enumerate list items]: ../api/listitem-list.md
[Обновление элемента списка]: ../api/listitem-update.md
[Update list item]: ../api/listitem-update.md
[Удаление элемента списка]: ../api/listitem-delete.md
[Delete list item]: ../api/listitem-delete.md
[Создание элемента в списке]: ../api/listitem-create.md
[Create list item]: ../api/listitem-create.md

## <a name="json-representation"></a><span data-ttu-id="eec69-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="eec69-128">JSON representation</span></span>

<span data-ttu-id="eec69-129">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eec69-129">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="eec69-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="eec69-130">Properties</span></span>

<span data-ttu-id="eec69-131">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="eec69-131">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="eec69-132">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="eec69-132">Property name</span></span>    | <span data-ttu-id="eec69-133">Тип</span><span class="sxs-lookup"><span data-stu-id="eec69-133">Type</span></span>                             | <span data-ttu-id="eec69-134">Описание</span><span class="sxs-lookup"><span data-stu-id="eec69-134">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="eec69-135">**displayName**</span><span class="sxs-lookup"><span data-stu-id="eec69-135">**displayName**</span></span>  | <span data-ttu-id="eec69-136">строка</span><span class="sxs-lookup"><span data-stu-id="eec69-136">string</span></span>                           | <span data-ttu-id="eec69-137">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="eec69-137">The displayable title of the list.</span></span>
| <span data-ttu-id="eec69-138">**list**</span><span class="sxs-lookup"><span data-stu-id="eec69-138">**list**</span></span>         | <span data-ttu-id="eec69-139">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="eec69-139">[listInfo][]</span></span>                     | <span data-ttu-id="eec69-140">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="eec69-140">Provides additional details about the list.</span></span>
| <span data-ttu-id="eec69-141">**system**</span><span class="sxs-lookup"><span data-stu-id="eec69-141">**system**</span></span>       | <span data-ttu-id="eec69-142">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="eec69-142">[systemFacet][]</span></span>                  | <span data-ttu-id="eec69-143">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="eec69-143">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="eec69-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eec69-144">Read-only.</span></span>

<span data-ttu-id="eec69-145">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="eec69-145">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="eec69-146">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="eec69-146">Property name</span></span>            | <span data-ttu-id="eec69-147">Тип</span><span class="sxs-lookup"><span data-stu-id="eec69-147">Type</span></span>              | <span data-ttu-id="eec69-148">Описание</span><span class="sxs-lookup"><span data-stu-id="eec69-148">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="eec69-149">**id**</span><span class="sxs-lookup"><span data-stu-id="eec69-149">**id**</span></span>                   | <span data-ttu-id="eec69-150">string</span><span class="sxs-lookup"><span data-stu-id="eec69-150">string</span></span>            | <span data-ttu-id="eec69-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eec69-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="eec69-153">**name**</span><span class="sxs-lookup"><span data-stu-id="eec69-153">**name**</span></span>                 | <span data-ttu-id="eec69-154">строка</span><span class="sxs-lookup"><span data-stu-id="eec69-154">string</span></span>            | <span data-ttu-id="eec69-155">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="eec69-155">The name of the item.</span></span>
| <span data-ttu-id="eec69-156">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="eec69-156">**createdBy**</span></span>            | <span data-ttu-id="eec69-157">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="eec69-157">[identitySet][]</span></span>   | <span data-ttu-id="eec69-158">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="eec69-158">Identity of the creator of this item.</span></span> <span data-ttu-id="eec69-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eec69-159">Read-only.</span></span>
| <span data-ttu-id="eec69-160">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="eec69-160">**createdDateTime**</span></span>      | <span data-ttu-id="eec69-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eec69-161">DateTimeOffset</span></span>    | <span data-ttu-id="eec69-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eec69-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="eec69-164">**description**</span><span class="sxs-lookup"><span data-stu-id="eec69-164">**description**</span></span>          | <span data-ttu-id="eec69-165">строка</span><span class="sxs-lookup"><span data-stu-id="eec69-165">string</span></span>            | <span data-ttu-id="eec69-166">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="eec69-166">The descriptive text for the item.</span></span>
| <span data-ttu-id="eec69-167">**eTag**</span><span class="sxs-lookup"><span data-stu-id="eec69-167">**eTag**</span></span>                 | <span data-ttu-id="eec69-168">string</span><span class="sxs-lookup"><span data-stu-id="eec69-168">string</span></span>            | <span data-ttu-id="eec69-p107">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eec69-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="eec69-171">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="eec69-171">**lastModifiedBy**</span></span>       | <span data-ttu-id="eec69-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="eec69-172">[identitySet][]</span></span>   | <span data-ttu-id="eec69-173">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="eec69-173">Identity of the last modifier of this item.</span></span> <span data-ttu-id="eec69-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eec69-174">Read-only.</span></span>
| <span data-ttu-id="eec69-175">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="eec69-175">**lastModifiedDateTime**</span></span> | <span data-ttu-id="eec69-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eec69-176">DateTimeOffset</span></span>    | <span data-ttu-id="eec69-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eec69-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="eec69-179">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="eec69-179">**parentReference**</span></span>      | <span data-ttu-id="eec69-180">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="eec69-180">[itemReference][]</span></span> | <span data-ttu-id="eec69-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="eec69-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="eec69-183">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="eec69-183">**sharepointIds**</span></span>        | <span data-ttu-id="eec69-184">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="eec69-184">[sharepointIds][]</span></span> | <span data-ttu-id="eec69-p111">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eec69-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="eec69-187">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="eec69-187">**webUrl**</span></span>               | <span data-ttu-id="eec69-188">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="eec69-188">string (url)</span></span>      | <span data-ttu-id="eec69-p112">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eec69-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="eec69-191">Связи</span><span class="sxs-lookup"><span data-stu-id="eec69-191">Relationships</span></span>

<span data-ttu-id="eec69-192">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="eec69-192">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="eec69-193">Имя связи</span><span class="sxs-lookup"><span data-stu-id="eec69-193">Relationship name</span></span> | <span data-ttu-id="eec69-194">Тип</span><span class="sxs-lookup"><span data-stu-id="eec69-194">Type</span></span>                             | <span data-ttu-id="eec69-195">Описание</span><span class="sxs-lookup"><span data-stu-id="eec69-195">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="eec69-196">**drive**</span><span class="sxs-lookup"><span data-stu-id="eec69-196">**drive**</span></span>         | <span data-ttu-id="eec69-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="eec69-197">[drive][]</span></span>                        | <span data-ttu-id="eec69-198">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="eec69-198">Only present on document libraries.</span></span> <span data-ttu-id="eec69-199">Разрешает доступ к списку как к ресурсу [drive][] с объектами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="eec69-199">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="eec69-200">**items**</span><span class="sxs-lookup"><span data-stu-id="eec69-200">**items**</span></span>         | <span data-ttu-id="eec69-201">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="eec69-201">Collection([listItem][])</span></span>         | <span data-ttu-id="eec69-202">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="eec69-202">All items contained in the list.</span></span>
| <span data-ttu-id="eec69-203">**columns**</span><span class="sxs-lookup"><span data-stu-id="eec69-203">**columns**</span></span>       | <span data-ttu-id="eec69-204">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="eec69-204">Collection([columnDefinition][])</span></span> | <span data-ttu-id="eec69-205">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="eec69-205">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="eec69-206">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="eec69-206">**contentTypes**</span></span>  | <span data-ttu-id="eec69-207">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="eec69-207">Collection([contentType][])</span></span>      | <span data-ttu-id="eec69-208">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="eec69-208">The collection of content types present in this list.</span></span>

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
