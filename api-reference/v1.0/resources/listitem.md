---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListItem
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: ba4b910f6d86caee23ce191b225d040ef023b4e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519950"
---
# <a name="listitem-resource"></a><span data-ttu-id="dcfc5-102">Ресурс ListItem</span><span class="sxs-lookup"><span data-stu-id="dcfc5-102">ListItem resource</span></span>

<span data-ttu-id="dcfc5-103">Этот ресурс представляет элемент объекта **[list][]** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="dcfc5-104">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="dcfc5-105">Задачи для ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="dcfc5-105">Tasks on a listItem</span></span>

<span data-ttu-id="dcfc5-106">Ниже перечислены задачи, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="dcfc5-107">Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="dcfc5-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="dcfc5-108">Common task</span></span>                    | <span data-ttu-id="dcfc5-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="dcfc5-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="dcfc5-110">[Получение][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-110">[Get][]</span></span>                        | <span data-ttu-id="dcfc5-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="dcfc5-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="dcfc5-112">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-112">[Get column values][Get]</span></span>       | <span data-ttu-id="dcfc5-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="dcfc5-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="dcfc5-114">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-114">[Create][]</span></span>                     | <span data-ttu-id="dcfc5-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="dcfc5-115">POST /items</span></span>
| <span data-ttu-id="dcfc5-116">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-116">[Delete][]</span></span>                     | <span data-ttu-id="dcfc5-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="dcfc5-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="dcfc5-118">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-118">[Update][]</span></span>                     | <span data-ttu-id="dcfc5-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="dcfc5-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="dcfc5-120">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-120">[Update column values][Update]</span></span> | <span data-ttu-id="dcfc5-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="dcfc5-121">PATCH /items/{item-id}/fields</span></span>

[Получение]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[Создание]: ../api/listitem-create.md
[Create]: ../api/listitem-create.md
[Удаление]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[Обновление]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="dcfc5-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dcfc5-126">JSON representation</span></span>

<span data-ttu-id="dcfc5-127">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-127">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dcfc5-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="dcfc5-128">Properties</span></span>

<span data-ttu-id="dcfc5-129">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="dcfc5-130">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dcfc5-130">Property name</span></span> | <span data-ttu-id="dcfc5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dcfc5-131">Type</span></span>                | <span data-ttu-id="dcfc5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dcfc5-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="dcfc5-133">contentType</span><span class="sxs-lookup"><span data-stu-id="dcfc5-133">contentType</span></span>   | <span data-ttu-id="dcfc5-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="dcfc5-135">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-135">The content type of this list item</span></span>

