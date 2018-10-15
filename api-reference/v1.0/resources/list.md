---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: List
ms.openlocfilehash: 9fa1de406a3c4064ccb410b4b5b2df91b54a1bac
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268461"
---
# <a name="list-resource"></a><span data-ttu-id="b52ff-102">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="b52ff-102">List resource</span></span>

<span data-ttu-id="b52ff-103">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="b52ff-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="b52ff-104">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="b52ff-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="b52ff-105">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="b52ff-105">Tasks on a list</span></span>

<span data-ttu-id="b52ff-106">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="b52ff-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="b52ff-107">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="b52ff-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="b52ff-108">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="b52ff-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="b52ff-109">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="b52ff-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="b52ff-110">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="b52ff-110">Common task</span></span>               | <span data-ttu-id="b52ff-111">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="b52ff-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="b52ff-112">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-112">[Get list][]</span></span>              | <span data-ttu-id="b52ff-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="b52ff-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="b52ff-114">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="b52ff-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="b52ff-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="b52ff-116">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-116">[Update list item][]</span></span>      | <span data-ttu-id="b52ff-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b52ff-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="b52ff-118">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-118">[Delete list item][]</span></span>      | <span data-ttu-id="b52ff-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b52ff-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="b52ff-120">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-120">[Create list item][]</span></span>      | <span data-ttu-id="b52ff-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="b52ff-121">POST /lists/{list-id}</span></span>

[Получение списка]: ../api/list_get.md
[Get list]: ../api/list_get.md
[Перечисление элементов списка]: ../api/listitem_list.md
[Enumerate list items]: ../api/listitem_list.md
[Обновление элемента списка]: ../api/listItem_update.md
[Update list item]: ../api/listItem_update.md
[Удаление элемента списка]: ../api/listItem_delete.md
[Delete list item]: ../api/listItem_delete.md
[Создание элемента в списке]: ../api/listItem_create.md
[Create list item]: ../api/listItem_create.md

## <a name="json-representation"></a><span data-ttu-id="b52ff-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b52ff-127">JSON representation</span></span>

<span data-ttu-id="b52ff-128">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b52ff-128">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b52ff-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="b52ff-129">Properties</span></span>

<span data-ttu-id="b52ff-130">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="b52ff-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="b52ff-131">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b52ff-131">Property name</span></span>    | <span data-ttu-id="b52ff-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b52ff-132">Type</span></span>                             | <span data-ttu-id="b52ff-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b52ff-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="b52ff-134">**displayName**</span><span class="sxs-lookup"><span data-stu-id="b52ff-134">**displayName**</span></span>  | <span data-ttu-id="b52ff-135">string</span><span class="sxs-lookup"><span data-stu-id="b52ff-135">string</span></span>                           | <span data-ttu-id="b52ff-136">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="b52ff-136">The displayable title of the list.</span></span>
| <span data-ttu-id="b52ff-137">**list**</span><span class="sxs-lookup"><span data-stu-id="b52ff-137">**list**</span></span>         | <span data-ttu-id="b52ff-138">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-138">[listInfo][]</span></span>                     | <span data-ttu-id="b52ff-139">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="b52ff-139">Provides additional details about the list.</span></span>
| <span data-ttu-id="b52ff-140">**system**</span><span class="sxs-lookup"><span data-stu-id="b52ff-140">**system**</span></span>       | <span data-ttu-id="b52ff-141">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-141">[systemFacet][]</span></span>                  | <span data-ttu-id="b52ff-142">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="b52ff-142">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="b52ff-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b52ff-143">Read-only.</span></span>

