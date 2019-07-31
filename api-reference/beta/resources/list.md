---
author: JeremyKelley
description: Ресурс list представляет список в ресурсе site.
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b79172049278758c77ac620f00c391d52633792b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009995"
---
# <a name="list-resource"></a><span data-ttu-id="97d3e-103">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="97d3e-103">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97d3e-104">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="97d3e-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="97d3e-105">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="97d3e-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="97d3e-106">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="97d3e-106">Tasks on a list</span></span>

<span data-ttu-id="97d3e-107">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="97d3e-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="97d3e-108">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="97d3e-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="97d3e-109">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="97d3e-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="97d3e-110">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="97d3e-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="97d3e-111">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="97d3e-111">Common task</span></span>               | <span data-ttu-id="97d3e-112">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="97d3e-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="97d3e-113">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-113">[Get list][]</span></span>              | <span data-ttu-id="97d3e-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="97d3e-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="97d3e-115">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-115">[Enumerate list items][]</span></span>  | <span data-ttu-id="97d3e-116">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="97d3e-116">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="97d3e-117">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-117">[Update list item][]</span></span>      | <span data-ttu-id="97d3e-118">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="97d3e-118">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="97d3e-119">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-119">[Delete list item][]</span></span>      | <span data-ttu-id="97d3e-120">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="97d3e-120">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="97d3e-121">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-121">[Create list item][]</span></span>      | <span data-ttu-id="97d3e-122">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="97d3e-122">POST /lists/{list-id}</span></span>
| <span data-ttu-id="97d3e-123">[Получение последних действий][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-123">[Get recent activities][]</span></span> | <span data-ttu-id="97d3e-124">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="97d3e-124">GET /lists/{list-id}/activities</span></span>

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
[Получение последних действий]: ../api/activities-list.md
[Get recent activities]: ../api/activities-list.md

## <a name="json-representation"></a><span data-ttu-id="97d3e-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="97d3e-131">JSON representation</span></span>

<span data-ttu-id="97d3e-132">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97d3e-132">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="97d3e-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="97d3e-133">Properties</span></span>

<span data-ttu-id="97d3e-134">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="97d3e-134">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="97d3e-135">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="97d3e-135">Property name</span></span>    | <span data-ttu-id="97d3e-136">Тип</span><span class="sxs-lookup"><span data-stu-id="97d3e-136">Type</span></span>                             | <span data-ttu-id="97d3e-137">Описание</span><span class="sxs-lookup"><span data-stu-id="97d3e-137">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="97d3e-138">**columns**</span><span class="sxs-lookup"><span data-stu-id="97d3e-138">**columns**</span></span>      | <span data-ttu-id="97d3e-139">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="97d3e-139">Collection([columnDefinition][])</span></span> | <span data-ttu-id="97d3e-140">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="97d3e-140">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="97d3e-141">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="97d3e-141">**contentTypes**</span></span> | <span data-ttu-id="97d3e-142">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="97d3e-142">Collection([contentType][])</span></span>      | <span data-ttu-id="97d3e-143">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="97d3e-143">The collection of content types present in this list.</span></span>
| <span data-ttu-id="97d3e-144">**displayName**</span><span class="sxs-lookup"><span data-stu-id="97d3e-144">**displayName**</span></span>  | <span data-ttu-id="97d3e-145">строка</span><span class="sxs-lookup"><span data-stu-id="97d3e-145">string</span></span>                           | <span data-ttu-id="97d3e-146">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="97d3e-146">The displayable title of the list.</span></span>
| <span data-ttu-id="97d3e-147">**list**</span><span class="sxs-lookup"><span data-stu-id="97d3e-147">**list**</span></span>         | <span data-ttu-id="97d3e-148">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-148">[listInfo][]</span></span>                     | <span data-ttu-id="97d3e-149">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="97d3e-149">Provides additional details about the list.</span></span>
| <span data-ttu-id="97d3e-150">**system**</span><span class="sxs-lookup"><span data-stu-id="97d3e-150">**system**</span></span>       | <span data-ttu-id="97d3e-151">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-151">[systemFacet][]</span></span>                  | <span data-ttu-id="97d3e-152">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="97d3e-152">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="97d3e-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3e-153">Read-only.</span></span>

<span data-ttu-id="97d3e-154">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="97d3e-154">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="97d3e-155">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="97d3e-155">Property name</span></span>            | <span data-ttu-id="97d3e-156">Тип</span><span class="sxs-lookup"><span data-stu-id="97d3e-156">Type</span></span>             | <span data-ttu-id="97d3e-157">Описание</span><span class="sxs-lookup"><span data-stu-id="97d3e-157">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="97d3e-158">**id**</span><span class="sxs-lookup"><span data-stu-id="97d3e-158">**id**</span></span>                   | <span data-ttu-id="97d3e-159">string</span><span class="sxs-lookup"><span data-stu-id="97d3e-159">string</span></span>           | <span data-ttu-id="97d3e-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3e-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="97d3e-162">**name**</span><span class="sxs-lookup"><span data-stu-id="97d3e-162">**name**</span></span>                 | <span data-ttu-id="97d3e-163">string</span><span class="sxs-lookup"><span data-stu-id="97d3e-163">string</span></span>           | <span data-ttu-id="97d3e-164">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="97d3e-164">The name of the item.</span></span>
| <span data-ttu-id="97d3e-165">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="97d3e-165">**createdBy**</span></span>            | <span data-ttu-id="97d3e-166">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-166">[identitySet][]</span></span>  | <span data-ttu-id="97d3e-167">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="97d3e-167">Identity of the creator of this item.</span></span> <span data-ttu-id="97d3e-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3e-168">Read-only.</span></span>
| <span data-ttu-id="97d3e-169">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="97d3e-169">**createdDateTime**</span></span>      | <span data-ttu-id="97d3e-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d3e-170">DateTimeOffset</span></span>   | <span data-ttu-id="97d3e-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3e-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="97d3e-173">**description**</span><span class="sxs-lookup"><span data-stu-id="97d3e-173">**description**</span></span>          | <span data-ttu-id="97d3e-174">строка</span><span class="sxs-lookup"><span data-stu-id="97d3e-174">string</span></span>           | <span data-ttu-id="97d3e-175">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="97d3e-175">The descriptive text for the item.</span></span>
| <span data-ttu-id="97d3e-176">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="97d3e-176">**lastModifiedBy**</span></span>       | <span data-ttu-id="97d3e-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-177">[identitySet][]</span></span>  | <span data-ttu-id="97d3e-178">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="97d3e-178">Identity of the last modifier of this item.</span></span> <span data-ttu-id="97d3e-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3e-179">Read-only.</span></span>
| <span data-ttu-id="97d3e-180">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="97d3e-180">**lastModifiedDateTime**</span></span> | <span data-ttu-id="97d3e-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d3e-181">DateTimeOffset</span></span>   | <span data-ttu-id="97d3e-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3e-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="97d3e-184">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="97d3e-184">**webUrl**</span></span>               | <span data-ttu-id="97d3e-185">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="97d3e-185">string (url)</span></span>     | <span data-ttu-id="97d3e-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3e-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="97d3e-188">Связи</span><span class="sxs-lookup"><span data-stu-id="97d3e-188">Relationships</span></span>

<span data-ttu-id="97d3e-189">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="97d3e-189">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="97d3e-190">Имя связи</span><span class="sxs-lookup"><span data-stu-id="97d3e-190">Relationship name</span></span> | <span data-ttu-id="97d3e-191">Тип</span><span class="sxs-lookup"><span data-stu-id="97d3e-191">Type</span></span>                        | <span data-ttu-id="97d3e-192">Описание</span><span class="sxs-lookup"><span data-stu-id="97d3e-192">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="97d3e-193">**activities**</span><span class="sxs-lookup"><span data-stu-id="97d3e-193">**activities**</span></span>    | <span data-ttu-id="97d3e-194">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-194">[itemActivity][] collection</span></span> | <span data-ttu-id="97d3e-195">Последние действия, выполненные в списке.</span><span class="sxs-lookup"><span data-stu-id="97d3e-195">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="97d3e-196">**drive**</span><span class="sxs-lookup"><span data-stu-id="97d3e-196">**drive**</span></span>         | <span data-ttu-id="97d3e-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="97d3e-197">[drive][]</span></span>                   | <span data-ttu-id="97d3e-198">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="97d3e-198">Only present on document libraries.</span></span> <span data-ttu-id="97d3e-199">Разрешает доступ к списку как к ресурсу [drive][] с ресурсами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="97d3e-199">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="97d3e-200">**items**</span><span class="sxs-lookup"><span data-stu-id="97d3e-200">**items**</span></span>         | <span data-ttu-id="97d3e-201">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="97d3e-201">Collection([listItem][])</span></span>    | <span data-ttu-id="97d3e-202">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="97d3e-202">All items contained in the list.</span></span>

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