<span data-ttu-id="dcfc5-136">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-136">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="dcfc5-137">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dcfc5-137">Property name</span></span>        | <span data-ttu-id="dcfc5-138">Тип</span><span class="sxs-lookup"><span data-stu-id="dcfc5-138">Type</span></span>              | <span data-ttu-id="dcfc5-139">Описание</span><span class="sxs-lookup"><span data-stu-id="dcfc5-139">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="dcfc5-140">id</span><span class="sxs-lookup"><span data-stu-id="dcfc5-140">id</span></span>                   | <span data-ttu-id="dcfc5-141">string</span><span class="sxs-lookup"><span data-stu-id="dcfc5-141">string</span></span>            | <span data-ttu-id="dcfc5-p103">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="dcfc5-144">name</span><span class="sxs-lookup"><span data-stu-id="dcfc5-144">name</span></span>                 | <span data-ttu-id="dcfc5-145">string</span><span class="sxs-lookup"><span data-stu-id="dcfc5-145">string</span></span>            | <span data-ttu-id="dcfc5-146">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-146">The name / title of the item.</span></span>
| <span data-ttu-id="dcfc5-147">createdBy</span><span class="sxs-lookup"><span data-stu-id="dcfc5-147">createdBy</span></span>            | <span data-ttu-id="dcfc5-148">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-148">[identitySet][]</span></span>   | <span data-ttu-id="dcfc5-149">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-149">Identity of the creator of this item.</span></span> <span data-ttu-id="dcfc5-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-150">Read-only.</span></span>
| <span data-ttu-id="dcfc5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dcfc5-151">createdDateTime</span></span>      | <span data-ttu-id="dcfc5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcfc5-152">DateTimeOffset</span></span>    | <span data-ttu-id="dcfc5-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="dcfc5-155">description</span><span class="sxs-lookup"><span data-stu-id="dcfc5-155">description</span></span>          | <span data-ttu-id="dcfc5-156">строка</span><span class="sxs-lookup"><span data-stu-id="dcfc5-156">string</span></span>            | <span data-ttu-id="dcfc5-157">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-157">The descriptive text for the item.</span></span>
| <span data-ttu-id="dcfc5-158">eTag</span><span class="sxs-lookup"><span data-stu-id="dcfc5-158">eTag</span></span>                 | <span data-ttu-id="dcfc5-159">string</span><span class="sxs-lookup"><span data-stu-id="dcfc5-159">string</span></span>            | <span data-ttu-id="dcfc5-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="dcfc5-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="dcfc5-162">lastModifiedBy</span></span>       | <span data-ttu-id="dcfc5-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-163">[identitySet][]</span></span>   | <span data-ttu-id="dcfc5-164">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-164">Identity of the last modifier of this item.</span></span> <span data-ttu-id="dcfc5-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-165">Read-only.</span></span>
| <span data-ttu-id="dcfc5-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dcfc5-166">lastModifiedDateTime</span></span> | <span data-ttu-id="dcfc5-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcfc5-167">DateTimeOffset</span></span>    | <span data-ttu-id="dcfc5-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="dcfc5-170">parentReference</span><span class="sxs-lookup"><span data-stu-id="dcfc5-170">parentReference</span></span>      | <span data-ttu-id="dcfc5-171">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-171">[itemReference][]</span></span> | <span data-ttu-id="dcfc5-p109">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="dcfc5-174">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="dcfc5-174">sharepointIds</span></span>        | <span data-ttu-id="dcfc5-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-175">[sharepointIds][]</span></span> | <span data-ttu-id="dcfc5-p110">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="dcfc5-178">webUrl</span><span class="sxs-lookup"><span data-stu-id="dcfc5-178">webUrl</span></span>               | <span data-ttu-id="dcfc5-179">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="dcfc5-179">string (url)</span></span>      | <span data-ttu-id="dcfc5-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="dcfc5-182">Связи</span><span class="sxs-lookup"><span data-stu-id="dcfc5-182">Relationships</span></span>

 <span data-ttu-id="dcfc5-183">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-183">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="dcfc5-184">Имя связи</span><span class="sxs-lookup"><span data-stu-id="dcfc5-184">Relationship name</span></span> | <span data-ttu-id="dcfc5-185">Тип</span><span class="sxs-lookup"><span data-stu-id="dcfc5-185">Type</span></span>                           | <span data-ttu-id="dcfc5-186">Описание</span><span class="sxs-lookup"><span data-stu-id="dcfc5-186">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="dcfc5-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="dcfc5-187">driveItem</span></span>         | <span data-ttu-id="dcfc5-188">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-188">[driveItem][]</span></span>                  | <span data-ttu-id="dcfc5-189">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="dcfc5-189">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="dcfc5-190">fields</span><span class="sxs-lookup"><span data-stu-id="dcfc5-190">fields</span></span>            | <span data-ttu-id="dcfc5-191">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-191">[fieldValueSet][]</span></span>              | <span data-ttu-id="dcfc5-192">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-192">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="dcfc5-193">versions</span><span class="sxs-lookup"><span data-stu-id="dcfc5-193">versions</span></span>          | <span data-ttu-id="dcfc5-194">Коллекция [listItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="dcfc5-194">[listItemVersion][] collection</span></span> | <span data-ttu-id="dcfc5-195">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="dcfc5-195">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
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
