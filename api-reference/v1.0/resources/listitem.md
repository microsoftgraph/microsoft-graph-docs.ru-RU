---
author: JeremyKelley
ms.author: JeremyKelley
title: Ресурс listItem
description: Этот ресурс представляет элемент объекта list в SharePoint.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 873ad5961c9cadb444c6fe9f2afec69853cc5d85
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968802"
---
# <a name="listitem-resource"></a><span data-ttu-id="6f705-103">Ресурс listItem</span><span class="sxs-lookup"><span data-stu-id="6f705-103">ListItem resource</span></span>

<span data-ttu-id="6f705-104">Этот ресурс представляет элемент объекта **[list][]** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6f705-104">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="6f705-105">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="6f705-105">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="6f705-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6f705-106">Methods</span></span>

<span data-ttu-id="6f705-107">Ниже перечислены методы, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="6f705-107">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="6f705-108">Все примеры относятся к объекту **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="6f705-108">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="6f705-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6f705-109">Method</span></span>                    | <span data-ttu-id="6f705-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6f705-110">Return Type</span></span> | <span data-ttu-id="6f705-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6f705-111">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="6f705-112">[Получение][]</span><span class="sxs-lookup"><span data-stu-id="6f705-112">[Get][]</span></span>                   | <span data-ttu-id="6f705-113">lisItem</span><span class="sxs-lookup"><span data-stu-id="6f705-113">lisItem</span></span>| <span data-ttu-id="6f705-114">Получение элемента списка.</span><span class="sxs-lookup"><span data-stu-id="6f705-114">Get an item in a list</span></span>
| <span data-ttu-id="6f705-115">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="6f705-115">[Get column values][Get]</span></span>       | <span data-ttu-id="6f705-116">listItem</span><span class="sxs-lookup"><span data-stu-id="6f705-116">listItem</span></span> | <span data-ttu-id="6f705-117">Получение значений столбцов из ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="6f705-117">Get column values from listItem.</span></span>
| <span data-ttu-id="6f705-118">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="6f705-118">[Get analytics][]</span></span>              | <span data-ttu-id="6f705-119">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="6f705-119">[itemAnalytics][]</span></span>| <span data-ttu-id="6f705-120">Получение аналитических данных для ресурса.</span><span class="sxs-lookup"><span data-stu-id="6f705-120">Get analytics for this resource.</span></span> 
| <span data-ttu-id="6f705-121">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="6f705-121">[Get activities by interval][]</span></span> | <span data-ttu-id="6f705-122">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="6f705-122">[itemActivityStat][]</span></span>| <span data-ttu-id="6f705-123">Получение коллекции объектов itemActivityStat в пределах указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="6f705-123">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="6f705-124">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="6f705-124">[Create][]</span></span>                     | <span data-ttu-id="6f705-125">listItem</span><span class="sxs-lookup"><span data-stu-id="6f705-125">listItem</span></span> | <span data-ttu-id="6f705-126">Создание ресурса listItem в списке.</span><span class="sxs-lookup"><span data-stu-id="6f705-126">Create a new listItem in a list.</span></span>
| <span data-ttu-id="6f705-127">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="6f705-127">[Delete][]</span></span>                     | <span data-ttu-id="6f705-128">Содержимое отсутствует</span><span class="sxs-lookup"><span data-stu-id="6f705-128">204 No Content</span></span> | <span data-ttu-id="6f705-129">Удаление элемента из списка.</span><span class="sxs-lookup"><span data-stu-id="6f705-129">Removes an item from a list.</span></span>
| <span data-ttu-id="6f705-130">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="6f705-130">[Update][]</span></span>                     | <span data-ttu-id="6f705-131">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="6f705-131">[fieldValueSet][]</span></span>| <span data-ttu-id="6f705-132">Изменение свойств ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="6f705-132">Update the properties on a listItem.</span></span>
| <span data-ttu-id="6f705-133">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="6f705-133">[Update column values][Update]</span></span> | <span data-ttu-id="6f705-134">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="6f705-134">[fieldValueSet][]</span></span>| <span data-ttu-id="6f705-135">Изменение значений столбцов ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="6f705-135">Update column values on a listItem.</span></span>

[Получение]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md
[Создание]: ../api/listitem-create.md
[Create]: ../api/listitem-create.md
[Удаление]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[Обновление]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

[itemActivityStat]: itemactivitystat.md
[fieldValueSet]: fieldvalueset.md

## <a name="properties"></a><span data-ttu-id="6f705-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f705-144">Properties</span></span>

<span data-ttu-id="6f705-145">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="6f705-145">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="6f705-146">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6f705-146">Property name</span></span> | <span data-ttu-id="6f705-147">Тип</span><span class="sxs-lookup"><span data-stu-id="6f705-147">Type</span></span>                | <span data-ttu-id="6f705-148">Описание</span><span class="sxs-lookup"><span data-stu-id="6f705-148">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="6f705-149">contentType</span><span class="sxs-lookup"><span data-stu-id="6f705-149">contentType</span></span>   | <span data-ttu-id="6f705-150">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="6f705-150">[contentTypeInfo][]</span></span> | <span data-ttu-id="6f705-151">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="6f705-151">The content type of this list item</span></span>

