---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: List
ms.openlocfilehash: ba0c01ce1887a32bd8b671cf511104e9128b5efb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="list-resource"></a><span data-ttu-id="daf8f-102">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="daf8f-102">List resource</span></span>

<span data-ttu-id="daf8f-103">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="daf8f-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="daf8f-104">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="daf8f-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="daf8f-105">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="daf8f-105">Tasks on a list</span></span>

<span data-ttu-id="daf8f-106">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="daf8f-106">The following tasks are available for {type} resources.</span></span>
<span data-ttu-id="daf8f-107">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="daf8f-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="daf8f-108">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="daf8f-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="daf8f-109">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="daf8f-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="daf8f-110">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="daf8f-110">Common task</span></span>               | <span data-ttu-id="daf8f-111">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="daf8f-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="daf8f-112">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="daf8f-112">[Get list][]</span></span>              | <span data-ttu-id="daf8f-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="daf8f-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="daf8f-114">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="daf8f-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="daf8f-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="daf8f-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="daf8f-116">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="daf8f-116">[Update list item][]</span></span>      | <span data-ttu-id="daf8f-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="daf8f-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="daf8f-118">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="daf8f-118">[Delete list item][]</span></span>      | <span data-ttu-id="daf8f-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="daf8f-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="daf8f-120">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="daf8f-120">[Create list item][]</span></span>      | <span data-ttu-id="daf8f-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="daf8f-121">POST /lists/{list-id}</span></span>

[Получение списка]: ../api/list_get.md
[Перечисление элементов списка]: ../api/listitem_list.md
[Обновление элемента списка]: ../api/listItem_update.md
[Удаление элемента списка]: ../api/listItem_delete.md
[Создание элемента в списке]: ../api/listItem_create.md

## <a name="json-representation"></a><span data-ttu-id="daf8f-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="daf8f-127">JSON representation</span></span>

<span data-ttu-id="daf8f-128">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daf8f-128">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

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
    "template": "documentLibrary | genericList | survey | links | announcements | contacts ..."
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
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="daf8f-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="daf8f-129">Properties</span></span>

<span data-ttu-id="daf8f-130">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="daf8f-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="daf8f-131">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="daf8f-131">Property name</span></span>    | <span data-ttu-id="daf8f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="daf8f-132">Type</span></span>                             | <span data-ttu-id="daf8f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="daf8f-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="daf8f-134">**columns**</span><span class="sxs-lookup"><span data-stu-id="daf8f-134">**columns**</span></span>      | <span data-ttu-id="daf8f-135">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="daf8f-135">Collection([columnDefinition][])</span></span> | <span data-ttu-id="daf8f-136">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="daf8f-136">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="daf8f-137">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="daf8f-137"><ContentTypes></span></span> | <span data-ttu-id="daf8f-138">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="daf8f-138">Collection([contentType][])</span></span>      | <span data-ttu-id="daf8f-139">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="daf8f-139">The collection of content types present in this list.</span></span>
| <span data-ttu-id="daf8f-140">**displayName**</span><span class="sxs-lookup"><span data-stu-id="daf8f-140">**displayName**</span></span>  | <span data-ttu-id="daf8f-141">строка</span><span class="sxs-lookup"><span data-stu-id="daf8f-141">string</span></span>                           | <span data-ttu-id="daf8f-142">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="daf8f-142">The new title of the list.</span></span>
| <span data-ttu-id="daf8f-143">**list**</span><span class="sxs-lookup"><span data-stu-id="daf8f-143">**list**</span></span>         | <span data-ttu-id="daf8f-144">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="daf8f-144">[listInfo][]</span></span>                     | <span data-ttu-id="daf8f-145">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="daf8f-145">Provides additional details about the list.</span></span>
| <span data-ttu-id="daf8f-146">**system**</span><span class="sxs-lookup"><span data-stu-id="daf8f-146">**System**</span></span>       | <span data-ttu-id="daf8f-147">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="daf8f-147">[systemFacet][]</span></span>                  | <span data-ttu-id="daf8f-148">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="daf8f-148">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="daf8f-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daf8f-149">Read-only.</span></span>

