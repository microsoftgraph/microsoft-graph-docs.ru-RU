---
author: JeremyKelley
ms.author: JeremyKelley
title: Ресурс listItem
description: Представляет элемент объекта list в SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 276a8f61cc12cb2860bab0025d430f039b96b89a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025216"
---
# <a name="listitem-resource"></a><span data-ttu-id="4455d-103">Ресурс listItem</span><span class="sxs-lookup"><span data-stu-id="4455d-103">listItem resource</span></span>

<span data-ttu-id="4455d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4455d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4455d-105">Представляет элемент объекта **[list][]** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4455d-105">Represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="4455d-106">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="4455d-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="4455d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="4455d-107">Methods</span></span>

<span data-ttu-id="4455d-108">Ниже перечислены методы, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="4455d-108">The following methods are available for **listItem** resources.</span></span>
<span data-ttu-id="4455d-109">Все примеры относятся к объекту **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="4455d-109">All examples are relative to a **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="4455d-110">Метод</span><span class="sxs-lookup"><span data-stu-id="4455d-110">Method</span></span>                    | <span data-ttu-id="4455d-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4455d-111">Return Type</span></span> | <span data-ttu-id="4455d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4455d-112">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="4455d-113">[получение][];</span><span class="sxs-lookup"><span data-stu-id="4455d-113">[Get][]</span></span>                   | <span data-ttu-id="4455d-114">listItem</span><span class="sxs-lookup"><span data-stu-id="4455d-114">listItem</span></span>| <span data-ttu-id="4455d-115">Получение элемента списка.</span><span class="sxs-lookup"><span data-stu-id="4455d-115">Get an item in a list.</span></span>
| <span data-ttu-id="4455d-116">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="4455d-116">[Get column values][Get]</span></span>       | <span data-ttu-id="4455d-117">listItem</span><span class="sxs-lookup"><span data-stu-id="4455d-117">listItem</span></span> | <span data-ttu-id="4455d-118">Получение значений столбцов из ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="4455d-118">Get column values from listItem.</span></span>
| <span data-ttu-id="4455d-119">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="4455d-119">[Get analytics][]</span></span>              | <span data-ttu-id="4455d-120">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="4455d-120">[itemAnalytics][]</span></span>| <span data-ttu-id="4455d-121">Получение аналитических данных для ресурса.</span><span class="sxs-lookup"><span data-stu-id="4455d-121">Get analytics for this resource.</span></span> 
| <span data-ttu-id="4455d-122">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="4455d-122">[Get activities by interval][]</span></span> | <span data-ttu-id="4455d-123">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="4455d-123">[itemActivityStat][]</span></span>| <span data-ttu-id="4455d-124">Получение коллекции объектов itemActivityStat в пределах указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="4455d-124">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="4455d-125">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="4455d-125">[Create][]</span></span>                     | <span data-ttu-id="4455d-126">listItem</span><span class="sxs-lookup"><span data-stu-id="4455d-126">listItem</span></span> | <span data-ttu-id="4455d-127">Создание ресурса listItem в списке.</span><span class="sxs-lookup"><span data-stu-id="4455d-127">Create a new listItem in a list.</span></span>
| <span data-ttu-id="4455d-128">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="4455d-128">[Delete][]</span></span>                     | <span data-ttu-id="4455d-129">Содержимое отсутствует</span><span class="sxs-lookup"><span data-stu-id="4455d-129">No Content</span></span> | <span data-ttu-id="4455d-130">Удаление элемента из списка.</span><span class="sxs-lookup"><span data-stu-id="4455d-130">Removes an item from a list.</span></span>
| <span data-ttu-id="4455d-131">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="4455d-131">[Update][]</span></span>                     | <span data-ttu-id="4455d-132">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="4455d-132">[fieldValueSet][]</span></span>| <span data-ttu-id="4455d-133">Изменение свойств ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="4455d-133">Update the properties on a listItem.</span></span>
| <span data-ttu-id="4455d-134">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="4455d-134">[Update column values][Update]</span></span> | <span data-ttu-id="4455d-135">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="4455d-135">[fieldValueSet][]</span></span>| <span data-ttu-id="4455d-136">Изменение значений столбцов ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="4455d-136">Update column values on a listItem.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4455d-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="4455d-145">Properties</span></span>

<span data-ttu-id="4455d-146">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="4455d-146">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="4455d-147">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4455d-147">Property name</span></span> | <span data-ttu-id="4455d-148">Тип</span><span class="sxs-lookup"><span data-stu-id="4455d-148">Type</span></span>                | <span data-ttu-id="4455d-149">Описание</span><span class="sxs-lookup"><span data-stu-id="4455d-149">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="4455d-150">contentType</span><span class="sxs-lookup"><span data-stu-id="4455d-150">contentType</span></span>   | <span data-ttu-id="4455d-151">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="4455d-151">[contentTypeInfo][]</span></span> | <span data-ttu-id="4455d-152">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="4455d-152">The content type of this list item</span></span>

