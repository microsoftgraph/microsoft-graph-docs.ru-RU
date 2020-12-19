---
author: JeremyKelley
title: Ресурс listItem
description: Представляет элемент объекта list в SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 7e9e7b00ee87127b7844d2d7208d63c8e4fb6af5
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714118"
---
# <a name="listitem-resource"></a><span data-ttu-id="643fe-103">Ресурс listItem</span><span class="sxs-lookup"><span data-stu-id="643fe-103">listItem resource</span></span>

<span data-ttu-id="643fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="643fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="643fe-105">Представляет элемент объекта [list][] в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="643fe-105">Represents an item in a SharePoint [list][].</span></span>

<span data-ttu-id="643fe-106">Все элементы в библиотеке документов SharePoint могут быть представлены как ресурс **listItem** или [driveItem][].</span><span class="sxs-lookup"><span data-stu-id="643fe-106">All items in a SharePoint document library can be represented as a **listItem** or [driveItem][] resource.</span></span>

<span data-ttu-id="643fe-107">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="643fe-107">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="643fe-108">Методы</span><span class="sxs-lookup"><span data-stu-id="643fe-108">Methods</span></span>

<span data-ttu-id="643fe-109">Ниже перечислены методы, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="643fe-109">The following methods are available for **listItem** resources.</span></span>
<span data-ttu-id="643fe-110">Все примеры относятся к объекту **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="643fe-110">All examples are relative to a **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="643fe-111">Метод</span><span class="sxs-lookup"><span data-stu-id="643fe-111">Method</span></span>                    | <span data-ttu-id="643fe-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="643fe-112">Return Type</span></span> | <span data-ttu-id="643fe-113">Описание</span><span class="sxs-lookup"><span data-stu-id="643fe-113">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="643fe-114">[получение][];</span><span class="sxs-lookup"><span data-stu-id="643fe-114">[Get][]</span></span>                   | <span data-ttu-id="643fe-115">listItem</span><span class="sxs-lookup"><span data-stu-id="643fe-115">listItem</span></span>| <span data-ttu-id="643fe-116">Получение элемента списка.</span><span class="sxs-lookup"><span data-stu-id="643fe-116">Get an item in a list.</span></span>
| <span data-ttu-id="643fe-117">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="643fe-117">[Get column values][Get]</span></span>       | <span data-ttu-id="643fe-118">listItem</span><span class="sxs-lookup"><span data-stu-id="643fe-118">listItem</span></span> | <span data-ttu-id="643fe-119">Получение значений столбцов из ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="643fe-119">Get column values from listItem.</span></span>
| <span data-ttu-id="643fe-120">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="643fe-120">[Get analytics][]</span></span>              | <span data-ttu-id="643fe-121">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="643fe-121">[itemAnalytics][]</span></span>| <span data-ttu-id="643fe-122">Получение аналитических данных для ресурса.</span><span class="sxs-lookup"><span data-stu-id="643fe-122">Get analytics for this resource.</span></span> 
| <span data-ttu-id="643fe-123">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="643fe-123">[Get activities by interval][]</span></span> | <span data-ttu-id="643fe-124">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="643fe-124">[itemActivityStat][]</span></span>| <span data-ttu-id="643fe-125">Получение коллекции объектов itemActivityStat в пределах указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="643fe-125">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="643fe-126">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="643fe-126">[Create][]</span></span>                     | <span data-ttu-id="643fe-127">listItem</span><span class="sxs-lookup"><span data-stu-id="643fe-127">listItem</span></span> | <span data-ttu-id="643fe-128">Создание ресурса listItem в списке.</span><span class="sxs-lookup"><span data-stu-id="643fe-128">Create a new listItem in a list.</span></span>
| <span data-ttu-id="643fe-129">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="643fe-129">[Delete][]</span></span>                     | <span data-ttu-id="643fe-130">Содержимое отсутствует</span><span class="sxs-lookup"><span data-stu-id="643fe-130">No Content</span></span> | <span data-ttu-id="643fe-131">Удаление элемента из списка.</span><span class="sxs-lookup"><span data-stu-id="643fe-131">Removes an item from a list.</span></span>
| <span data-ttu-id="643fe-132">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="643fe-132">[Update][]</span></span>                     | <span data-ttu-id="643fe-133">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="643fe-133">[fieldValueSet][]</span></span>| <span data-ttu-id="643fe-134">Изменение свойств ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="643fe-134">Update the properties on a listItem.</span></span>
| <span data-ttu-id="643fe-135">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="643fe-135">[Update column values][Update]</span></span> | <span data-ttu-id="643fe-136">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="643fe-136">[fieldValueSet][]</span></span>| <span data-ttu-id="643fe-137">Изменение значений столбцов ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="643fe-137">Update column values on a listItem.</span></span>

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

