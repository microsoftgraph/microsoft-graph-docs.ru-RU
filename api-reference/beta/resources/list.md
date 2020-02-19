---
author: JeremyKelley
description: Ресурс list представляет список на сайте.
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4df869eeba7b66dad0bddef48b7d5686d8899702
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108464"
---
# <a name="list-resource"></a><span data-ttu-id="e7643-103">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="e7643-103">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7643-104">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="e7643-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="e7643-105">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="e7643-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="e7643-106">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="e7643-106">Tasks on a list</span></span>

<span data-ttu-id="e7643-107">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="e7643-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="e7643-108">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="e7643-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="e7643-109">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="e7643-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="e7643-110">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="e7643-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="e7643-111">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="e7643-111">Common task</span></span>               | <span data-ttu-id="e7643-112">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="e7643-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="e7643-113">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="e7643-113">[Get list][]</span></span>              | <span data-ttu-id="e7643-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="e7643-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="e7643-115">[Создание списка][]</span><span class="sxs-lookup"><span data-stu-id="e7643-115">[Create list][]</span></span>           | <span data-ttu-id="e7643-116">POST/листс</span><span class="sxs-lookup"><span data-stu-id="e7643-116">POST /lists</span></span>
| <span data-ttu-id="e7643-117">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="e7643-117">[Enumerate list items][]</span></span>  | <span data-ttu-id="e7643-118">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="e7643-118">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="e7643-119">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="e7643-119">[Update list item][]</span></span>      | <span data-ttu-id="e7643-120">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="e7643-120">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="e7643-121">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="e7643-121">[Delete list item][]</span></span>      | <span data-ttu-id="e7643-122">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="e7643-122">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="e7643-123">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="e7643-123">[Create list item][]</span></span>      | <span data-ttu-id="e7643-124">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="e7643-124">POST /lists/{list-id}</span></span>
| <span data-ttu-id="e7643-125">[Получение последних действий][]</span><span class="sxs-lookup"><span data-stu-id="e7643-125">[Get recent activities][]</span></span> | <span data-ttu-id="e7643-126">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="e7643-126">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="e7643-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e7643-134">JSON representation</span></span>

<span data-ttu-id="e7643-135">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7643-135">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e7643-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7643-136">Properties</span></span>

<span data-ttu-id="e7643-137">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="e7643-137">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="e7643-138">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e7643-138">Property name</span></span>    | <span data-ttu-id="e7643-139">Тип</span><span class="sxs-lookup"><span data-stu-id="e7643-139">Type</span></span>                             | <span data-ttu-id="e7643-140">Описание</span><span class="sxs-lookup"><span data-stu-id="e7643-140">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="e7643-141">**columns**</span><span class="sxs-lookup"><span data-stu-id="e7643-141">**columns**</span></span>      | <span data-ttu-id="e7643-142">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="e7643-142">Collection([columnDefinition][])</span></span> | <span data-ttu-id="e7643-143">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="e7643-143">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="e7643-144">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="e7643-144">**contentTypes**</span></span> | <span data-ttu-id="e7643-145">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="e7643-145">Collection([contentType][])</span></span>      | <span data-ttu-id="e7643-146">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="e7643-146">The collection of content types present in this list.</span></span>
| <span data-ttu-id="e7643-147">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e7643-147">**displayName**</span></span>  | <span data-ttu-id="e7643-148">строка</span><span class="sxs-lookup"><span data-stu-id="e7643-148">string</span></span>                           | <span data-ttu-id="e7643-149">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="e7643-149">The displayable title of the list.</span></span>
| <span data-ttu-id="e7643-150">**list**</span><span class="sxs-lookup"><span data-stu-id="e7643-150">**list**</span></span>         | <span data-ttu-id="e7643-151">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="e7643-151">[listInfo][]</span></span>                     | <span data-ttu-id="e7643-152">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="e7643-152">Provides additional details about the list.</span></span>
| <span data-ttu-id="e7643-153">**system**</span><span class="sxs-lookup"><span data-stu-id="e7643-153">**system**</span></span>       | <span data-ttu-id="e7643-154">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="e7643-154">[systemFacet][]</span></span>                  | <span data-ttu-id="e7643-155">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="e7643-155">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="e7643-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7643-156">Read-only.</span></span>

