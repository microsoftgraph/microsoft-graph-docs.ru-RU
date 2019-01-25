---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2a405ad8a71c766642bd23adbce64c2b57b72e23
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517444"
---
# <a name="listitem-resource"></a><span data-ttu-id="bb151-102">Ресурс ListItem</span><span class="sxs-lookup"><span data-stu-id="bb151-102">ListItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb151-103">Этот ресурс представляет элемент объекта **[list][]** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bb151-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="bb151-104">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="bb151-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="bb151-105">Задачи для ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="bb151-105">Tasks on a listItem</span></span>

<span data-ttu-id="bb151-106">Ниже перечислены задачи, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="bb151-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="bb151-107">Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="bb151-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="bb151-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="bb151-108">Common task</span></span>                    | <span data-ttu-id="bb151-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="bb151-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="bb151-110">[Получение][]</span><span class="sxs-lookup"><span data-stu-id="bb151-110">[Get][]</span></span>                        | <span data-ttu-id="bb151-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="bb151-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="bb151-112">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="bb151-112">[Get column values][Get]</span></span>       | <span data-ttu-id="bb151-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="bb151-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="bb151-114">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="bb151-114">[Get analytics][]</span></span>              | <span data-ttu-id="bb151-115">GET /items/ {идентификатор элемента} / аналитики</span><span class="sxs-lookup"><span data-stu-id="bb151-115">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="bb151-116">[Получение действий по интервал][]</span><span class="sxs-lookup"><span data-stu-id="bb151-116">[Get activities by interval][]</span></span> | <span data-ttu-id="bb151-117">GET /items/ {идентификатор элемента} / getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="bb151-117">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="bb151-118">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="bb151-118">[Create][]</span></span>                     | <span data-ttu-id="bb151-119">POST /items</span><span class="sxs-lookup"><span data-stu-id="bb151-119">POST /items</span></span>
| <span data-ttu-id="bb151-120">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="bb151-120">[Delete][]</span></span>                     | <span data-ttu-id="bb151-121">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="bb151-121">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="bb151-122">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="bb151-122">[Update][]</span></span>                     | <span data-ttu-id="bb151-123">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="bb151-123">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="bb151-124">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="bb151-124">[Update column values][Update]</span></span> | <span data-ttu-id="bb151-125">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="bb151-125">PATCH /items/{item-id}/fields</span></span>

[Получение]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Получение действий по интервал]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="bb151-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bb151-132">JSON representation</span></span>

<span data-ttu-id="bb151-133">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb151-133">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="bb151-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb151-134">Properties</span></span>

<span data-ttu-id="bb151-135">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="bb151-135">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="bb151-136">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bb151-136">Property name</span></span> | <span data-ttu-id="bb151-137">Тип</span><span class="sxs-lookup"><span data-stu-id="bb151-137">Type</span></span>                | <span data-ttu-id="bb151-138">Описание</span><span class="sxs-lookup"><span data-stu-id="bb151-138">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="bb151-139">contentType</span><span class="sxs-lookup"><span data-stu-id="bb151-139">contentType</span></span>   | <span data-ttu-id="bb151-140">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="bb151-140">[contentTypeInfo][]</span></span> | <span data-ttu-id="bb151-141">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="bb151-141">The content type of this list item</span></span>

