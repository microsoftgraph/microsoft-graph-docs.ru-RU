---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: List
ms.openlocfilehash: b1538fd3eadd3cd00193519a32effdd7c3b61247
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076563"
---
# <a name="list-resource"></a><span data-ttu-id="fe036-102">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="fe036-102">List resource</span></span>

> <span data-ttu-id="fe036-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe036-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe036-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe036-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe036-105">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="fe036-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="fe036-106">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="fe036-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="fe036-107">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="fe036-107">Tasks on a list</span></span>

<span data-ttu-id="fe036-108">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="fe036-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="fe036-109">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="fe036-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="fe036-110">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="fe036-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="fe036-111">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="fe036-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="fe036-112">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="fe036-112">Common task</span></span>               | <span data-ttu-id="fe036-113">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="fe036-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="fe036-114">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="fe036-114">[Get list][]</span></span>              | <span data-ttu-id="fe036-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="fe036-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="fe036-116">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="fe036-116">[Enumerate list items][]</span></span>  | <span data-ttu-id="fe036-117">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="fe036-117">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="fe036-118">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="fe036-118">[Update list item][]</span></span>      | <span data-ttu-id="fe036-119">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="fe036-119">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="fe036-120">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="fe036-120">[Delete list item][]</span></span>      | <span data-ttu-id="fe036-121">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="fe036-121">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="fe036-122">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="fe036-122">[Create list item][]</span></span>      | <span data-ttu-id="fe036-123">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="fe036-123">POST /lists/{list-id}</span></span>
| <span data-ttu-id="fe036-124">[Получение последних действий][]</span><span class="sxs-lookup"><span data-stu-id="fe036-124">[Get recent activities][]</span></span> | <span data-ttu-id="fe036-125">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="fe036-125">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="fe036-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fe036-132">JSON representation</span></span>

<span data-ttu-id="fe036-133">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe036-133">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fe036-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe036-134">Properties</span></span>

<span data-ttu-id="fe036-135">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="fe036-135">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="fe036-136">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="fe036-136">Property name</span></span>    | <span data-ttu-id="fe036-137">Тип</span><span class="sxs-lookup"><span data-stu-id="fe036-137">Type</span></span>                             | <span data-ttu-id="fe036-138">Описание</span><span class="sxs-lookup"><span data-stu-id="fe036-138">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="fe036-139">**columns**</span><span class="sxs-lookup"><span data-stu-id="fe036-139">**columns**</span></span>      | <span data-ttu-id="fe036-140">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="fe036-140">Collection([columnDefinition][])</span></span> | <span data-ttu-id="fe036-141">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="fe036-141">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="fe036-142">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="fe036-142">**contentTypes**</span></span> | <span data-ttu-id="fe036-143">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="fe036-143">Collection([contentType][])</span></span>      | <span data-ttu-id="fe036-144">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="fe036-144">The collection of content types present in this list.</span></span>
| <span data-ttu-id="fe036-145">**displayName**</span><span class="sxs-lookup"><span data-stu-id="fe036-145">**displayName**</span></span>  | <span data-ttu-id="fe036-146">строка</span><span class="sxs-lookup"><span data-stu-id="fe036-146">string</span></span>                           | <span data-ttu-id="fe036-147">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="fe036-147">The displayable title of the list.</span></span>
| <span data-ttu-id="fe036-148">**list**</span><span class="sxs-lookup"><span data-stu-id="fe036-148">**list**</span></span>         | <span data-ttu-id="fe036-149">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="fe036-149">[listInfo][]</span></span>                     | <span data-ttu-id="fe036-150">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="fe036-150">Provides additional details about the list.</span></span>
| <span data-ttu-id="fe036-151">**system**</span><span class="sxs-lookup"><span data-stu-id="fe036-151">**system**</span></span>       | <span data-ttu-id="fe036-152">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="fe036-152">[systemFacet][]</span></span>                  | <span data-ttu-id="fe036-153">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="fe036-153">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="fe036-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe036-154">Read-only.</span></span>

