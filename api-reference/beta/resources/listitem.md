---
author: JeremyKelley
description: Этот ресурс представляет элемент объекта list в SharePoint.
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e457840ee55206b47b035ae53127c5bf3e5130c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055262"
---
# <a name="listitem-resource"></a><span data-ttu-id="97d3a-103">Ресурс ListItem</span><span class="sxs-lookup"><span data-stu-id="97d3a-103">ListItem resource</span></span>

<span data-ttu-id="97d3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97d3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97d3a-105">Этот ресурс представляет элемент объекта **[list][]** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="97d3a-105">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="97d3a-106">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="97d3a-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="97d3a-107">Задачи для ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="97d3a-107">Tasks on a listItem</span></span>

<span data-ttu-id="97d3a-108">Ниже перечислены задачи, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="97d3a-108">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="97d3a-109">Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="97d3a-109">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="97d3a-110">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="97d3a-110">Common task</span></span>                    | <span data-ttu-id="97d3a-111">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="97d3a-111">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="97d3a-112">[Получение][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-112">[Get][]</span></span>                        | <span data-ttu-id="97d3a-113">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="97d3a-113">GET /items/{item-id}</span></span>
| <span data-ttu-id="97d3a-114">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="97d3a-114">[Get column values][Get]</span></span>       | <span data-ttu-id="97d3a-115">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="97d3a-115">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="97d3a-116">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-116">[Get analytics][]</span></span>              | <span data-ttu-id="97d3a-117">ПОЛУЧЕНИЕ/итемс/{итем-ИД}/Аналитикс</span><span class="sxs-lookup"><span data-stu-id="97d3a-117">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="97d3a-118">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-118">[Get activities by interval][]</span></span> | <span data-ttu-id="97d3a-119">ПОЛУЧЕНИЕ/Итемс/{итем-ИД}/жетактивитиесбинтервал</span><span class="sxs-lookup"><span data-stu-id="97d3a-119">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="97d3a-120">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-120">[Create][]</span></span>                     | <span data-ttu-id="97d3a-121">POST /items</span><span class="sxs-lookup"><span data-stu-id="97d3a-121">POST /items</span></span>
| <span data-ttu-id="97d3a-122">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-122">[Delete][]</span></span>                     | <span data-ttu-id="97d3a-123">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="97d3a-123">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="97d3a-124">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-124">[Update][]</span></span>                     | <span data-ttu-id="97d3a-125">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="97d3a-125">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="97d3a-126">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="97d3a-126">[Update column values][Update]</span></span> | <span data-ttu-id="97d3a-127">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="97d3a-127">PATCH /items/{item-id}/fields</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="97d3a-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="97d3a-134">JSON representation</span></span>

<span data-ttu-id="97d3a-135">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97d3a-135">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="97d3a-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="97d3a-136">Properties</span></span>

<span data-ttu-id="97d3a-137">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="97d3a-137">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="97d3a-138">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="97d3a-138">Property name</span></span> | <span data-ttu-id="97d3a-139">Тип</span><span class="sxs-lookup"><span data-stu-id="97d3a-139">Type</span></span>                | <span data-ttu-id="97d3a-140">Описание</span><span class="sxs-lookup"><span data-stu-id="97d3a-140">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="97d3a-141">contentType</span><span class="sxs-lookup"><span data-stu-id="97d3a-141">contentType</span></span>   | <span data-ttu-id="97d3a-142">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-142">[contentTypeInfo][]</span></span> | <span data-ttu-id="97d3a-143">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="97d3a-143">The content type of this list item</span></span>

<span data-ttu-id="97d3a-144">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="97d3a-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="97d3a-145">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="97d3a-145">Property name</span></span>        | <span data-ttu-id="97d3a-146">Тип</span><span class="sxs-lookup"><span data-stu-id="97d3a-146">Type</span></span>              | <span data-ttu-id="97d3a-147">Описание</span><span class="sxs-lookup"><span data-stu-id="97d3a-147">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="97d3a-148">id</span><span class="sxs-lookup"><span data-stu-id="97d3a-148">id</span></span>                   | <span data-ttu-id="97d3a-149">string</span><span class="sxs-lookup"><span data-stu-id="97d3a-149">string</span></span>            | <span data-ttu-id="97d3a-p103">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3a-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="97d3a-152">name</span><span class="sxs-lookup"><span data-stu-id="97d3a-152">name</span></span>                 | <span data-ttu-id="97d3a-153">string</span><span class="sxs-lookup"><span data-stu-id="97d3a-153">string</span></span>            | <span data-ttu-id="97d3a-154">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="97d3a-154">The name / title of the item.</span></span>
| <span data-ttu-id="97d3a-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="97d3a-155">createdBy</span></span>            | <span data-ttu-id="97d3a-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-156">[identitySet][]</span></span>   | <span data-ttu-id="97d3a-157">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="97d3a-157">Identity of the creator of this item.</span></span> <span data-ttu-id="97d3a-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3a-158">Read-only.</span></span>
| <span data-ttu-id="97d3a-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97d3a-159">createdDateTime</span></span>      | <span data-ttu-id="97d3a-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d3a-160">DateTimeOffset</span></span>    | <span data-ttu-id="97d3a-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3a-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="97d3a-163">description</span><span class="sxs-lookup"><span data-stu-id="97d3a-163">description</span></span>          | <span data-ttu-id="97d3a-164">строка</span><span class="sxs-lookup"><span data-stu-id="97d3a-164">string</span></span>            | <span data-ttu-id="97d3a-165">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="97d3a-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="97d3a-166">eTag</span><span class="sxs-lookup"><span data-stu-id="97d3a-166">eTag</span></span>                 | <span data-ttu-id="97d3a-167">string</span><span class="sxs-lookup"><span data-stu-id="97d3a-167">string</span></span>            | <span data-ttu-id="97d3a-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3a-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="97d3a-170">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="97d3a-170">lastModifiedBy</span></span>       | <span data-ttu-id="97d3a-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-171">[identitySet][]</span></span>   | <span data-ttu-id="97d3a-172">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="97d3a-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="97d3a-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3a-173">Read-only.</span></span>
| <span data-ttu-id="97d3a-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97d3a-174">lastModifiedDateTime</span></span> | <span data-ttu-id="97d3a-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d3a-175">DateTimeOffset</span></span>    | <span data-ttu-id="97d3a-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3a-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="97d3a-178">parentReference</span><span class="sxs-lookup"><span data-stu-id="97d3a-178">parentReference</span></span>      | <span data-ttu-id="97d3a-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-179">[itemReference][]</span></span> | <span data-ttu-id="97d3a-p109">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="97d3a-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="97d3a-182">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="97d3a-182">sharepointIds</span></span>        | <span data-ttu-id="97d3a-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-183">[sharepointIds][]</span></span> | <span data-ttu-id="97d3a-p110">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3a-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="97d3a-186">webUrl</span><span class="sxs-lookup"><span data-stu-id="97d3a-186">webUrl</span></span>               | <span data-ttu-id="97d3a-187">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="97d3a-187">string (url)</span></span>      | <span data-ttu-id="97d3a-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97d3a-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="97d3a-190">Связи</span><span class="sxs-lookup"><span data-stu-id="97d3a-190">Relationships</span></span>

 <span data-ttu-id="97d3a-191">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="97d3a-191">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="97d3a-192">Имя связи</span><span class="sxs-lookup"><span data-stu-id="97d3a-192">Relationship name</span></span> | <span data-ttu-id="97d3a-193">Тип</span><span class="sxs-lookup"><span data-stu-id="97d3a-193">Type</span></span>                           | <span data-ttu-id="97d3a-194">Описание</span><span class="sxs-lookup"><span data-stu-id="97d3a-194">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="97d3a-195">activities</span><span class="sxs-lookup"><span data-stu-id="97d3a-195">activities</span></span>        | <span data-ttu-id="97d3a-196">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-196">[itemActivity][] collection</span></span>    | <span data-ttu-id="97d3a-197">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="97d3a-197">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="97d3a-198">analytics</span><span class="sxs-lookup"><span data-stu-id="97d3a-198">analytics</span></span>         | <span data-ttu-id="97d3a-199">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-199">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="97d3a-200">Аналитические данные о действиях просмотра, выполненных для элемента.</span><span class="sxs-lookup"><span data-stu-id="97d3a-200">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="97d3a-201">driveItem</span><span class="sxs-lookup"><span data-stu-id="97d3a-201">driveItem</span></span>         | <span data-ttu-id="97d3a-202">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-202">[driveItem][]</span></span>                  | <span data-ttu-id="97d3a-203">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="97d3a-203">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="97d3a-204">fields</span><span class="sxs-lookup"><span data-stu-id="97d3a-204">fields</span></span>            | <span data-ttu-id="97d3a-205">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-205">[fieldValueSet][]</span></span>              | <span data-ttu-id="97d3a-206">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="97d3a-206">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="97d3a-207">versions</span><span class="sxs-lookup"><span data-stu-id="97d3a-207">versions</span></span>          | <span data-ttu-id="97d3a-208">Коллекция [listItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="97d3a-208">[listItemVersion][] collection</span></span> | <span data-ttu-id="97d3a-209">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="97d3a-209">The list of previous versions of the list item.</span></span>

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