<span data-ttu-id="bb151-142">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="bb151-142">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="bb151-143">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bb151-143">Property name</span></span>        | <span data-ttu-id="bb151-144">Тип</span><span class="sxs-lookup"><span data-stu-id="bb151-144">Type</span></span>              | <span data-ttu-id="bb151-145">Описание</span><span class="sxs-lookup"><span data-stu-id="bb151-145">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="bb151-146">id</span><span class="sxs-lookup"><span data-stu-id="bb151-146">id</span></span>                   | <span data-ttu-id="bb151-147">string</span><span class="sxs-lookup"><span data-stu-id="bb151-147">string</span></span>            | <span data-ttu-id="bb151-p103">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb151-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="bb151-150">name</span><span class="sxs-lookup"><span data-stu-id="bb151-150">name</span></span>                 | <span data-ttu-id="bb151-151">string</span><span class="sxs-lookup"><span data-stu-id="bb151-151">string</span></span>            | <span data-ttu-id="bb151-152">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="bb151-152">The name / title of the item.</span></span>
| <span data-ttu-id="bb151-153">createdBy</span><span class="sxs-lookup"><span data-stu-id="bb151-153">createdBy</span></span>            | <span data-ttu-id="bb151-154">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bb151-154">[identitySet][]</span></span>   | <span data-ttu-id="bb151-155">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="bb151-155">Identity of the creator of this item.</span></span> <span data-ttu-id="bb151-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb151-156">Read-only.</span></span>
| <span data-ttu-id="bb151-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb151-157">createdDateTime</span></span>      | <span data-ttu-id="bb151-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb151-158">DateTimeOffset</span></span>    | <span data-ttu-id="bb151-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb151-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="bb151-161">description</span><span class="sxs-lookup"><span data-stu-id="bb151-161">description</span></span>          | <span data-ttu-id="bb151-162">строка</span><span class="sxs-lookup"><span data-stu-id="bb151-162">string</span></span>            | <span data-ttu-id="bb151-163">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="bb151-163">The descriptive text for the item.</span></span>
| <span data-ttu-id="bb151-164">eTag</span><span class="sxs-lookup"><span data-stu-id="bb151-164">eTag</span></span>                 | <span data-ttu-id="bb151-165">string</span><span class="sxs-lookup"><span data-stu-id="bb151-165">string</span></span>            | <span data-ttu-id="bb151-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb151-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="bb151-168">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="bb151-168">lastModifiedBy</span></span>       | <span data-ttu-id="bb151-169">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bb151-169">[identitySet][]</span></span>   | <span data-ttu-id="bb151-170">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="bb151-170">Identity of the last modifier of this item.</span></span> <span data-ttu-id="bb151-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb151-171">Read-only.</span></span>
| <span data-ttu-id="bb151-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb151-172">lastModifiedDateTime</span></span> | <span data-ttu-id="bb151-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb151-173">DateTimeOffset</span></span>    | <span data-ttu-id="bb151-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb151-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="bb151-176">parentReference</span><span class="sxs-lookup"><span data-stu-id="bb151-176">parentReference</span></span>      | <span data-ttu-id="bb151-177">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="bb151-177">[itemReference][]</span></span> | <span data-ttu-id="bb151-p109">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="bb151-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="bb151-180">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="bb151-180">sharepointIds</span></span>        | <span data-ttu-id="bb151-181">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="bb151-181">[sharepointIds][]</span></span> | <span data-ttu-id="bb151-p110">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb151-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="bb151-184">webUrl</span><span class="sxs-lookup"><span data-stu-id="bb151-184">webUrl</span></span>               | <span data-ttu-id="bb151-185">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="bb151-185">string (url)</span></span>      | <span data-ttu-id="bb151-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb151-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="bb151-188">Связи</span><span class="sxs-lookup"><span data-stu-id="bb151-188">Relationships</span></span>

 <span data-ttu-id="bb151-189">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="bb151-189">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="bb151-190">Имя связи</span><span class="sxs-lookup"><span data-stu-id="bb151-190">Relationship name</span></span> | <span data-ttu-id="bb151-191">Тип</span><span class="sxs-lookup"><span data-stu-id="bb151-191">Type</span></span>                           | <span data-ttu-id="bb151-192">Описание</span><span class="sxs-lookup"><span data-stu-id="bb151-192">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="bb151-193">activities</span><span class="sxs-lookup"><span data-stu-id="bb151-193">activities</span></span>        | <span data-ttu-id="bb151-194">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="bb151-194">[itemActivity][] collection</span></span>    | <span data-ttu-id="bb151-195">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="bb151-195">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="bb151-196">Аналитика</span><span class="sxs-lookup"><span data-stu-id="bb151-196">analytics</span></span>         | <span data-ttu-id="bb151-197">[itemAnalytics][] ресурсов</span><span class="sxs-lookup"><span data-stu-id="bb151-197">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="bb151-198">Аналитика о Просмотр действий, выполняемых по этому элементу.</span><span class="sxs-lookup"><span data-stu-id="bb151-198">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="bb151-199">driveItem</span><span class="sxs-lookup"><span data-stu-id="bb151-199">driveItem</span></span>         | <span data-ttu-id="bb151-200">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="bb151-200">[driveItem][]</span></span>                  | <span data-ttu-id="bb151-201">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="bb151-201">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="bb151-202">fields</span><span class="sxs-lookup"><span data-stu-id="bb151-202">fields</span></span>            | <span data-ttu-id="bb151-203">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="bb151-203">[fieldValueSet][]</span></span>              | <span data-ttu-id="bb151-204">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="bb151-204">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="bb151-205">версии</span><span class="sxs-lookup"><span data-stu-id="bb151-205">versions</span></span>          | <span data-ttu-id="bb151-206">[listItemVersion][] коллекции</span><span class="sxs-lookup"><span data-stu-id="bb151-206">[listItemVersion][] collection</span></span> | <span data-ttu-id="bb151-207">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="bb151-207">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[списки]: list.md
[list]: list.md
[listItemVersion]: listitemversion.md.
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
  "suppressions": [
    "Error: /api-reference/beta/resources/listitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