<span data-ttu-id="fe036-155">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="fe036-155">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="fe036-156">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="fe036-156">Property name</span></span>            | <span data-ttu-id="fe036-157">Тип</span><span class="sxs-lookup"><span data-stu-id="fe036-157">Type</span></span>             | <span data-ttu-id="fe036-158">Описание</span><span class="sxs-lookup"><span data-stu-id="fe036-158">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="fe036-159">**id**</span><span class="sxs-lookup"><span data-stu-id="fe036-159">**id**</span></span>                   | <span data-ttu-id="fe036-160">строка</span><span class="sxs-lookup"><span data-stu-id="fe036-160">string</span></span>           | <span data-ttu-id="fe036-p105">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe036-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="fe036-163">**name**</span><span class="sxs-lookup"><span data-stu-id="fe036-163">**name**</span></span>                 | <span data-ttu-id="fe036-164">строка</span><span class="sxs-lookup"><span data-stu-id="fe036-164">string</span></span>           | <span data-ttu-id="fe036-165">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="fe036-165">The name of the item.</span></span>
| <span data-ttu-id="fe036-166">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="fe036-166">**createdBy**</span></span>            | <span data-ttu-id="fe036-167">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="fe036-167">[identitySet][]</span></span>  | <span data-ttu-id="fe036-168">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="fe036-168">Identity of the creator of this item.</span></span> <span data-ttu-id="fe036-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe036-169">Read-only.</span></span>
| <span data-ttu-id="fe036-170">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="fe036-170">**createdDateTime**</span></span>      | <span data-ttu-id="fe036-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe036-171">DateTimeOffset</span></span>   | <span data-ttu-id="fe036-p107">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe036-p107">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="fe036-174">**description**</span><span class="sxs-lookup"><span data-stu-id="fe036-174">**description**</span></span>          | <span data-ttu-id="fe036-175">строка</span><span class="sxs-lookup"><span data-stu-id="fe036-175">string</span></span>           | <span data-ttu-id="fe036-176">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="fe036-176">The descriptive text for the item.</span></span>
| <span data-ttu-id="fe036-177">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="fe036-177">**lastModifiedBy**</span></span>       | <span data-ttu-id="fe036-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="fe036-178">[identitySet][]</span></span>  | <span data-ttu-id="fe036-179">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="fe036-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="fe036-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe036-180">Read-only.</span></span>
| <span data-ttu-id="fe036-181">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="fe036-181">**lastModifiedDateTime**</span></span> | <span data-ttu-id="fe036-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe036-182">DateTimeOffset</span></span>   | <span data-ttu-id="fe036-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe036-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="fe036-185">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="fe036-185">**webUrl**</span></span>               | <span data-ttu-id="fe036-186">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="fe036-186">string (url)</span></span>     | <span data-ttu-id="fe036-p110">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe036-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="fe036-189">Связи</span><span class="sxs-lookup"><span data-stu-id="fe036-189">Relationships</span></span>

<span data-ttu-id="fe036-190">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="fe036-190">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="fe036-191">Имя связи</span><span class="sxs-lookup"><span data-stu-id="fe036-191">Relationship name</span></span> | <span data-ttu-id="fe036-192">Тип</span><span class="sxs-lookup"><span data-stu-id="fe036-192">Type</span></span>                        | <span data-ttu-id="fe036-193">Описание</span><span class="sxs-lookup"><span data-stu-id="fe036-193">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="fe036-194">**activities**</span><span class="sxs-lookup"><span data-stu-id="fe036-194">**activities**</span></span>    | <span data-ttu-id="fe036-195">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="fe036-195">[itemActivity][] collection</span></span> | <span data-ttu-id="fe036-196">Последние действия, выполненные в списке.</span><span class="sxs-lookup"><span data-stu-id="fe036-196">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="fe036-197">**drive**</span><span class="sxs-lookup"><span data-stu-id="fe036-197">**drive**</span></span>         | <span data-ttu-id="fe036-198">[drive][]</span><span class="sxs-lookup"><span data-stu-id="fe036-198">[drive][]</span></span>                   | <span data-ttu-id="fe036-199">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="fe036-199">Only present on document libraries.</span></span> <span data-ttu-id="fe036-200">Разрешает доступ к списку как к ресурсу [drive][] с ресурсами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="fe036-200">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="fe036-201">**items**</span><span class="sxs-lookup"><span data-stu-id="fe036-201">**items**</span></span>         | <span data-ttu-id="fe036-202">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="fe036-202">Collection([listItem][])</span></span>    | <span data-ttu-id="fe036-203">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="fe036-203">All items contained in the list.</span></span>

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
