---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5e078c79603235059cbe326c850e51dfa33d2f8e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345348"
---
# <a name="list-resource"></a><span data-ttu-id="16180-102">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="16180-102">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16180-103">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="16180-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="16180-104">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="16180-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="16180-105">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="16180-105">Tasks on a list</span></span>

<span data-ttu-id="16180-106">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="16180-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="16180-107">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="16180-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="16180-108">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="16180-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="16180-109">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="16180-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="16180-110">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="16180-110">Common task</span></span>               | <span data-ttu-id="16180-111">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="16180-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="16180-112">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="16180-112">[Get list][]</span></span>              | <span data-ttu-id="16180-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="16180-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="16180-114">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="16180-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="16180-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="16180-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="16180-116">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="16180-116">[Update list item][]</span></span>      | <span data-ttu-id="16180-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="16180-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="16180-118">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="16180-118">[Delete list item][]</span></span>      | <span data-ttu-id="16180-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="16180-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="16180-120">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="16180-120">[Create list item][]</span></span>      | <span data-ttu-id="16180-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="16180-121">POST /lists/{list-id}</span></span>
| <span data-ttu-id="16180-122">[Получение последних действий][]</span><span class="sxs-lookup"><span data-stu-id="16180-122">[Get recent activities][]</span></span> | <span data-ttu-id="16180-123">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="16180-123">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="16180-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="16180-130">JSON representation</span></span>

<span data-ttu-id="16180-131">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16180-131">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="16180-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="16180-132">Properties</span></span>

<span data-ttu-id="16180-133">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="16180-133">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="16180-134">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="16180-134">Property name</span></span>    | <span data-ttu-id="16180-135">Тип</span><span class="sxs-lookup"><span data-stu-id="16180-135">Type</span></span>                             | <span data-ttu-id="16180-136">Описание</span><span class="sxs-lookup"><span data-stu-id="16180-136">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="16180-137">**columns**</span><span class="sxs-lookup"><span data-stu-id="16180-137">**columns**</span></span>      | <span data-ttu-id="16180-138">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="16180-138">Collection([columnDefinition][])</span></span> | <span data-ttu-id="16180-139">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="16180-139">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="16180-140">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="16180-140">**contentTypes**</span></span> | <span data-ttu-id="16180-141">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="16180-141">Collection([contentType][])</span></span>      | <span data-ttu-id="16180-142">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="16180-142">The collection of content types present in this list.</span></span>
| <span data-ttu-id="16180-143">**displayName**</span><span class="sxs-lookup"><span data-stu-id="16180-143">**displayName**</span></span>  | <span data-ttu-id="16180-144">строка</span><span class="sxs-lookup"><span data-stu-id="16180-144">string</span></span>                           | <span data-ttu-id="16180-145">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="16180-145">The displayable title of the list.</span></span>
| <span data-ttu-id="16180-146">**list**</span><span class="sxs-lookup"><span data-stu-id="16180-146">**list**</span></span>         | <span data-ttu-id="16180-147">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="16180-147">[listInfo][]</span></span>                     | <span data-ttu-id="16180-148">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="16180-148">Provides additional details about the list.</span></span>
| <span data-ttu-id="16180-149">**system**</span><span class="sxs-lookup"><span data-stu-id="16180-149">**system**</span></span>       | <span data-ttu-id="16180-150">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="16180-150">[systemFacet][]</span></span>                  | <span data-ttu-id="16180-151">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="16180-151">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="16180-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16180-152">Read-only.</span></span>

