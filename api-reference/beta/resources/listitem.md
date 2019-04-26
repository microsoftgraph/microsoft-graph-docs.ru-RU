---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9f813511ffa8a033d2ee85f8c7e5d2d5a271dd1e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345248"
---
# <a name="listitem-resource"></a><span data-ttu-id="e761b-102">Ресурс ListItem</span><span class="sxs-lookup"><span data-stu-id="e761b-102">ListItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e761b-103">Этот ресурс представляет элемент объекта **[list][]** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e761b-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="e761b-104">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="e761b-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="e761b-105">Задачи для ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="e761b-105">Tasks on a listItem</span></span>

<span data-ttu-id="e761b-106">Ниже перечислены задачи, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="e761b-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="e761b-107">Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="e761b-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="e761b-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="e761b-108">Common task</span></span>                    | <span data-ttu-id="e761b-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="e761b-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="e761b-110">[Получение][]</span><span class="sxs-lookup"><span data-stu-id="e761b-110">[Get][]</span></span>                        | <span data-ttu-id="e761b-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="e761b-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="e761b-112">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="e761b-112">[Get column values][Get]</span></span>       | <span data-ttu-id="e761b-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="e761b-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="e761b-114">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="e761b-114">[Get analytics][]</span></span>              | <span data-ttu-id="e761b-115">ПОЛУЧЕНИЕ/итемс/{итем-ИД}/Аналитикс</span><span class="sxs-lookup"><span data-stu-id="e761b-115">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="e761b-116">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="e761b-116">[Get activities by interval][]</span></span> | <span data-ttu-id="e761b-117">ПОЛУЧЕНИЕ/Итемс/{итем-ИД}/жетактивитиесбинтервал</span><span class="sxs-lookup"><span data-stu-id="e761b-117">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="e761b-118">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="e761b-118">[Create][]</span></span>                     | <span data-ttu-id="e761b-119">POST /items</span><span class="sxs-lookup"><span data-stu-id="e761b-119">POST /items</span></span>
| <span data-ttu-id="e761b-120">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="e761b-120">[Delete][]</span></span>                     | <span data-ttu-id="e761b-121">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="e761b-121">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="e761b-122">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="e761b-122">[Update][]</span></span>                     | <span data-ttu-id="e761b-123">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="e761b-123">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="e761b-124">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="e761b-124">[Update column values][Update]</span></span> | <span data-ttu-id="e761b-125">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="e761b-125">PATCH /items/{item-id}/fields</span></span>

[Получение]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Создание]: ../api/listitem-create.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Обновление]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="e761b-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e761b-132">JSON representation</span></span>

<span data-ttu-id="e761b-133">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e761b-133">Here is a JSON representation of a **listItem** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="e761b-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="e761b-134">Properties</span></span>

<span data-ttu-id="e761b-135">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="e761b-135">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="e761b-136">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e761b-136">Property name</span></span> | <span data-ttu-id="e761b-137">Тип</span><span class="sxs-lookup"><span data-stu-id="e761b-137">Type</span></span>                | <span data-ttu-id="e761b-138">Описание</span><span class="sxs-lookup"><span data-stu-id="e761b-138">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="e761b-139">contentType</span><span class="sxs-lookup"><span data-stu-id="e761b-139">contentType</span></span>   | <span data-ttu-id="e761b-140">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="e761b-140">[contentTypeInfo][]</span></span> | <span data-ttu-id="e761b-141">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="e761b-141">The content type of this list item</span></span>