## <a name="properties"></a><span data-ttu-id="643fe-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="643fe-146">Properties</span></span>

<span data-ttu-id="643fe-147">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="643fe-147">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="643fe-148">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="643fe-148">Property name</span></span> | <span data-ttu-id="643fe-149">Тип</span><span class="sxs-lookup"><span data-stu-id="643fe-149">Type</span></span>                | <span data-ttu-id="643fe-150">Описание</span><span class="sxs-lookup"><span data-stu-id="643fe-150">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="643fe-151">contentType</span><span class="sxs-lookup"><span data-stu-id="643fe-151">contentType</span></span>   | <span data-ttu-id="643fe-152">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="643fe-152">[contentTypeInfo][]</span></span> | <span data-ttu-id="643fe-153">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="643fe-153">The content type of this list item</span></span>

<span data-ttu-id="643fe-154">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="643fe-154">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="643fe-155">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="643fe-155">Property name</span></span>        | <span data-ttu-id="643fe-156">Тип</span><span class="sxs-lookup"><span data-stu-id="643fe-156">Type</span></span>              | <span data-ttu-id="643fe-157">Описание</span><span class="sxs-lookup"><span data-stu-id="643fe-157">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="643fe-158">id</span><span class="sxs-lookup"><span data-stu-id="643fe-158">id</span></span>                   | <span data-ttu-id="643fe-159">string</span><span class="sxs-lookup"><span data-stu-id="643fe-159">string</span></span>            | <span data-ttu-id="643fe-p102">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="643fe-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="643fe-162">name</span><span class="sxs-lookup"><span data-stu-id="643fe-162">name</span></span>                 | <span data-ttu-id="643fe-163">string</span><span class="sxs-lookup"><span data-stu-id="643fe-163">string</span></span>            | <span data-ttu-id="643fe-164">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="643fe-164">The name / title of the item.</span></span>
| <span data-ttu-id="643fe-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="643fe-165">createdBy</span></span>            | <span data-ttu-id="643fe-166">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="643fe-166">[identitySet][]</span></span>   | <span data-ttu-id="643fe-167">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="643fe-167">Identity of the creator of this item.</span></span> <span data-ttu-id="643fe-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="643fe-168">Read-only.</span></span>
| <span data-ttu-id="643fe-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="643fe-169">createdDateTime</span></span>      | <span data-ttu-id="643fe-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="643fe-170">DateTimeOffset</span></span>    | <span data-ttu-id="643fe-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="643fe-p104">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="643fe-173">description</span><span class="sxs-lookup"><span data-stu-id="643fe-173">description</span></span>          | <span data-ttu-id="643fe-174">строка</span><span class="sxs-lookup"><span data-stu-id="643fe-174">string</span></span>            | <span data-ttu-id="643fe-175">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="643fe-175">The descriptive text for the item.</span></span>
| <span data-ttu-id="643fe-176">eTag</span><span class="sxs-lookup"><span data-stu-id="643fe-176">eTag</span></span>                 | <span data-ttu-id="643fe-177">string</span><span class="sxs-lookup"><span data-stu-id="643fe-177">string</span></span>            | <span data-ttu-id="643fe-p105">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="643fe-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="643fe-180">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="643fe-180">lastModifiedBy</span></span>       | <span data-ttu-id="643fe-181">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="643fe-181">[identitySet][]</span></span>   | <span data-ttu-id="643fe-182">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="643fe-182">Identity of the last modifier of this item.</span></span> <span data-ttu-id="643fe-183">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="643fe-183">Read-only.</span></span>
| <span data-ttu-id="643fe-184">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="643fe-184">lastModifiedDateTime</span></span> | <span data-ttu-id="643fe-185">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="643fe-185">DateTimeOffset</span></span>    | <span data-ttu-id="643fe-p107">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="643fe-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="643fe-188">parentReference</span><span class="sxs-lookup"><span data-stu-id="643fe-188">parentReference</span></span>      | <span data-ttu-id="643fe-189">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="643fe-189">[itemReference][]</span></span> | <span data-ttu-id="643fe-p108">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="643fe-p108">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="643fe-192">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="643fe-192">sharepointIds</span></span>        | <span data-ttu-id="643fe-193">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="643fe-193">[sharepointIds][]</span></span> | <span data-ttu-id="643fe-p109">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="643fe-p109">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="643fe-196">webUrl</span><span class="sxs-lookup"><span data-stu-id="643fe-196">webUrl</span></span>               | <span data-ttu-id="643fe-197">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="643fe-197">string (url)</span></span>      | <span data-ttu-id="643fe-p110">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="643fe-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="643fe-200">Связи</span><span class="sxs-lookup"><span data-stu-id="643fe-200">Relationships</span></span>

 <span data-ttu-id="643fe-201">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="643fe-201">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="643fe-202">Имя связи</span><span class="sxs-lookup"><span data-stu-id="643fe-202">Relationship name</span></span> | <span data-ttu-id="643fe-203">Тип</span><span class="sxs-lookup"><span data-stu-id="643fe-203">Type</span></span>                           | <span data-ttu-id="643fe-204">Описание</span><span class="sxs-lookup"><span data-stu-id="643fe-204">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="643fe-205">activities</span><span class="sxs-lookup"><span data-stu-id="643fe-205">activities</span></span>        | <span data-ttu-id="643fe-206">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="643fe-206">[itemActivity][] collection</span></span>    | <span data-ttu-id="643fe-207">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="643fe-207">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="643fe-208">analytics</span><span class="sxs-lookup"><span data-stu-id="643fe-208">analytics</span></span>         | <span data-ttu-id="643fe-209">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="643fe-209">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="643fe-210">Аналитические данные о действиях просмотра, выполненных для элемента.</span><span class="sxs-lookup"><span data-stu-id="643fe-210">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="643fe-211">driveItem</span><span class="sxs-lookup"><span data-stu-id="643fe-211">driveItem</span></span>         | <span data-ttu-id="643fe-212">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="643fe-212">[driveItem][]</span></span>                  | <span data-ttu-id="643fe-213">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="643fe-213">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="643fe-214">fields</span><span class="sxs-lookup"><span data-stu-id="643fe-214">fields</span></span>            | <span data-ttu-id="643fe-215">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="643fe-215">[fieldValueSet][]</span></span>              | <span data-ttu-id="643fe-216">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="643fe-216">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="643fe-217">versions</span><span class="sxs-lookup"><span data-stu-id="643fe-217">versions</span></span>          | <span data-ttu-id="643fe-218">Коллекция [listItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="643fe-218">[listItemVersion][] collection</span></span> | <span data-ttu-id="643fe-219">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="643fe-219">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="643fe-231">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="643fe-231">JSON representation</span></span>

<span data-ttu-id="643fe-232">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="643fe-232">Here is a JSON representation of a **listItem** resource.</span></span>

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