<span data-ttu-id="16180-153">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="16180-153">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="16180-154">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="16180-154">Property name</span></span>            | <span data-ttu-id="16180-155">Тип</span><span class="sxs-lookup"><span data-stu-id="16180-155">Type</span></span>             | <span data-ttu-id="16180-156">Описание</span><span class="sxs-lookup"><span data-stu-id="16180-156">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="16180-157">**id**</span><span class="sxs-lookup"><span data-stu-id="16180-157">**id**</span></span>                   | <span data-ttu-id="16180-158">string</span><span class="sxs-lookup"><span data-stu-id="16180-158">string</span></span>           | <span data-ttu-id="16180-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16180-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="16180-161">**name**</span><span class="sxs-lookup"><span data-stu-id="16180-161">**name**</span></span>                 | <span data-ttu-id="16180-162">string</span><span class="sxs-lookup"><span data-stu-id="16180-162">string</span></span>           | <span data-ttu-id="16180-163">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="16180-163">The name of the item.</span></span>
| <span data-ttu-id="16180-164">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="16180-164">**createdBy**</span></span>            | <span data-ttu-id="16180-165">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="16180-165">[identitySet][]</span></span>  | <span data-ttu-id="16180-166">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="16180-166">Identity of the creator of this item.</span></span> <span data-ttu-id="16180-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16180-167">Read-only.</span></span>
| <span data-ttu-id="16180-168">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="16180-168">**createdDateTime**</span></span>      | <span data-ttu-id="16180-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16180-169">DateTimeOffset</span></span>   | <span data-ttu-id="16180-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16180-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="16180-172">**description**</span><span class="sxs-lookup"><span data-stu-id="16180-172">**description**</span></span>          | <span data-ttu-id="16180-173">строка</span><span class="sxs-lookup"><span data-stu-id="16180-173">string</span></span>           | <span data-ttu-id="16180-174">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="16180-174">The descriptive text for the item.</span></span>
| <span data-ttu-id="16180-175">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="16180-175">**lastModifiedBy**</span></span>       | <span data-ttu-id="16180-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="16180-176">[identitySet][]</span></span>  | <span data-ttu-id="16180-177">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="16180-177">Identity of the last modifier of this item.</span></span> <span data-ttu-id="16180-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16180-178">Read-only.</span></span>
| <span data-ttu-id="16180-179">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="16180-179">**lastModifiedDateTime**</span></span> | <span data-ttu-id="16180-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16180-180">DateTimeOffset</span></span>   | <span data-ttu-id="16180-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16180-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="16180-183">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="16180-183">**webUrl**</span></span>               | <span data-ttu-id="16180-184">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="16180-184">string (url)</span></span>     | <span data-ttu-id="16180-p109">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16180-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="16180-187">Связи</span><span class="sxs-lookup"><span data-stu-id="16180-187">Relationships</span></span>

<span data-ttu-id="16180-188">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="16180-188">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="16180-189">Имя связи</span><span class="sxs-lookup"><span data-stu-id="16180-189">Relationship name</span></span> | <span data-ttu-id="16180-190">Тип</span><span class="sxs-lookup"><span data-stu-id="16180-190">Type</span></span>                        | <span data-ttu-id="16180-191">Описание</span><span class="sxs-lookup"><span data-stu-id="16180-191">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="16180-192">**activities**</span><span class="sxs-lookup"><span data-stu-id="16180-192">**activities**</span></span>    | <span data-ttu-id="16180-193">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="16180-193">[itemActivity][] collection</span></span> | <span data-ttu-id="16180-194">Последние действия, выполненные в списке.</span><span class="sxs-lookup"><span data-stu-id="16180-194">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="16180-195">**drive**</span><span class="sxs-lookup"><span data-stu-id="16180-195">**drive**</span></span>         | <span data-ttu-id="16180-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="16180-196">[drive][]</span></span>                   | <span data-ttu-id="16180-197">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="16180-197">Only present on document libraries.</span></span> <span data-ttu-id="16180-198">Разрешает доступ к списку как к ресурсу [drive][] с ресурсами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="16180-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="16180-199">**items**</span><span class="sxs-lookup"><span data-stu-id="16180-199">**items**</span></span>         | <span data-ttu-id="16180-200">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="16180-200">Collection([listItem][])</span></span>    | <span data-ttu-id="16180-201">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="16180-201">All items contained in the list.</span></span>

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
