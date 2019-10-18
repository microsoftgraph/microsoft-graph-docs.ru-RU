---
author: JeremyKelley
ms.author: JeremyKelley
title: Ресурс listItem
description: Этот ресурс представляет элемент объекта list в SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 883e7257b55826abf5cf60197c7854161f568fa5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036472"
---
# <a name="listitem-resource"></a><span data-ttu-id="8376c-103">Ресурс listItem</span><span class="sxs-lookup"><span data-stu-id="8376c-103">listItem resource</span></span>

<span data-ttu-id="8376c-104">Этот ресурс представляет элемент объекта **[list][]** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8376c-104">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="8376c-105">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="8376c-105">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="8376c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8376c-106">Methods</span></span>

<span data-ttu-id="8376c-107">Ниже перечислены методы, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="8376c-107">The following methods are available for **listItem** resources.</span></span>
<span data-ttu-id="8376c-108">Все примеры относятся к объекту **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="8376c-108">All examples are relative to a **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="8376c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8376c-109">Method</span></span>                    | <span data-ttu-id="8376c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8376c-110">Return Type</span></span> | <span data-ttu-id="8376c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8376c-111">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="8376c-112">[Получение][]</span><span class="sxs-lookup"><span data-stu-id="8376c-112">[Get][]</span></span>                   | <span data-ttu-id="8376c-113">lisItem</span><span class="sxs-lookup"><span data-stu-id="8376c-113">lisItem</span></span>| <span data-ttu-id="8376c-114">Получение элемента списка.</span><span class="sxs-lookup"><span data-stu-id="8376c-114">Get an item in a list.</span></span>
| <span data-ttu-id="8376c-115">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="8376c-115">[Get column values][Get]</span></span>       | <span data-ttu-id="8376c-116">listItem</span><span class="sxs-lookup"><span data-stu-id="8376c-116">listItem</span></span> | <span data-ttu-id="8376c-117">Получение значений столбцов из ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="8376c-117">Get column values from listItem.</span></span>
| <span data-ttu-id="8376c-118">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="8376c-118">[Get analytics][]</span></span>              | <span data-ttu-id="8376c-119">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="8376c-119">[itemAnalytics][]</span></span>| <span data-ttu-id="8376c-120">Получение аналитических данных для ресурса.</span><span class="sxs-lookup"><span data-stu-id="8376c-120">Get analytics for this resource.</span></span> 
| <span data-ttu-id="8376c-121">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="8376c-121">[Get activities by interval][]</span></span> | <span data-ttu-id="8376c-122">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="8376c-122">[itemActivityStat][]</span></span>| <span data-ttu-id="8376c-123">Получение коллекции объектов itemActivityStat в пределах указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="8376c-123">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="8376c-124">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="8376c-124">[Create][]</span></span>                     | <span data-ttu-id="8376c-125">listItem</span><span class="sxs-lookup"><span data-stu-id="8376c-125">listItem</span></span> | <span data-ttu-id="8376c-126">Создание ресурса listItem в списке.</span><span class="sxs-lookup"><span data-stu-id="8376c-126">Create a new listItem in a list.</span></span>
| <span data-ttu-id="8376c-127">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="8376c-127">[Delete][]</span></span>                     | <span data-ttu-id="8376c-128">Содержимое отсутствует</span><span class="sxs-lookup"><span data-stu-id="8376c-128">No Content</span></span> | <span data-ttu-id="8376c-129">Удаление элемента из списка.</span><span class="sxs-lookup"><span data-stu-id="8376c-129">Removes an item from a list.</span></span>
| <span data-ttu-id="8376c-130">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="8376c-130">[Update][]</span></span>                     | <span data-ttu-id="8376c-131">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="8376c-131">[fieldValueSet][]</span></span>| <span data-ttu-id="8376c-132">Изменение свойств ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="8376c-132">Update the properties on a listItem.</span></span>
| <span data-ttu-id="8376c-133">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="8376c-133">[Update column values][Update]</span></span> | <span data-ttu-id="8376c-134">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="8376c-134">[fieldValueSet][]</span></span>| <span data-ttu-id="8376c-135">Изменение значений столбцов ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="8376c-135">Update column values on a listItem.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8376c-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="8376c-144">Properties</span></span>

<span data-ttu-id="8376c-145">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="8376c-145">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="8376c-146">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8376c-146">Property name</span></span> | <span data-ttu-id="8376c-147">Тип</span><span class="sxs-lookup"><span data-stu-id="8376c-147">Type</span></span>                | <span data-ttu-id="8376c-148">Описание</span><span class="sxs-lookup"><span data-stu-id="8376c-148">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="8376c-149">contentType</span><span class="sxs-lookup"><span data-stu-id="8376c-149">contentType</span></span>   | <span data-ttu-id="8376c-150">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="8376c-150">[contentTypeInfo][]</span></span> | <span data-ttu-id="8376c-151">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="8376c-151">The content type of this list item</span></span>