<span data-ttu-id="e7643-157">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="e7643-157">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="e7643-158">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e7643-158">Property name</span></span>            | <span data-ttu-id="e7643-159">Тип</span><span class="sxs-lookup"><span data-stu-id="e7643-159">Type</span></span>             | <span data-ttu-id="e7643-160">Описание</span><span class="sxs-lookup"><span data-stu-id="e7643-160">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="e7643-161">**id**</span><span class="sxs-lookup"><span data-stu-id="e7643-161">**id**</span></span>                   | <span data-ttu-id="e7643-162">string</span><span class="sxs-lookup"><span data-stu-id="e7643-162">string</span></span>           | <span data-ttu-id="e7643-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7643-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="e7643-165">**name**</span><span class="sxs-lookup"><span data-stu-id="e7643-165">**name**</span></span>                 | <span data-ttu-id="e7643-166">string</span><span class="sxs-lookup"><span data-stu-id="e7643-166">string</span></span>           | <span data-ttu-id="e7643-167">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="e7643-167">The name of the item.</span></span>
| <span data-ttu-id="e7643-168">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="e7643-168">**createdBy**</span></span>            | <span data-ttu-id="e7643-169">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e7643-169">[identitySet][]</span></span>  | <span data-ttu-id="e7643-170">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="e7643-170">Identity of the creator of this item.</span></span> <span data-ttu-id="e7643-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7643-171">Read-only.</span></span>
| <span data-ttu-id="e7643-172">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="e7643-172">**createdDateTime**</span></span>      | <span data-ttu-id="e7643-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7643-173">DateTimeOffset</span></span>   | <span data-ttu-id="e7643-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7643-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="e7643-176">**description**</span><span class="sxs-lookup"><span data-stu-id="e7643-176">**description**</span></span>          | <span data-ttu-id="e7643-177">строка</span><span class="sxs-lookup"><span data-stu-id="e7643-177">string</span></span>           | <span data-ttu-id="e7643-178">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="e7643-178">The descriptive text for the item.</span></span>
| <span data-ttu-id="e7643-179">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="e7643-179">**lastModifiedBy**</span></span>       | <span data-ttu-id="e7643-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e7643-180">[identitySet][]</span></span>  | <span data-ttu-id="e7643-181">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="e7643-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="e7643-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7643-182">Read-only.</span></span>
| <span data-ttu-id="e7643-183">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e7643-183">**lastModifiedDateTime**</span></span> | <span data-ttu-id="e7643-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7643-184">DateTimeOffset</span></span>   | <span data-ttu-id="e7643-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7643-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="e7643-187">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="e7643-187">**webUrl**</span></span>               | <span data-ttu-id="e7643-188">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="e7643-188">string (url)</span></span>     | <span data-ttu-id="e7643-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7643-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="e7643-191">Связи</span><span class="sxs-lookup"><span data-stu-id="e7643-191">Relationships</span></span>

<span data-ttu-id="e7643-192">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="e7643-192">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="e7643-193">Имя связи</span><span class="sxs-lookup"><span data-stu-id="e7643-193">Relationship name</span></span> | <span data-ttu-id="e7643-194">Тип</span><span class="sxs-lookup"><span data-stu-id="e7643-194">Type</span></span>                        | <span data-ttu-id="e7643-195">Описание</span><span class="sxs-lookup"><span data-stu-id="e7643-195">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="e7643-196">**activities**</span><span class="sxs-lookup"><span data-stu-id="e7643-196">**activities**</span></span>    | <span data-ttu-id="e7643-197">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="e7643-197">[itemActivity][] collection</span></span> | <span data-ttu-id="e7643-198">Последние действия, выполненные в списке.</span><span class="sxs-lookup"><span data-stu-id="e7643-198">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="e7643-199">**drive**</span><span class="sxs-lookup"><span data-stu-id="e7643-199">**drive**</span></span>         | <span data-ttu-id="e7643-200">[drive][]</span><span class="sxs-lookup"><span data-stu-id="e7643-200">[drive][]</span></span>                   | <span data-ttu-id="e7643-201">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="e7643-201">Only present on document libraries.</span></span> <span data-ttu-id="e7643-202">Разрешает доступ к списку как к ресурсу [drive][] с объектами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="e7643-202">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="e7643-203">**items**</span><span class="sxs-lookup"><span data-stu-id="e7643-203">**items**</span></span>         | <span data-ttu-id="e7643-204">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="e7643-204">Collection([listItem][])</span></span>    | <span data-ttu-id="e7643-205">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="e7643-205">All items contained in the list.</span></span>

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
