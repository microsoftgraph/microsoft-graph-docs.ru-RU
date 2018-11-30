---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 18ba74fd677c83da5f8bfe5d13303f7b18ed43f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076517"
---
# <a name="listitem-resource"></a><span data-ttu-id="a4e90-102">Ресурс ListItem</span><span class="sxs-lookup"><span data-stu-id="a4e90-102">ListItem resource</span></span>

> <span data-ttu-id="a4e90-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a4e90-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4e90-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4e90-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4e90-105">Этот ресурс представляет элемент объекта **[list][]** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a4e90-105">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="a4e90-106">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="a4e90-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="a4e90-107">Задачи для ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="a4e90-107">Tasks on a listItem</span></span>

<span data-ttu-id="a4e90-108">Ниже перечислены задачи, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="a4e90-108">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="a4e90-109">Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="a4e90-109">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="a4e90-110">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="a4e90-110">Common task</span></span>                    | <span data-ttu-id="a4e90-111">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="a4e90-111">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="a4e90-112">[Получение][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-112">[Get][]</span></span>                        | <span data-ttu-id="a4e90-113">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a4e90-113">GET /items/{item-id}</span></span>
| <span data-ttu-id="a4e90-114">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="a4e90-114">[Get column values][Get]</span></span>       | <span data-ttu-id="a4e90-115">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="a4e90-115">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="a4e90-116">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-116">[Get analytics][]</span></span>              | <span data-ttu-id="a4e90-117">GET /items/ {идентификатор элемента} / аналитики</span><span class="sxs-lookup"><span data-stu-id="a4e90-117">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="a4e90-118">[Получение действий по интервал][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-118">[Get activities by interval][]</span></span> | <span data-ttu-id="a4e90-119">GET /items/ {идентификатор элемента} / getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="a4e90-119">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="a4e90-120">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-120">[Create][]</span></span>                     | <span data-ttu-id="a4e90-121">POST /items</span><span class="sxs-lookup"><span data-stu-id="a4e90-121">POST /items</span></span>
| <span data-ttu-id="a4e90-122">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-122">[Delete][]</span></span>                     | <span data-ttu-id="a4e90-123">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a4e90-123">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="a4e90-124">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-124">[Update][]</span></span>                     | <span data-ttu-id="a4e90-125">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a4e90-125">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="a4e90-126">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="a4e90-126">[Update column values][Update]</span></span> | <span data-ttu-id="a4e90-127">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="a4e90-127">PATCH /items/{item-id}/fields</span></span>

[Получение]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Получение действий по интервал]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Обновление]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="a4e90-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a4e90-134">JSON representation</span></span>

<span data-ttu-id="a4e90-135">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4e90-135">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a4e90-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4e90-136">Properties</span></span>

<span data-ttu-id="a4e90-137">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="a4e90-137">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="a4e90-138">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a4e90-138">Property name</span></span> | <span data-ttu-id="a4e90-139">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e90-139">Type</span></span>                | <span data-ttu-id="a4e90-140">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e90-140">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="a4e90-141">contentType</span><span class="sxs-lookup"><span data-stu-id="a4e90-141">contentType</span></span>   | <span data-ttu-id="a4e90-142">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-142">[contentTypeInfo][]</span></span> | <span data-ttu-id="a4e90-143">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="a4e90-143">The content type of this list item</span></span>