<span data-ttu-id="daf8f-150">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="daf8f-150">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="daf8f-151">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="daf8f-151">Property name</span></span>            | <span data-ttu-id="daf8f-152">Тип</span><span class="sxs-lookup"><span data-stu-id="daf8f-152">Type</span></span>             | <span data-ttu-id="daf8f-153">Описание</span><span class="sxs-lookup"><span data-stu-id="daf8f-153">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="daf8f-154">**id**</span><span class="sxs-lookup"><span data-stu-id="daf8f-154">**id**</span></span>                   | <span data-ttu-id="daf8f-155">string</span><span class="sxs-lookup"><span data-stu-id="daf8f-155">string</span></span>           | <span data-ttu-id="daf8f-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daf8f-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="daf8f-158">**name**</span><span class="sxs-lookup"><span data-stu-id="daf8f-158">**name**</span></span>                 | <span data-ttu-id="daf8f-159">строка</span><span class="sxs-lookup"><span data-stu-id="daf8f-159">string</span></span>           | <span data-ttu-id="daf8f-160">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="daf8f-160">The name of the named item.</span></span>
| <span data-ttu-id="daf8f-161">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="daf8f-161">**createdBy**</span></span>            | <span data-ttu-id="daf8f-162">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="daf8f-162">[identitySet][]</span></span>  | <span data-ttu-id="daf8f-163">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="daf8f-163">Identity of the creator of this item.</span></span> <span data-ttu-id="daf8f-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daf8f-164">Read-only.</span></span>
| <span data-ttu-id="daf8f-165">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="daf8f-165">**createdDateTime**</span></span>      | <span data-ttu-id="daf8f-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="daf8f-166">DateTimeOffset</span></span>   | <span data-ttu-id="daf8f-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daf8f-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="daf8f-169">**description**</span><span class="sxs-lookup"><span data-stu-id="daf8f-169">**description**</span></span>          | <span data-ttu-id="daf8f-170">строка</span><span class="sxs-lookup"><span data-stu-id="daf8f-170">string</span></span>           | <span data-ttu-id="daf8f-171">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="daf8f-171">The descriptive text for the site.</span></span>
| <span data-ttu-id="daf8f-172">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="daf8f-172">**lastModifiedBy**</span></span>       | <span data-ttu-id="daf8f-173">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="daf8f-173">[identitySet][]</span></span>  | <span data-ttu-id="daf8f-174">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="daf8f-174">Identity of the last modifier of this item.</span></span> <span data-ttu-id="daf8f-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daf8f-175">Read-only.</span></span>
| <span data-ttu-id="daf8f-176">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="daf8f-176">**lastModifiedDateTime**</span></span> | <span data-ttu-id="daf8f-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="daf8f-177">DateTimeOffset</span></span>   | <span data-ttu-id="daf8f-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daf8f-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="daf8f-180">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="daf8f-180">**webUrl**</span></span>               | <span data-ttu-id="daf8f-181">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="daf8f-181">string (url)</span></span>     | <span data-ttu-id="daf8f-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daf8f-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="daf8f-184">Связи</span><span class="sxs-lookup"><span data-stu-id="daf8f-184">Relationships</span></span>

<span data-ttu-id="daf8f-185">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="daf8f-185">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="daf8f-186">Имя связи</span><span class="sxs-lookup"><span data-stu-id="daf8f-186">Relationship name</span></span> | <span data-ttu-id="daf8f-187">Тип</span><span class="sxs-lookup"><span data-stu-id="daf8f-187">Type</span></span>                        | <span data-ttu-id="daf8f-188">Описание</span><span class="sxs-lookup"><span data-stu-id="daf8f-188">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="daf8f-189">**drive**</span><span class="sxs-lookup"><span data-stu-id="daf8f-189">**drive**</span></span>         | <span data-ttu-id="daf8f-190">[drive][]</span><span class="sxs-lookup"><span data-stu-id="daf8f-190">[drive][]</span></span>                   | <span data-ttu-id="daf8f-191">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="daf8f-191">Only present on document libraries.</span></span> <span data-ttu-id="daf8f-192">Разрешает доступ к списку как к ресурсу [drive][] с ресурсами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="daf8f-192">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="daf8f-193">**items**</span><span class="sxs-lookup"><span data-stu-id="daf8f-193">**items**</span></span>         | <span data-ttu-id="daf8f-194">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="daf8f-194">Collection([listItem][])</span></span>    | <span data-ttu-id="daf8f-195">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="daf8f-195">All items contained in the drive.</span></span>

[baseItem]: baseItem.md
[contentType]: contentType.md
[drive]: drive.md
[driveItem]: driveItem.md
[columnDefinition]: columnDefinition.md
[identitySet]: identitySet.md
[listInfo]: listInfo.md
[listItem]: listItem.md
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
