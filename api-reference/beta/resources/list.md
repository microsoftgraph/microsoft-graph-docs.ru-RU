---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.openlocfilehash: 03121447e0b9d7d091005283ed12ef7d93e68108
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870464"
---
# <a name="list-resource"></a><span data-ttu-id="13acd-102">Ресурс List</span><span class="sxs-lookup"><span data-stu-id="13acd-102">List resource</span></span>

> <span data-ttu-id="13acd-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="13acd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13acd-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13acd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13acd-105">Ресурс **list** представляет список в ресурсе [site][].</span><span class="sxs-lookup"><span data-stu-id="13acd-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="13acd-106">Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.</span><span class="sxs-lookup"><span data-stu-id="13acd-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="13acd-107">Задачи для ресурса list</span><span class="sxs-lookup"><span data-stu-id="13acd-107">Tasks on a list</span></span>

<span data-ttu-id="13acd-108">Ниже перечислены задачи, доступные для ресурсов list.</span><span class="sxs-lookup"><span data-stu-id="13acd-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="13acd-109">**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="13acd-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="13acd-110">Однако вы можете создавать и менять [элементы списков][listItem].</span><span class="sxs-lookup"><span data-stu-id="13acd-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="13acd-111">Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="13acd-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="13acd-112">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="13acd-112">Common task</span></span>               | <span data-ttu-id="13acd-113">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="13acd-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="13acd-114">[Получение списка][]</span><span class="sxs-lookup"><span data-stu-id="13acd-114">[Get list][]</span></span>              | <span data-ttu-id="13acd-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="13acd-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="13acd-116">[Перечисление элементов списка][]</span><span class="sxs-lookup"><span data-stu-id="13acd-116">[Enumerate list items][]</span></span>  | <span data-ttu-id="13acd-117">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="13acd-117">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="13acd-118">[Обновление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="13acd-118">[Update list item][]</span></span>      | <span data-ttu-id="13acd-119">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="13acd-119">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="13acd-120">[Удаление элемента списка][]</span><span class="sxs-lookup"><span data-stu-id="13acd-120">[Delete list item][]</span></span>      | <span data-ttu-id="13acd-121">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="13acd-121">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="13acd-122">[Создание элемента в списке][]</span><span class="sxs-lookup"><span data-stu-id="13acd-122">[Create list item][]</span></span>      | <span data-ttu-id="13acd-123">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="13acd-123">POST /lists/{list-id}</span></span>
| <span data-ttu-id="13acd-124">[Получение последних действий][]</span><span class="sxs-lookup"><span data-stu-id="13acd-124">[Get recent activities][]</span></span> | <span data-ttu-id="13acd-125">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="13acd-125">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="13acd-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="13acd-132">JSON representation</span></span>

<span data-ttu-id="13acd-133">Ниже показано представление ресурса **list** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13acd-133">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="13acd-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="13acd-134">Properties</span></span>

<span data-ttu-id="13acd-135">Ниже перечислены свойства ресурса **list**.</span><span class="sxs-lookup"><span data-stu-id="13acd-135">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="13acd-136">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="13acd-136">Property name</span></span>    | <span data-ttu-id="13acd-137">Тип</span><span class="sxs-lookup"><span data-stu-id="13acd-137">Type</span></span>                             | <span data-ttu-id="13acd-138">Описание</span><span class="sxs-lookup"><span data-stu-id="13acd-138">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="13acd-139">**columns**</span><span class="sxs-lookup"><span data-stu-id="13acd-139">**columns**</span></span>      | <span data-ttu-id="13acd-140">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="13acd-140">Collection([columnDefinition][])</span></span> | <span data-ttu-id="13acd-141">Коллекция определений полей для данного списка.</span><span class="sxs-lookup"><span data-stu-id="13acd-141">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="13acd-142">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="13acd-142">**contentTypes**</span></span> | <span data-ttu-id="13acd-143">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="13acd-143">Collection([contentType][])</span></span>      | <span data-ttu-id="13acd-144">Коллекция типов контента в данном списке.</span><span class="sxs-lookup"><span data-stu-id="13acd-144">The collection of content types present in this list.</span></span>
| <span data-ttu-id="13acd-145">**displayName**</span><span class="sxs-lookup"><span data-stu-id="13acd-145">**displayName**</span></span>  | <span data-ttu-id="13acd-146">строка</span><span class="sxs-lookup"><span data-stu-id="13acd-146">string</span></span>                           | <span data-ttu-id="13acd-147">Отображаемый заголовок списка.</span><span class="sxs-lookup"><span data-stu-id="13acd-147">The displayable title of the list.</span></span>
| <span data-ttu-id="13acd-148">**list**</span><span class="sxs-lookup"><span data-stu-id="13acd-148">**list**</span></span>         | <span data-ttu-id="13acd-149">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="13acd-149">[listInfo][]</span></span>                     | <span data-ttu-id="13acd-150">Предоставляет дополнительные сведения о списке.</span><span class="sxs-lookup"><span data-stu-id="13acd-150">Provides additional details about the list.</span></span>
| <span data-ttu-id="13acd-151">**system**</span><span class="sxs-lookup"><span data-stu-id="13acd-151">**system**</span></span>       | <span data-ttu-id="13acd-152">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="13acd-152">[systemFacet][]</span></span>                  | <span data-ttu-id="13acd-153">Если это свойство задано, оно указывает, что данным списком управляет система.</span><span class="sxs-lookup"><span data-stu-id="13acd-153">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="13acd-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13acd-154">Read-only.</span></span>