<span data-ttu-id="a4e90-144">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="a4e90-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="a4e90-145">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a4e90-145">Property name</span></span>        | <span data-ttu-id="a4e90-146">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e90-146">Type</span></span>              | <span data-ttu-id="a4e90-147">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e90-147">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="a4e90-148">id</span><span class="sxs-lookup"><span data-stu-id="a4e90-148">id</span></span>                   | <span data-ttu-id="a4e90-149">строка</span><span class="sxs-lookup"><span data-stu-id="a4e90-149">string</span></span>            | <span data-ttu-id="a4e90-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e90-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="a4e90-152">name</span><span class="sxs-lookup"><span data-stu-id="a4e90-152">name</span></span>                 | <span data-ttu-id="a4e90-153">строка</span><span class="sxs-lookup"><span data-stu-id="a4e90-153">string</span></span>            | <span data-ttu-id="a4e90-154">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="a4e90-154">The name / title of the item.</span></span>
| <span data-ttu-id="a4e90-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="a4e90-155">createdBy</span></span>            | <span data-ttu-id="a4e90-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-156">[identitySet][]</span></span>   | <span data-ttu-id="a4e90-157">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="a4e90-157">Identity of the creator of this item.</span></span> <span data-ttu-id="a4e90-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e90-158">Read-only.</span></span>
| <span data-ttu-id="a4e90-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4e90-159">createdDateTime</span></span>      | <span data-ttu-id="a4e90-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4e90-160">DateTimeOffset</span></span>    | <span data-ttu-id="a4e90-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e90-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="a4e90-163">description</span><span class="sxs-lookup"><span data-stu-id="a4e90-163">description</span></span>          | <span data-ttu-id="a4e90-164">строка</span><span class="sxs-lookup"><span data-stu-id="a4e90-164">string</span></span>            | <span data-ttu-id="a4e90-165">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="a4e90-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="a4e90-166">eTag</span><span class="sxs-lookup"><span data-stu-id="a4e90-166">eTag</span></span>                 | <span data-ttu-id="a4e90-167">string</span><span class="sxs-lookup"><span data-stu-id="a4e90-167">string</span></span>            | <span data-ttu-id="a4e90-p107">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e90-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="a4e90-170">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a4e90-170">lastModifiedBy</span></span>       | <span data-ttu-id="a4e90-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-171">[identitySet][]</span></span>   | <span data-ttu-id="a4e90-172">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="a4e90-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="a4e90-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e90-173">Read-only.</span></span>
| <span data-ttu-id="a4e90-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4e90-174">lastModifiedDateTime</span></span> | <span data-ttu-id="a4e90-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4e90-175">DateTimeOffset</span></span>    | <span data-ttu-id="a4e90-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e90-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="a4e90-178">parentReference</span><span class="sxs-lookup"><span data-stu-id="a4e90-178">parentReference</span></span>      | <span data-ttu-id="a4e90-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-179">[itemReference][]</span></span> | <span data-ttu-id="a4e90-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="a4e90-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="a4e90-182">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="a4e90-182">sharepointIds</span></span>        | <span data-ttu-id="a4e90-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-183">[sharepointIds][]</span></span> | <span data-ttu-id="a4e90-p111">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e90-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="a4e90-186">webUrl</span><span class="sxs-lookup"><span data-stu-id="a4e90-186">webUrl</span></span>               | <span data-ttu-id="a4e90-187">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="a4e90-187">string (url)</span></span>      | <span data-ttu-id="a4e90-p112">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e90-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="a4e90-190">Связи</span><span class="sxs-lookup"><span data-stu-id="a4e90-190">Relationships</span></span>

 <span data-ttu-id="a4e90-191">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="a4e90-191">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="a4e90-192">Имя связи</span><span class="sxs-lookup"><span data-stu-id="a4e90-192">Relationship name</span></span> | <span data-ttu-id="a4e90-193">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e90-193">Type</span></span>                           | <span data-ttu-id="a4e90-194">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e90-194">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="a4e90-195">activities</span><span class="sxs-lookup"><span data-stu-id="a4e90-195">activities</span></span>        | <span data-ttu-id="a4e90-196">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-196">[itemActivity][] collection</span></span>    | <span data-ttu-id="a4e90-197">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="a4e90-197">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="a4e90-198">Аналитика</span><span class="sxs-lookup"><span data-stu-id="a4e90-198">analytics</span></span>         | <span data-ttu-id="a4e90-199">[itemAnalytics][] ресурсов</span><span class="sxs-lookup"><span data-stu-id="a4e90-199">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="a4e90-200">Аналитика о Просмотр действий, выполняемых по этому элементу.</span><span class="sxs-lookup"><span data-stu-id="a4e90-200">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="a4e90-201">driveItem</span><span class="sxs-lookup"><span data-stu-id="a4e90-201">driveItem</span></span>         | <span data-ttu-id="a4e90-202">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-202">[driveItem][]</span></span>                  | <span data-ttu-id="a4e90-203">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="a4e90-203">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="a4e90-204">fields</span><span class="sxs-lookup"><span data-stu-id="a4e90-204">fields</span></span>            | <span data-ttu-id="a4e90-205">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="a4e90-205">[fieldValueSet][]</span></span>              | <span data-ttu-id="a4e90-206">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="a4e90-206">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="a4e90-207">версии</span><span class="sxs-lookup"><span data-stu-id="a4e90-207">versions</span></span>          | <span data-ttu-id="a4e90-208">[listItemVersion][] коллекции</span><span class="sxs-lookup"><span data-stu-id="a4e90-208">[listItemVersion][] collection</span></span> | <span data-ttu-id="a4e90-209">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="a4e90-209">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md.
[sharepointIds]: sharepointids.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