<span data-ttu-id="6f705-152">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="6f705-152">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="6f705-153">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6f705-153">Property name</span></span>        | <span data-ttu-id="6f705-154">Тип</span><span class="sxs-lookup"><span data-stu-id="6f705-154">Type</span></span>              | <span data-ttu-id="6f705-155">Описание</span><span class="sxs-lookup"><span data-stu-id="6f705-155">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="6f705-156">id</span><span class="sxs-lookup"><span data-stu-id="6f705-156">id</span></span>                   | <span data-ttu-id="6f705-157">string</span><span class="sxs-lookup"><span data-stu-id="6f705-157">string</span></span>            | <span data-ttu-id="6f705-p103">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f705-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="6f705-160">name</span><span class="sxs-lookup"><span data-stu-id="6f705-160">name</span></span>                 | <span data-ttu-id="6f705-161">string</span><span class="sxs-lookup"><span data-stu-id="6f705-161">string</span></span>            | <span data-ttu-id="6f705-162">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="6f705-162">The name / title of the item.</span></span>
| <span data-ttu-id="6f705-163">createdBy</span><span class="sxs-lookup"><span data-stu-id="6f705-163">createdBy</span></span>            | <span data-ttu-id="6f705-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6f705-164">[identitySet][]</span></span>   | <span data-ttu-id="6f705-165">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="6f705-165">Identity of the creator of this item.</span></span> <span data-ttu-id="6f705-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f705-166">Read-only.</span></span>
| <span data-ttu-id="6f705-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f705-167">createdDateTime</span></span>      | <span data-ttu-id="6f705-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f705-168">DateTimeOffset</span></span>    | <span data-ttu-id="6f705-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f705-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="6f705-171">description</span><span class="sxs-lookup"><span data-stu-id="6f705-171">description</span></span>          | <span data-ttu-id="6f705-172">строка</span><span class="sxs-lookup"><span data-stu-id="6f705-172">string</span></span>            | <span data-ttu-id="6f705-173">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="6f705-173">The descriptive text for the item.</span></span>
| <span data-ttu-id="6f705-174">eTag</span><span class="sxs-lookup"><span data-stu-id="6f705-174">eTag</span></span>                 | <span data-ttu-id="6f705-175">string</span><span class="sxs-lookup"><span data-stu-id="6f705-175">string</span></span>            | <span data-ttu-id="6f705-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f705-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="6f705-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6f705-178">lastModifiedBy</span></span>       | <span data-ttu-id="6f705-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6f705-179">[identitySet][]</span></span>   | <span data-ttu-id="6f705-180">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="6f705-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="6f705-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f705-181">Read-only.</span></span>
| <span data-ttu-id="6f705-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f705-182">lastModifiedDateTime</span></span> | <span data-ttu-id="6f705-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f705-183">DateTimeOffset</span></span>    | <span data-ttu-id="6f705-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f705-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="6f705-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="6f705-186">parentReference</span></span>      | <span data-ttu-id="6f705-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="6f705-187">[itemReference][]</span></span> | <span data-ttu-id="6f705-p109">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="6f705-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="6f705-190">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="6f705-190">sharepointIds</span></span>        | <span data-ttu-id="6f705-191">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="6f705-191">[sharepointIds][]</span></span> | <span data-ttu-id="6f705-p110">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f705-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="6f705-194">webUrl</span><span class="sxs-lookup"><span data-stu-id="6f705-194">webUrl</span></span>               | <span data-ttu-id="6f705-195">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="6f705-195">string (url)</span></span>      | <span data-ttu-id="6f705-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f705-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="6f705-198">Связи</span><span class="sxs-lookup"><span data-stu-id="6f705-198">Relationships</span></span>

 <span data-ttu-id="6f705-199">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="6f705-199">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="6f705-200">Имя связи</span><span class="sxs-lookup"><span data-stu-id="6f705-200">Relationship name</span></span> | <span data-ttu-id="6f705-201">Тип</span><span class="sxs-lookup"><span data-stu-id="6f705-201">Type</span></span>                           | <span data-ttu-id="6f705-202">Описание</span><span class="sxs-lookup"><span data-stu-id="6f705-202">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="6f705-203">activities</span><span class="sxs-lookup"><span data-stu-id="6f705-203">activities</span></span>        | <span data-ttu-id="6f705-204">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="6f705-204">[itemActivity][] collection</span></span>    | <span data-ttu-id="6f705-205">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="6f705-205">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="6f705-206">analytics</span><span class="sxs-lookup"><span data-stu-id="6f705-206">analytics</span></span>         | <span data-ttu-id="6f705-207">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="6f705-207">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="6f705-208">Аналитические данные о действиях просмотра, выполненных для элемента.</span><span class="sxs-lookup"><span data-stu-id="6f705-208">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="6f705-209">driveItem</span><span class="sxs-lookup"><span data-stu-id="6f705-209">driveItem</span></span>         | <span data-ttu-id="6f705-210">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6f705-210">[driveItem][]</span></span>                  | <span data-ttu-id="6f705-211">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="6f705-211">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="6f705-212">fields</span><span class="sxs-lookup"><span data-stu-id="6f705-212">fields</span></span>            | <span data-ttu-id="6f705-213">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="6f705-213">[fieldValueSet][]</span></span>              | <span data-ttu-id="6f705-214">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="6f705-214">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="6f705-215">versions</span><span class="sxs-lookup"><span data-stu-id="6f705-215">versions</span></span>          | <span data-ttu-id="6f705-216">Коллекция [listItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="6f705-216">[listItemVersion][] collection</span></span> | <span data-ttu-id="6f705-217">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="6f705-217">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="6f705-229">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f705-229">JSON representation</span></span>

<span data-ttu-id="6f705-230">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f705-230">Here is a JSON representation of a **listItem** resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/listItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