<span data-ttu-id="4455d-153">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="4455d-153">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="4455d-154">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4455d-154">Property name</span></span>        | <span data-ttu-id="4455d-155">Тип</span><span class="sxs-lookup"><span data-stu-id="4455d-155">Type</span></span>              | <span data-ttu-id="4455d-156">Описание</span><span class="sxs-lookup"><span data-stu-id="4455d-156">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="4455d-157">id</span><span class="sxs-lookup"><span data-stu-id="4455d-157">id</span></span>                   | <span data-ttu-id="4455d-158">string</span><span class="sxs-lookup"><span data-stu-id="4455d-158">string</span></span>            | <span data-ttu-id="4455d-p103">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4455d-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="4455d-161">name</span><span class="sxs-lookup"><span data-stu-id="4455d-161">name</span></span>                 | <span data-ttu-id="4455d-162">string</span><span class="sxs-lookup"><span data-stu-id="4455d-162">string</span></span>            | <span data-ttu-id="4455d-163">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="4455d-163">The name / title of the item.</span></span>
| <span data-ttu-id="4455d-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="4455d-164">createdBy</span></span>            | <span data-ttu-id="4455d-165">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4455d-165">[identitySet][]</span></span>   | <span data-ttu-id="4455d-166">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="4455d-166">Identity of the creator of this item.</span></span> <span data-ttu-id="4455d-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4455d-167">Read-only.</span></span>
| <span data-ttu-id="4455d-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4455d-168">createdDateTime</span></span>      | <span data-ttu-id="4455d-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4455d-169">DateTimeOffset</span></span>    | <span data-ttu-id="4455d-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4455d-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="4455d-172">description</span><span class="sxs-lookup"><span data-stu-id="4455d-172">description</span></span>          | <span data-ttu-id="4455d-173">строка</span><span class="sxs-lookup"><span data-stu-id="4455d-173">string</span></span>            | <span data-ttu-id="4455d-174">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="4455d-174">The descriptive text for the item.</span></span>
| <span data-ttu-id="4455d-175">eTag</span><span class="sxs-lookup"><span data-stu-id="4455d-175">eTag</span></span>                 | <span data-ttu-id="4455d-176">string</span><span class="sxs-lookup"><span data-stu-id="4455d-176">string</span></span>            | <span data-ttu-id="4455d-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4455d-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="4455d-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4455d-179">lastModifiedBy</span></span>       | <span data-ttu-id="4455d-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4455d-180">[identitySet][]</span></span>   | <span data-ttu-id="4455d-181">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="4455d-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="4455d-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4455d-182">Read-only.</span></span>
| <span data-ttu-id="4455d-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4455d-183">lastModifiedDateTime</span></span> | <span data-ttu-id="4455d-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4455d-184">DateTimeOffset</span></span>    | <span data-ttu-id="4455d-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4455d-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="4455d-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="4455d-187">parentReference</span></span>      | <span data-ttu-id="4455d-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="4455d-188">[itemReference][]</span></span> | <span data-ttu-id="4455d-p109">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="4455d-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="4455d-191">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="4455d-191">sharepointIds</span></span>        | <span data-ttu-id="4455d-192">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="4455d-192">[sharepointIds][]</span></span> | <span data-ttu-id="4455d-p110">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4455d-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="4455d-195">webUrl</span><span class="sxs-lookup"><span data-stu-id="4455d-195">webUrl</span></span>               | <span data-ttu-id="4455d-196">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="4455d-196">string (url)</span></span>      | <span data-ttu-id="4455d-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4455d-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="4455d-199">Связи</span><span class="sxs-lookup"><span data-stu-id="4455d-199">Relationships</span></span>

 <span data-ttu-id="4455d-200">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="4455d-200">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="4455d-201">Имя связи</span><span class="sxs-lookup"><span data-stu-id="4455d-201">Relationship name</span></span> | <span data-ttu-id="4455d-202">Тип</span><span class="sxs-lookup"><span data-stu-id="4455d-202">Type</span></span>                           | <span data-ttu-id="4455d-203">Описание</span><span class="sxs-lookup"><span data-stu-id="4455d-203">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="4455d-204">activities</span><span class="sxs-lookup"><span data-stu-id="4455d-204">activities</span></span>        | <span data-ttu-id="4455d-205">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="4455d-205">[itemActivity][] collection</span></span>    | <span data-ttu-id="4455d-206">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="4455d-206">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="4455d-207">analytics</span><span class="sxs-lookup"><span data-stu-id="4455d-207">analytics</span></span>         | <span data-ttu-id="4455d-208">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="4455d-208">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="4455d-209">Аналитические данные о действиях просмотра, выполненных для элемента.</span><span class="sxs-lookup"><span data-stu-id="4455d-209">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="4455d-210">driveItem</span><span class="sxs-lookup"><span data-stu-id="4455d-210">driveItem</span></span>         | <span data-ttu-id="4455d-211">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="4455d-211">[driveItem][]</span></span>                  | <span data-ttu-id="4455d-212">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="4455d-212">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="4455d-213">fields</span><span class="sxs-lookup"><span data-stu-id="4455d-213">fields</span></span>            | <span data-ttu-id="4455d-214">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="4455d-214">[fieldValueSet][]</span></span>              | <span data-ttu-id="4455d-215">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="4455d-215">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="4455d-216">versions</span><span class="sxs-lookup"><span data-stu-id="4455d-216">versions</span></span>          | <span data-ttu-id="4455d-217">Коллекция [listItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="4455d-217">[listItemVersion][] collection</span></span> | <span data-ttu-id="4455d-218">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="4455d-218">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="4455d-230">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4455d-230">JSON representation</span></span>

<span data-ttu-id="4455d-231">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4455d-231">Here is a JSON representation of a **listItem** resource.</span></span>

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

