---
author: JeremyKelley
description: Этот ресурс представляет элемент объекта list в SharePoint.
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3c05125257eeec9d7b21a7d1eb03de79bc189ccd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009981"
---
# <a name="listitem-resource"></a><span data-ttu-id="0f4b4-103">Ресурс ListItem</span><span class="sxs-lookup"><span data-stu-id="0f4b4-103">ListItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f4b4-104">Этот ресурс представляет элемент объекта **[list][]** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-104">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="0f4b4-105">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-105">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="0f4b4-106">Задачи для ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="0f4b4-106">Tasks on a listItem</span></span>

<span data-ttu-id="0f4b4-107">Ниже перечислены задачи, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-107">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="0f4b4-108">Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-108">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="0f4b4-109">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="0f4b4-109">Common task</span></span>                    | <span data-ttu-id="0f4b4-110">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="0f4b4-110">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="0f4b4-111">[Получение][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-111">[Get][]</span></span>                        | <span data-ttu-id="0f4b4-112">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="0f4b4-112">GET /items/{item-id}</span></span>
| <span data-ttu-id="0f4b4-113">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-113">[Get column values][Get]</span></span>       | <span data-ttu-id="0f4b4-114">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="0f4b4-114">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="0f4b4-115">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-115">[Get analytics][]</span></span>              | <span data-ttu-id="0f4b4-116">ПОЛУЧЕНИЕ/итемс/{итем-ИД}/Аналитикс</span><span class="sxs-lookup"><span data-stu-id="0f4b4-116">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="0f4b4-117">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-117">[Get activities by interval][]</span></span> | <span data-ttu-id="0f4b4-118">ПОЛУЧЕНИЕ/Итемс/{итем-ИД}/жетактивитиесбинтервал</span><span class="sxs-lookup"><span data-stu-id="0f4b4-118">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="0f4b4-119">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-119">[Create][]</span></span>                     | <span data-ttu-id="0f4b4-120">POST /items</span><span class="sxs-lookup"><span data-stu-id="0f4b4-120">POST /items</span></span>
| <span data-ttu-id="0f4b4-121">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-121">[Delete][]</span></span>                     | <span data-ttu-id="0f4b4-122">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="0f4b4-122">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="0f4b4-123">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-123">[Update][]</span></span>                     | <span data-ttu-id="0f4b4-124">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="0f4b4-124">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="0f4b4-125">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-125">[Update column values][Update]</span></span> | <span data-ttu-id="0f4b4-126">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="0f4b4-126">PATCH /items/{item-id}/fields</span></span>

[Получение]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Создание]: ../api/listitem-create.md
[Create]: ../api/listitem-create.md
[Удаление]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[Обновление]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="0f4b4-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0f4b4-133">JSON representation</span></span>

<span data-ttu-id="0f4b4-134">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-134">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0f4b4-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f4b4-135">Properties</span></span>

<span data-ttu-id="0f4b4-136">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-136">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="0f4b4-137">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="0f4b4-137">Property name</span></span> | <span data-ttu-id="0f4b4-138">Тип</span><span class="sxs-lookup"><span data-stu-id="0f4b4-138">Type</span></span>                | <span data-ttu-id="0f4b4-139">Описание</span><span class="sxs-lookup"><span data-stu-id="0f4b4-139">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="0f4b4-140">contentType</span><span class="sxs-lookup"><span data-stu-id="0f4b4-140">contentType</span></span>   | <span data-ttu-id="0f4b4-141">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-141">[contentTypeInfo][]</span></span> | <span data-ttu-id="0f4b4-142">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-142">The content type of this list item</span></span>