<span data-ttu-id="13acd-155">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="13acd-155">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="13acd-156">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="13acd-156">Property name</span></span>            | <span data-ttu-id="13acd-157">Тип</span><span class="sxs-lookup"><span data-stu-id="13acd-157">Type</span></span>             | <span data-ttu-id="13acd-158">Описание</span><span class="sxs-lookup"><span data-stu-id="13acd-158">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="13acd-159">**id**</span><span class="sxs-lookup"><span data-stu-id="13acd-159">**id**</span></span>                   | <span data-ttu-id="13acd-160">строка</span><span class="sxs-lookup"><span data-stu-id="13acd-160">string</span></span>           | <span data-ttu-id="13acd-p105">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13acd-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="13acd-163">**name**</span><span class="sxs-lookup"><span data-stu-id="13acd-163">**name**</span></span>                 | <span data-ttu-id="13acd-164">строка</span><span class="sxs-lookup"><span data-stu-id="13acd-164">string</span></span>           | <span data-ttu-id="13acd-165">Имя элемента.</span><span class="sxs-lookup"><span data-stu-id="13acd-165">The name of the item.</span></span>
| <span data-ttu-id="13acd-166">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="13acd-166">**createdBy**</span></span>            | <span data-ttu-id="13acd-167">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="13acd-167">[identitySet][]</span></span>  | <span data-ttu-id="13acd-168">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="13acd-168">Identity of the creator of this item.</span></span> <span data-ttu-id="13acd-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13acd-169">Read-only.</span></span>
| <span data-ttu-id="13acd-170">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="13acd-170">**createdDateTime**</span></span>      | <span data-ttu-id="13acd-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13acd-171">DateTimeOffset</span></span>   | <span data-ttu-id="13acd-p107">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13acd-p107">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="13acd-174">**description**</span><span class="sxs-lookup"><span data-stu-id="13acd-174">**description**</span></span>          | <span data-ttu-id="13acd-175">строка</span><span class="sxs-lookup"><span data-stu-id="13acd-175">string</span></span>           | <span data-ttu-id="13acd-176">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="13acd-176">The descriptive text for the item.</span></span>
| <span data-ttu-id="13acd-177">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="13acd-177">**lastModifiedBy**</span></span>       | <span data-ttu-id="13acd-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="13acd-178">[identitySet][]</span></span>  | <span data-ttu-id="13acd-179">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="13acd-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="13acd-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13acd-180">Read-only.</span></span>
| <span data-ttu-id="13acd-181">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="13acd-181">**lastModifiedDateTime**</span></span> | <span data-ttu-id="13acd-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13acd-182">DateTimeOffset</span></span>   | <span data-ttu-id="13acd-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13acd-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="13acd-185">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="13acd-185">**webUrl**</span></span>               | <span data-ttu-id="13acd-186">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="13acd-186">string (url)</span></span>     | <span data-ttu-id="13acd-p110">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13acd-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="13acd-189">Связи</span><span class="sxs-lookup"><span data-stu-id="13acd-189">Relationships</span></span>

<span data-ttu-id="13acd-190">Ниже перечислены связи ресурса **list** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="13acd-190">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="13acd-191">Имя связи</span><span class="sxs-lookup"><span data-stu-id="13acd-191">Relationship name</span></span> | <span data-ttu-id="13acd-192">Тип</span><span class="sxs-lookup"><span data-stu-id="13acd-192">Type</span></span>                        | <span data-ttu-id="13acd-193">Описание</span><span class="sxs-lookup"><span data-stu-id="13acd-193">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="13acd-194">**activities**</span><span class="sxs-lookup"><span data-stu-id="13acd-194">**activities**</span></span>    | <span data-ttu-id="13acd-195">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="13acd-195">[itemActivity][] collection</span></span> | <span data-ttu-id="13acd-196">Последние действия, выполненные в списке.</span><span class="sxs-lookup"><span data-stu-id="13acd-196">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="13acd-197">**drive**</span><span class="sxs-lookup"><span data-stu-id="13acd-197">**drive**</span></span>         | <span data-ttu-id="13acd-198">[drive][]</span><span class="sxs-lookup"><span data-stu-id="13acd-198">[drive][]</span></span>                   | <span data-ttu-id="13acd-199">Доступна только для библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="13acd-199">Only present on document libraries.</span></span> <span data-ttu-id="13acd-200">Разрешает доступ к списку как к ресурсу [drive][] с ресурсами [driveItem][driveItem].</span><span class="sxs-lookup"><span data-stu-id="13acd-200">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="13acd-201">**items**</span><span class="sxs-lookup"><span data-stu-id="13acd-201">**items**</span></span>         | <span data-ttu-id="13acd-202">Коллекция ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="13acd-202">Collection([listItem][])</span></span>    | <span data-ttu-id="13acd-203">Все элементы, содержащиеся в списке.</span><span class="sxs-lookup"><span data-stu-id="13acd-203">All items contained in the list.</span></span>

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