<span data-ttu-id="b52ff-144">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="b52ff-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="b52ff-145">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b52ff-145">Property name</span></span>            | <span data-ttu-id="b52ff-146">Тип</span><span class="sxs-lookup"><span data-stu-id="b52ff-146">Type</span></span>              | <span data-ttu-id="b52ff-147">Описание</span><span class="sxs-lookup"><span data-stu-id="b52ff-147">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="b52ff-148">**id**</span><span class="sxs-lookup"><span data-stu-id="b52ff-148">**id**</span></span>                   | <span data-ttu-id="b52ff-149">string</span><span class="sxs-lookup"><span data-stu-id="b52ff-149">string</span></span>            | <span data-ttu-id="b52ff-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b52ff-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="b52ff-152">**name**</span><span class="sxs-lookup"><span data-stu-id="b52ff-152">**name**</span></span>                 | <span data-ttu-id="b52ff-153">string</span><span class="sxs-lookup"><span data-stu-id="b52ff-153">string</span></span>            | <span data-ttu-id="b52ff-154">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="b52ff-154">The name of the item.</span></span>
| <span data-ttu-id="b52ff-155">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="b52ff-155">**createdBy**</span></span>            | <span data-ttu-id="b52ff-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-156">[identitySet][]</span></span>   | <span data-ttu-id="b52ff-157">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="b52ff-157">Identity of the creator of this item.</span></span> <span data-ttu-id="b52ff-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b52ff-158">Read-only.</span></span>
| <span data-ttu-id="b52ff-159">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="b52ff-159">**createdDateTime**</span></span>      | <span data-ttu-id="b52ff-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b52ff-160">DateTimeOffset</span></span>    | <span data-ttu-id="b52ff-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b52ff-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="b52ff-163">**description**</span><span class="sxs-lookup"><span data-stu-id="b52ff-163">**description**</span></span>          | <span data-ttu-id="b52ff-164">string</span><span class="sxs-lookup"><span data-stu-id="b52ff-164">string</span></span>            | <span data-ttu-id="b52ff-165">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="b52ff-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="b52ff-166">**|||UNTRANSLATED_CONTENT_START|||eTag|||UNTRANSLATED_CONTENT_END|||**</span><span class="sxs-lookup"><span data-stu-id="b52ff-166">**eTag**</span></span>                 | <span data-ttu-id="b52ff-167">string</span><span class="sxs-lookup"><span data-stu-id="b52ff-167">string</span></span>            | <span data-ttu-id="b52ff-p107">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b52ff-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="b52ff-170">**lastModifiedBy;**</span><span class="sxs-lookup"><span data-stu-id="b52ff-170">**lastModifiedBy**</span></span>       | <span data-ttu-id="b52ff-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-171">[identitySet][]</span></span>   | <span data-ttu-id="b52ff-172">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="b52ff-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="b52ff-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b52ff-173">Read-only.</span></span>
| <span data-ttu-id="b52ff-174">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b52ff-174">**lastModifiedDateTime**</span></span> | <span data-ttu-id="b52ff-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b52ff-175">DateTimeOffset</span></span>    | <span data-ttu-id="b52ff-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b52ff-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="b52ff-178">**|||UNTRANSLATED_CONTENT_START|||parentReference|||UNTRANSLATED_CONTENT_END|||**</span><span class="sxs-lookup"><span data-stu-id="b52ff-178">**parentReference**</span></span>      | <span data-ttu-id="b52ff-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-179">[itemReference][]</span></span> | <span data-ttu-id="b52ff-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="b52ff-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="b52ff-182">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="b52ff-182">**sharepointIds**</span></span>        | <span data-ttu-id="b52ff-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-183">[sharepointIds][]</span></span> | <span data-ttu-id="b52ff-p111">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b52ff-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="b52ff-186">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="b52ff-186">**webUrl**</span></span>               | <span data-ttu-id="b52ff-187">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="b52ff-187">string (url)</span></span>      | <span data-ttu-id="b52ff-p112">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b52ff-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="b52ff-190">Связи</span><span class="sxs-lookup"><span data-stu-id="b52ff-190">Relationships</span></span>

<span data-ttu-id="b52ff-191">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="b52ff-191">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="b52ff-192">Имя связи</span><span class="sxs-lookup"><span data-stu-id="b52ff-192">Relationship name</span></span> | <span data-ttu-id="b52ff-193">Тип</span><span class="sxs-lookup"><span data-stu-id="b52ff-193">Type</span></span>                             | <span data-ttu-id="b52ff-194">Описание</span><span class="sxs-lookup"><span data-stu-id="b52ff-194">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="b52ff-195">**drive**</span><span class="sxs-lookup"><span data-stu-id="b52ff-195">**drive**</span></span>         | <span data-ttu-id="b52ff-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="b52ff-196">[drive][]</span></span>                        | <span data-ttu-id="b52ff-197">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="b52ff-197">Only present on document libraries.</span></span> <span data-ttu-id="b52ff-198">Разрешает доступ к списку как к ресурсу [drive][] с ресурсами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="b52ff-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="b52ff-199">**items**</span><span class="sxs-lookup"><span data-stu-id="b52ff-199">**items**</span></span>         | <span data-ttu-id="b52ff-200">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="b52ff-200">Collection([listItem][])</span></span>         | <span data-ttu-id="b52ff-201">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="b52ff-201">All items contained in the list.</span></span>
| <span data-ttu-id="b52ff-202">**столбцы**</span><span class="sxs-lookup"><span data-stu-id="b52ff-202">**columns**</span></span>       | <span data-ttu-id="b52ff-203">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="b52ff-203">Collection([columnDefinition][])</span></span> | <span data-ttu-id="b52ff-204">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="b52ff-204">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="b52ff-205">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="b52ff-205">**contentTypes**</span></span>  | <span data-ttu-id="b52ff-206">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="b52ff-206">Collection([contentType][])</span></span>      | <span data-ttu-id="b52ff-207">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="b52ff-207">The collection of content types present in this list.</span></span>

[baseItem]: baseItem.md
[contentType]: contentType.md
[drive]: drive.md
[driveItem]: driveItem.md
[columnDefinition]: columnDefinition.md
[identitySet]: identitySet.md
[itemReference]: itemreference.md
[listInfo]: listInfo.md
[listItem]: listItem.md
[sharepointIds]: sharepointIds.md
[сайте]: site.md
[site]: site.md
[systemFacet]: systemFacet.md

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