<span data-ttu-id="0f4b4-143">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-143">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="0f4b4-144">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="0f4b4-144">Property name</span></span>        | <span data-ttu-id="0f4b4-145">Тип</span><span class="sxs-lookup"><span data-stu-id="0f4b4-145">Type</span></span>              | <span data-ttu-id="0f4b4-146">Описание</span><span class="sxs-lookup"><span data-stu-id="0f4b4-146">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="0f4b4-147">id</span><span class="sxs-lookup"><span data-stu-id="0f4b4-147">id</span></span>                   | <span data-ttu-id="0f4b4-148">строка</span><span class="sxs-lookup"><span data-stu-id="0f4b4-148">string</span></span>            | <span data-ttu-id="0f4b4-p103">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="0f4b4-151">name</span><span class="sxs-lookup"><span data-stu-id="0f4b4-151">name</span></span>                 | <span data-ttu-id="0f4b4-152">string</span><span class="sxs-lookup"><span data-stu-id="0f4b4-152">string</span></span>            | <span data-ttu-id="0f4b4-153">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-153">The name / title of the item.</span></span>
| <span data-ttu-id="0f4b4-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="0f4b4-154">createdBy</span></span>            | <span data-ttu-id="0f4b4-155">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-155">[identitySet][]</span></span>   | <span data-ttu-id="0f4b4-156">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-156">Identity of the creator of this item.</span></span> <span data-ttu-id="0f4b4-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-157">Read-only.</span></span>
| <span data-ttu-id="0f4b4-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f4b4-158">createdDateTime</span></span>      | <span data-ttu-id="0f4b4-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f4b4-159">DateTimeOffset</span></span>    | <span data-ttu-id="0f4b4-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="0f4b4-162">description</span><span class="sxs-lookup"><span data-stu-id="0f4b4-162">description</span></span>          | <span data-ttu-id="0f4b4-163">строка</span><span class="sxs-lookup"><span data-stu-id="0f4b4-163">string</span></span>            | <span data-ttu-id="0f4b4-164">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-164">The descriptive text for the item.</span></span>
| <span data-ttu-id="0f4b4-165">eTag</span><span class="sxs-lookup"><span data-stu-id="0f4b4-165">eTag</span></span>                 | <span data-ttu-id="0f4b4-166">string</span><span class="sxs-lookup"><span data-stu-id="0f4b4-166">string</span></span>            | <span data-ttu-id="0f4b4-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="0f4b4-169">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0f4b4-169">lastModifiedBy</span></span>       | <span data-ttu-id="0f4b4-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-170">[identitySet][]</span></span>   | <span data-ttu-id="0f4b4-171">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-171">Identity of the last modifier of this item.</span></span> <span data-ttu-id="0f4b4-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-172">Read-only.</span></span>
| <span data-ttu-id="0f4b4-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f4b4-173">lastModifiedDateTime</span></span> | <span data-ttu-id="0f4b4-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f4b4-174">DateTimeOffset</span></span>    | <span data-ttu-id="0f4b4-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="0f4b4-177">parentReference</span><span class="sxs-lookup"><span data-stu-id="0f4b4-177">parentReference</span></span>      | <span data-ttu-id="0f4b4-178">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-178">[itemReference][]</span></span> | <span data-ttu-id="0f4b4-p109">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="0f4b4-181">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="0f4b4-181">sharepointIds</span></span>        | <span data-ttu-id="0f4b4-182">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-182">[sharepointIds][]</span></span> | <span data-ttu-id="0f4b4-p110">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="0f4b4-185">webUrl</span><span class="sxs-lookup"><span data-stu-id="0f4b4-185">webUrl</span></span>               | <span data-ttu-id="0f4b4-186">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="0f4b4-186">string (url)</span></span>      | <span data-ttu-id="0f4b4-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="0f4b4-189">Связи</span><span class="sxs-lookup"><span data-stu-id="0f4b4-189">Relationships</span></span>

 <span data-ttu-id="0f4b4-190">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-190">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="0f4b4-191">Имя связи</span><span class="sxs-lookup"><span data-stu-id="0f4b4-191">Relationship name</span></span> | <span data-ttu-id="0f4b4-192">Тип</span><span class="sxs-lookup"><span data-stu-id="0f4b4-192">Type</span></span>                           | <span data-ttu-id="0f4b4-193">Описание</span><span class="sxs-lookup"><span data-stu-id="0f4b4-193">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="0f4b4-194">activities</span><span class="sxs-lookup"><span data-stu-id="0f4b4-194">activities</span></span>        | <span data-ttu-id="0f4b4-195">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-195">[itemActivity][] collection</span></span>    | <span data-ttu-id="0f4b4-196">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-196">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="0f4b4-197">analytics</span><span class="sxs-lookup"><span data-stu-id="0f4b4-197">analytics</span></span>         | <span data-ttu-id="0f4b4-198">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-198">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="0f4b4-199">Аналитические данные о действиях просмотра, выполненных для элемента.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-199">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="0f4b4-200">driveItem</span><span class="sxs-lookup"><span data-stu-id="0f4b4-200">driveItem</span></span>         | <span data-ttu-id="0f4b4-201">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-201">[driveItem][]</span></span>                  | <span data-ttu-id="0f4b4-202">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="0f4b4-202">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="0f4b4-203">fields</span><span class="sxs-lookup"><span data-stu-id="0f4b4-203">fields</span></span>            | <span data-ttu-id="0f4b4-204">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-204">[fieldValueSet][]</span></span>              | <span data-ttu-id="0f4b4-205">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-205">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="0f4b4-206">versions</span><span class="sxs-lookup"><span data-stu-id="0f4b4-206">versions</span></span>          | <span data-ttu-id="0f4b4-207">Коллекция [listItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="0f4b4-207">[listItemVersion][] collection</span></span> | <span data-ttu-id="0f4b4-208">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="0f4b4-208">The list of previous versions of the list item.</span></span>

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