<span data-ttu-id="e761b-142">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="e761b-142">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="e761b-143">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e761b-143">Property name</span></span>        | <span data-ttu-id="e761b-144">Тип</span><span class="sxs-lookup"><span data-stu-id="e761b-144">Type</span></span>              | <span data-ttu-id="e761b-145">Описание</span><span class="sxs-lookup"><span data-stu-id="e761b-145">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="e761b-146">id</span><span class="sxs-lookup"><span data-stu-id="e761b-146">id</span></span>                   | <span data-ttu-id="e761b-147">строка</span><span class="sxs-lookup"><span data-stu-id="e761b-147">string</span></span>            | <span data-ttu-id="e761b-p103">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e761b-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="e761b-150">name</span><span class="sxs-lookup"><span data-stu-id="e761b-150">name</span></span>                 | <span data-ttu-id="e761b-151">string</span><span class="sxs-lookup"><span data-stu-id="e761b-151">string</span></span>            | <span data-ttu-id="e761b-152">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="e761b-152">The name / title of the item.</span></span>
| <span data-ttu-id="e761b-153">createdBy</span><span class="sxs-lookup"><span data-stu-id="e761b-153">createdBy</span></span>            | <span data-ttu-id="e761b-154">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e761b-154">[identitySet][]</span></span>   | <span data-ttu-id="e761b-155">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="e761b-155">Identity of the creator of this item.</span></span> <span data-ttu-id="e761b-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e761b-156">Read-only.</span></span>
| <span data-ttu-id="e761b-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e761b-157">createdDateTime</span></span>      | <span data-ttu-id="e761b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e761b-158">DateTimeOffset</span></span>    | <span data-ttu-id="e761b-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e761b-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="e761b-161">description</span><span class="sxs-lookup"><span data-stu-id="e761b-161">description</span></span>          | <span data-ttu-id="e761b-162">строка</span><span class="sxs-lookup"><span data-stu-id="e761b-162">string</span></span>            | <span data-ttu-id="e761b-163">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="e761b-163">The descriptive text for the item.</span></span>
| <span data-ttu-id="e761b-164">eTag</span><span class="sxs-lookup"><span data-stu-id="e761b-164">eTag</span></span>                 | <span data-ttu-id="e761b-165">string</span><span class="sxs-lookup"><span data-stu-id="e761b-165">string</span></span>            | <span data-ttu-id="e761b-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e761b-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="e761b-168">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e761b-168">lastModifiedBy</span></span>       | <span data-ttu-id="e761b-169">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e761b-169">[identitySet][]</span></span>   | <span data-ttu-id="e761b-170">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="e761b-170">Identity of the last modifier of this item.</span></span> <span data-ttu-id="e761b-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e761b-171">Read-only.</span></span>
| <span data-ttu-id="e761b-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e761b-172">lastModifiedDateTime</span></span> | <span data-ttu-id="e761b-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e761b-173">DateTimeOffset</span></span>    | <span data-ttu-id="e761b-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e761b-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="e761b-176">parentReference</span><span class="sxs-lookup"><span data-stu-id="e761b-176">parentReference</span></span>      | <span data-ttu-id="e761b-177">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="e761b-177">[itemReference][]</span></span> | <span data-ttu-id="e761b-p109">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="e761b-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="e761b-180">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="e761b-180">sharepointIds</span></span>        | <span data-ttu-id="e761b-181">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="e761b-181">[sharepointIds][]</span></span> | <span data-ttu-id="e761b-p110">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e761b-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="e761b-184">webUrl</span><span class="sxs-lookup"><span data-stu-id="e761b-184">webUrl</span></span>               | <span data-ttu-id="e761b-185">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="e761b-185">string (url)</span></span>      | <span data-ttu-id="e761b-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e761b-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="e761b-188">Связи</span><span class="sxs-lookup"><span data-stu-id="e761b-188">Relationships</span></span>

 <span data-ttu-id="e761b-189">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="e761b-189">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="e761b-190">Имя связи</span><span class="sxs-lookup"><span data-stu-id="e761b-190">Relationship name</span></span> | <span data-ttu-id="e761b-191">Тип</span><span class="sxs-lookup"><span data-stu-id="e761b-191">Type</span></span>                           | <span data-ttu-id="e761b-192">Описание</span><span class="sxs-lookup"><span data-stu-id="e761b-192">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="e761b-193">activities</span><span class="sxs-lookup"><span data-stu-id="e761b-193">activities</span></span>        | <span data-ttu-id="e761b-194">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="e761b-194">[itemActivity][] collection</span></span>    | <span data-ttu-id="e761b-195">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="e761b-195">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="e761b-196">analytics</span><span class="sxs-lookup"><span data-stu-id="e761b-196">analytics</span></span>         | <span data-ttu-id="e761b-197">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="e761b-197">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="e761b-198">Аналитика сведений о действиях, которые были выполнены для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e761b-198">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="e761b-199">driveItem</span><span class="sxs-lookup"><span data-stu-id="e761b-199">driveItem</span></span>         | <span data-ttu-id="e761b-200">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="e761b-200">[driveItem][]</span></span>                  | <span data-ttu-id="e761b-201">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="e761b-201">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="e761b-202">fields</span><span class="sxs-lookup"><span data-stu-id="e761b-202">fields</span></span>            | <span data-ttu-id="e761b-203">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="e761b-203">[fieldValueSet][]</span></span>              | <span data-ttu-id="e761b-204">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="e761b-204">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="e761b-205">versions</span><span class="sxs-lookup"><span data-stu-id="e761b-205">versions</span></span>          | <span data-ttu-id="e761b-206">Коллекция [listItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="e761b-206">[listItemVersion][] collection</span></span> | <span data-ttu-id="e761b-207">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="e761b-207">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  },
  "suppressions": []
}
-->