<span data-ttu-id="8376c-152">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="8376c-152">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="8376c-153">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8376c-153">Property name</span></span>        | <span data-ttu-id="8376c-154">Тип</span><span class="sxs-lookup"><span data-stu-id="8376c-154">Type</span></span>              | <span data-ttu-id="8376c-155">Описание</span><span class="sxs-lookup"><span data-stu-id="8376c-155">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="8376c-156">id</span><span class="sxs-lookup"><span data-stu-id="8376c-156">id</span></span>                   | <span data-ttu-id="8376c-157">string</span><span class="sxs-lookup"><span data-stu-id="8376c-157">string</span></span>            | <span data-ttu-id="8376c-p103">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8376c-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="8376c-160">name</span><span class="sxs-lookup"><span data-stu-id="8376c-160">name</span></span>                 | <span data-ttu-id="8376c-161">string</span><span class="sxs-lookup"><span data-stu-id="8376c-161">string</span></span>            | <span data-ttu-id="8376c-162">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="8376c-162">The name / title of the item.</span></span>
| <span data-ttu-id="8376c-163">createdBy</span><span class="sxs-lookup"><span data-stu-id="8376c-163">createdBy</span></span>            | <span data-ttu-id="8376c-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8376c-164">[identitySet][]</span></span>   | <span data-ttu-id="8376c-165">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="8376c-165">Identity of the creator of this item.</span></span> <span data-ttu-id="8376c-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8376c-166">Read-only.</span></span>
| <span data-ttu-id="8376c-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8376c-167">createdDateTime</span></span>      | <span data-ttu-id="8376c-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8376c-168">DateTimeOffset</span></span>    | <span data-ttu-id="8376c-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8376c-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="8376c-171">description</span><span class="sxs-lookup"><span data-stu-id="8376c-171">description</span></span>          | <span data-ttu-id="8376c-172">строка</span><span class="sxs-lookup"><span data-stu-id="8376c-172">string</span></span>            | <span data-ttu-id="8376c-173">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="8376c-173">The descriptive text for the item.</span></span>
| <span data-ttu-id="8376c-174">eTag</span><span class="sxs-lookup"><span data-stu-id="8376c-174">eTag</span></span>                 | <span data-ttu-id="8376c-175">string</span><span class="sxs-lookup"><span data-stu-id="8376c-175">string</span></span>            | <span data-ttu-id="8376c-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8376c-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="8376c-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8376c-178">lastModifiedBy</span></span>       | <span data-ttu-id="8376c-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8376c-179">[identitySet][]</span></span>   | <span data-ttu-id="8376c-180">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="8376c-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="8376c-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8376c-181">Read-only.</span></span>
| <span data-ttu-id="8376c-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8376c-182">lastModifiedDateTime</span></span> | <span data-ttu-id="8376c-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8376c-183">DateTimeOffset</span></span>    | <span data-ttu-id="8376c-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8376c-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="8376c-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="8376c-186">parentReference</span></span>      | <span data-ttu-id="8376c-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="8376c-187">[itemReference][]</span></span> | <span data-ttu-id="8376c-p109">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="8376c-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="8376c-190">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="8376c-190">sharepointIds</span></span>        | <span data-ttu-id="8376c-191">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="8376c-191">[sharepointIds][]</span></span> | <span data-ttu-id="8376c-p110">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8376c-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="8376c-194">webUrl</span><span class="sxs-lookup"><span data-stu-id="8376c-194">webUrl</span></span>               | <span data-ttu-id="8376c-195">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="8376c-195">string (url)</span></span>      | <span data-ttu-id="8376c-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8376c-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="8376c-198">Связи</span><span class="sxs-lookup"><span data-stu-id="8376c-198">Relationships</span></span>

 <span data-ttu-id="8376c-199">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="8376c-199">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="8376c-200">Имя связи</span><span class="sxs-lookup"><span data-stu-id="8376c-200">Relationship name</span></span> | <span data-ttu-id="8376c-201">Тип</span><span class="sxs-lookup"><span data-stu-id="8376c-201">Type</span></span>                           | <span data-ttu-id="8376c-202">Описание</span><span class="sxs-lookup"><span data-stu-id="8376c-202">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="8376c-203">activities</span><span class="sxs-lookup"><span data-stu-id="8376c-203">activities</span></span>        | <span data-ttu-id="8376c-204">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="8376c-204">[itemActivity][] collection</span></span>    | <span data-ttu-id="8376c-205">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="8376c-205">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="8376c-206">analytics</span><span class="sxs-lookup"><span data-stu-id="8376c-206">analytics</span></span>         | <span data-ttu-id="8376c-207">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="8376c-207">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="8376c-208">Аналитические данные о действиях просмотра, выполненных для элемента.</span><span class="sxs-lookup"><span data-stu-id="8376c-208">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="8376c-209">driveItem</span><span class="sxs-lookup"><span data-stu-id="8376c-209">driveItem</span></span>         | <span data-ttu-id="8376c-210">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="8376c-210">[driveItem][]</span></span>                  | <span data-ttu-id="8376c-211">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="8376c-211">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="8376c-212">fields</span><span class="sxs-lookup"><span data-stu-id="8376c-212">fields</span></span>            | <span data-ttu-id="8376c-213">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="8376c-213">[fieldValueSet][]</span></span>              | <span data-ttu-id="8376c-214">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="8376c-214">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="8376c-215">versions</span><span class="sxs-lookup"><span data-stu-id="8376c-215">versions</span></span>          | <span data-ttu-id="8376c-216">Коллекция [listItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="8376c-216">[listItemVersion][] collection</span></span> | <span data-ttu-id="8376c-217">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="8376c-217">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="8376c-229">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8376c-229">JSON representation</span></span>

<span data-ttu-id="8376c-230">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8376c-230">Here is a JSON representation of a **listItem** resource.</span></span>

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
