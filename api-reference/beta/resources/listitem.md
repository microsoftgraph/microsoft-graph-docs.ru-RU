---
author: JeremyKelley
description: Этот ресурс представляет элемент объекта list в SharePoint.
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ad1e278f31bbeb0bc079f1ad2a6345d9b260cdec
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941468"
---
# <a name="listitem-resource"></a><span data-ttu-id="29a14-103">Ресурс ListItem</span><span class="sxs-lookup"><span data-stu-id="29a14-103">ListItem resource</span></span>

<span data-ttu-id="29a14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29a14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29a14-105">Представляет элемент объекта [list][] в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="29a14-105">Represents an item in a SharePoint [list][].</span></span>

<span data-ttu-id="29a14-106">Все элементы в библиотеке документов SharePoint могут быть представлены как ресурс **listItem** или [driveItem][].</span><span class="sxs-lookup"><span data-stu-id="29a14-106">All items in a SharePoint document library can be represented as a **listItem** or [driveItem][] resource.</span></span>

<span data-ttu-id="29a14-107">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="29a14-107">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="29a14-108">Задачи для ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="29a14-108">Tasks on a listItem</span></span>

<span data-ttu-id="29a14-109">Ниже перечислены задачи, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="29a14-109">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="29a14-110">Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="29a14-110">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="29a14-111">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="29a14-111">Common task</span></span>                    | <span data-ttu-id="29a14-112">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="29a14-112">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="29a14-113">[Получение][]</span><span class="sxs-lookup"><span data-stu-id="29a14-113">[Get][]</span></span>                        | <span data-ttu-id="29a14-114">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="29a14-114">GET /items/{item-id}</span></span>
| <span data-ttu-id="29a14-115">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="29a14-115">[Get column values][Get]</span></span>       | <span data-ttu-id="29a14-116">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="29a14-116">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="29a14-117">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="29a14-117">[Get analytics][]</span></span>              | <span data-ttu-id="29a14-118">GET /items/{item-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="29a14-118">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="29a14-119">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="29a14-119">[Get activities by interval][]</span></span> | <span data-ttu-id="29a14-120">GET /items/{item-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="29a14-120">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="29a14-121">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="29a14-121">[Create][]</span></span>                     | <span data-ttu-id="29a14-122">POST /items</span><span class="sxs-lookup"><span data-stu-id="29a14-122">POST /items</span></span>
| <span data-ttu-id="29a14-123">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="29a14-123">[Delete][]</span></span>                     | <span data-ttu-id="29a14-124">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="29a14-124">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="29a14-125">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="29a14-125">[Update][]</span></span>                     | <span data-ttu-id="29a14-126">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="29a14-126">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="29a14-127">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="29a14-127">[Update column values][Update]</span></span> | <span data-ttu-id="29a14-128">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="29a14-128">PATCH /items/{item-id}/fields</span></span>
| <span data-ttu-id="29a14-129">[createLink][CreateLink]</span><span class="sxs-lookup"><span data-stu-id="29a14-129">[createLink][CreateLink]</span></span>       | <span data-ttu-id="29a14-130">POST /items/{itemId}/createLink</span><span class="sxs-lookup"><span data-stu-id="29a14-130">POST /items/{itemId}/createLink</span></span>

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
[CreateLink]: ../api/listitem-createlink.md

## <a name="json-representation"></a><span data-ttu-id="29a14-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="29a14-137">JSON representation</span></span>

<span data-ttu-id="29a14-138">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29a14-138">Here is a JSON representation of a **listItem** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type&quot;: &quot;microsoft.graph.listItem"
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
  "webUrl&quot;: &quot;url"
}
```

## <a name="properties"></a><span data-ttu-id="29a14-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="29a14-139">Properties</span></span>

<span data-ttu-id="29a14-140">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="29a14-140">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="29a14-141">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="29a14-141">Property name</span></span> | <span data-ttu-id="29a14-142">Тип</span><span class="sxs-lookup"><span data-stu-id="29a14-142">Type</span></span>                | <span data-ttu-id="29a14-143">Описание</span><span class="sxs-lookup"><span data-stu-id="29a14-143">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="29a14-144">contentType</span><span class="sxs-lookup"><span data-stu-id="29a14-144">contentType</span></span>   | <span data-ttu-id="29a14-145">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="29a14-145">[contentTypeInfo][]</span></span> | <span data-ttu-id="29a14-146">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="29a14-146">The content type of this list item</span></span>

<span data-ttu-id="29a14-147">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="29a14-147">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="29a14-148">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="29a14-148">Property name</span></span>        | <span data-ttu-id="29a14-149">Тип</span><span class="sxs-lookup"><span data-stu-id="29a14-149">Type</span></span>              | <span data-ttu-id="29a14-150">Описание</span><span class="sxs-lookup"><span data-stu-id="29a14-150">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="29a14-151">id</span><span class="sxs-lookup"><span data-stu-id="29a14-151">id</span></span>                   | <span data-ttu-id="29a14-152">string</span><span class="sxs-lookup"><span data-stu-id="29a14-152">string</span></span>            | <span data-ttu-id="29a14-p102">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29a14-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="29a14-155">name</span><span class="sxs-lookup"><span data-stu-id="29a14-155">name</span></span>                 | <span data-ttu-id="29a14-156">string</span><span class="sxs-lookup"><span data-stu-id="29a14-156">string</span></span>            | <span data-ttu-id="29a14-157">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="29a14-157">The name / title of the item.</span></span>
| <span data-ttu-id="29a14-158">createdBy</span><span class="sxs-lookup"><span data-stu-id="29a14-158">createdBy</span></span>            | <span data-ttu-id="29a14-159">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="29a14-159">[identitySet][]</span></span>   | <span data-ttu-id="29a14-160">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="29a14-160">Identity of the creator of this item.</span></span> <span data-ttu-id="29a14-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29a14-161">Read-only.</span></span>
| <span data-ttu-id="29a14-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29a14-162">createdDateTime</span></span>      | <span data-ttu-id="29a14-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29a14-163">DateTimeOffset</span></span>    | <span data-ttu-id="29a14-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29a14-p104">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="29a14-166">description</span><span class="sxs-lookup"><span data-stu-id="29a14-166">description</span></span>          | <span data-ttu-id="29a14-167">строка</span><span class="sxs-lookup"><span data-stu-id="29a14-167">string</span></span>            | <span data-ttu-id="29a14-168">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="29a14-168">The descriptive text for the item.</span></span>
| <span data-ttu-id="29a14-169">eTag</span><span class="sxs-lookup"><span data-stu-id="29a14-169">eTag</span></span>                 | <span data-ttu-id="29a14-170">string</span><span class="sxs-lookup"><span data-stu-id="29a14-170">string</span></span>            | <span data-ttu-id="29a14-p105">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29a14-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="29a14-173">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="29a14-173">lastModifiedBy</span></span>       | <span data-ttu-id="29a14-174">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="29a14-174">[identitySet][]</span></span>   | <span data-ttu-id="29a14-175">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="29a14-175">Identity of the last modifier of this item.</span></span> <span data-ttu-id="29a14-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29a14-176">Read-only.</span></span>
| <span data-ttu-id="29a14-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29a14-177">lastModifiedDateTime</span></span> | <span data-ttu-id="29a14-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29a14-178">DateTimeOffset</span></span>    | <span data-ttu-id="29a14-p107">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29a14-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="29a14-181">parentReference</span><span class="sxs-lookup"><span data-stu-id="29a14-181">parentReference</span></span>      | <span data-ttu-id="29a14-182">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="29a14-182">[itemReference][]</span></span> | <span data-ttu-id="29a14-p108">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="29a14-p108">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="29a14-185">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="29a14-185">sharepointIds</span></span>        | <span data-ttu-id="29a14-186">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="29a14-186">[sharepointIds][]</span></span> | <span data-ttu-id="29a14-p109">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29a14-p109">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="29a14-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="29a14-189">webUrl</span></span>               | <span data-ttu-id="29a14-190">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="29a14-190">string (url)</span></span>      | <span data-ttu-id="29a14-p110">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29a14-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="29a14-193">Связи</span><span class="sxs-lookup"><span data-stu-id="29a14-193">Relationships</span></span>

 <span data-ttu-id="29a14-194">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="29a14-194">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="29a14-195">Имя связи</span><span class="sxs-lookup"><span data-stu-id="29a14-195">Relationship name</span></span> | <span data-ttu-id="29a14-196">Тип</span><span class="sxs-lookup"><span data-stu-id="29a14-196">Type</span></span>                           | <span data-ttu-id="29a14-197">Описание</span><span class="sxs-lookup"><span data-stu-id="29a14-197">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="29a14-198">activities</span><span class="sxs-lookup"><span data-stu-id="29a14-198">activities</span></span>        | <span data-ttu-id="29a14-199">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="29a14-199">[itemActivity][] collection</span></span>    | <span data-ttu-id="29a14-200">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="29a14-200">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="29a14-201">analytics</span><span class="sxs-lookup"><span data-stu-id="29a14-201">analytics</span></span>         | <span data-ttu-id="29a14-202">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="29a14-202">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="29a14-203">Аналитические данные о действиях просмотра, выполненных для элемента.</span><span class="sxs-lookup"><span data-stu-id="29a14-203">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="29a14-204">driveItem</span><span class="sxs-lookup"><span data-stu-id="29a14-204">driveItem</span></span>         | <span data-ttu-id="29a14-205">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="29a14-205">[driveItem][]</span></span>                  | <span data-ttu-id="29a14-206">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="29a14-206">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="29a14-207">fields</span><span class="sxs-lookup"><span data-stu-id="29a14-207">fields</span></span>            | <span data-ttu-id="29a14-208">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="29a14-208">[fieldValueSet][]</span></span>              | <span data-ttu-id="29a14-209">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="29a14-209">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="29a14-210">versions</span><span class="sxs-lookup"><span data-stu-id="29a14-210">versions</span></span>          | <span data-ttu-id="29a14-211">Коллекция [listItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="29a14-211">[listItemVersion][] collection</span></span> | <span data-ttu-id="29a14-212">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="29a14-212">The list of previous versions of the list item.</span></span>

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
    "ListItem&quot;: &quot;#"
  },
  "suppressions": []
}
-->


