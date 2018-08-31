---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 13ddb00d90880570361c7dcbe198c7c90e044957
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264401"
---
# <a name="listitem-resource"></a><span data-ttu-id="1e4de-102">Ресурс ListItem</span><span class="sxs-lookup"><span data-stu-id="1e4de-102">ListItem resource</span></span>

<span data-ttu-id="1e4de-103">Этот ресурс представляет элемент объекта **[list][]** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1e4de-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="1e4de-104">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="1e4de-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="1e4de-105">Задачи для ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="1e4de-105">Tasks on a listItem</span></span>

<span data-ttu-id="1e4de-106">Ниже перечислены задачи, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="1e4de-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="1e4de-107">Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="1e4de-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="1e4de-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="1e4de-108">Common task</span></span>                    | <span data-ttu-id="1e4de-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="1e4de-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="1e4de-110">[Получение][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-110">[Get][]</span></span>                        | <span data-ttu-id="1e4de-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="1e4de-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="1e4de-112">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="1e4de-112">[Get column values][Get]</span></span>       | <span data-ttu-id="1e4de-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="1e4de-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="1e4de-114">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-114">[Create][]</span></span>                     | <span data-ttu-id="1e4de-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="1e4de-115">POST /items</span></span>
| <span data-ttu-id="1e4de-116">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-116">[Delete][]</span></span>                     | <span data-ttu-id="1e4de-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="1e4de-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="1e4de-118">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-118">[Update][]</span></span>                     | <span data-ttu-id="1e4de-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="1e4de-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="1e4de-120">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="1e4de-120">[Update column values][Update]</span></span> | <span data-ttu-id="1e4de-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="1e4de-121">PATCH /items/{item-id}/fields</span></span>

[Получение]: ../api/listItem_get.md
[Get]: ../api/listItem_get.md
[Создание]: ../api/listItem_create.md
[Create]: ../api/listItem_create.md
[Удаление]: ../api/listItem_delete.md
[Delete]: ../api/listItem_delete.md
[Обновление]: ../api/listItem_update.md
[Update]: ../api/listItem_update.md

## <a name="json-representation"></a><span data-ttu-id="1e4de-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1e4de-126">JSON representation</span></span>

<span data-ttu-id="1e4de-127">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e4de-127">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="1e4de-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e4de-128">Properties</span></span>

<span data-ttu-id="1e4de-129">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="1e4de-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="1e4de-130">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1e4de-130">Property name</span></span> | <span data-ttu-id="1e4de-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1e4de-131">Type</span></span>                | <span data-ttu-id="1e4de-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1e4de-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="1e4de-133">contentType</span><span class="sxs-lookup"><span data-stu-id="1e4de-133">contentType</span></span>   | <span data-ttu-id="1e4de-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="1e4de-135">Тип содержимого для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="1e4de-135">The content type of this list item</span></span>

<span data-ttu-id="1e4de-136">Следующие свойства наследуются от **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="1e4de-136">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="1e4de-137">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1e4de-137">Property name</span></span>        | <span data-ttu-id="1e4de-138">Тип</span><span class="sxs-lookup"><span data-stu-id="1e4de-138">Type</span></span>              | <span data-ttu-id="1e4de-139">Описание</span><span class="sxs-lookup"><span data-stu-id="1e4de-139">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="1e4de-140">id</span><span class="sxs-lookup"><span data-stu-id="1e4de-140">id</span></span>                   | <span data-ttu-id="1e4de-141">string (строка)</span><span class="sxs-lookup"><span data-stu-id="1e4de-141">string</span></span>            | <span data-ttu-id="1e4de-p103">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e4de-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="1e4de-144">name</span><span class="sxs-lookup"><span data-stu-id="1e4de-144">name</span></span>                 | <span data-ttu-id="1e4de-145">string (строка)</span><span class="sxs-lookup"><span data-stu-id="1e4de-145">string</span></span>            | <span data-ttu-id="1e4de-146">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="1e4de-146">The name / title of the item.</span></span>
| <span data-ttu-id="1e4de-147">createdBy</span><span class="sxs-lookup"><span data-stu-id="1e4de-147">createdBy</span></span>            | <span data-ttu-id="1e4de-148">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-148">[identitySet][]</span></span>   | <span data-ttu-id="1e4de-149">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="1e4de-149">Identity of the creator of this item.</span></span> <span data-ttu-id="1e4de-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e4de-150">Read-only.</span></span>
| <span data-ttu-id="1e4de-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e4de-151">createdDateTime</span></span>      | <span data-ttu-id="1e4de-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e4de-152">DateTimeOffset</span></span>    | <span data-ttu-id="1e4de-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e4de-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="1e4de-155">description</span><span class="sxs-lookup"><span data-stu-id="1e4de-155">description</span></span>          | <span data-ttu-id="1e4de-156">string (строка)</span><span class="sxs-lookup"><span data-stu-id="1e4de-156">string</span></span>            | <span data-ttu-id="1e4de-157">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="1e4de-157">The descriptive text for the item.</span></span>
| <span data-ttu-id="1e4de-158">eTag</span><span class="sxs-lookup"><span data-stu-id="1e4de-158">eTag</span></span>                 | <span data-ttu-id="1e4de-159">string (строка)</span><span class="sxs-lookup"><span data-stu-id="1e4de-159">string</span></span>            | <span data-ttu-id="1e4de-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e4de-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="1e4de-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1e4de-162">lastModifiedBy</span></span>       | <span data-ttu-id="1e4de-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-163">[identitySet][]</span></span>   | <span data-ttu-id="1e4de-164">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="1e4de-164">Identity of the last modifier of this item.</span></span> <span data-ttu-id="1e4de-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e4de-165">Read-only.</span></span>
| <span data-ttu-id="1e4de-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e4de-166">lastModifiedDateTime</span></span> | <span data-ttu-id="1e4de-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e4de-167">DateTimeOffset</span></span>    | <span data-ttu-id="1e4de-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e4de-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="1e4de-170">parentReference</span><span class="sxs-lookup"><span data-stu-id="1e4de-170">parentReference</span></span>      | <span data-ttu-id="1e4de-171">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-171">[itemReference][]</span></span> | <span data-ttu-id="1e4de-p109">Сведения о родительском элементе, если у элемента таковой имеется. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="1e4de-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="1e4de-174">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="1e4de-174">sharepointIds</span></span>        | <span data-ttu-id="1e4de-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-175">[sharepointIds][]</span></span> | <span data-ttu-id="1e4de-p110">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e4de-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="1e4de-178">webUrl</span><span class="sxs-lookup"><span data-stu-id="1e4de-178">webUrl</span></span>               | <span data-ttu-id="1e4de-179">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="1e4de-179">string (url)</span></span>      | <span data-ttu-id="1e4de-p111">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e4de-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="1e4de-182">Связи</span><span class="sxs-lookup"><span data-stu-id="1e4de-182">Relationships</span></span>

 <span data-ttu-id="1e4de-183">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="1e4de-183">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="1e4de-184">Имя связи</span><span class="sxs-lookup"><span data-stu-id="1e4de-184">Relationship name</span></span> | <span data-ttu-id="1e4de-185">Тип</span><span class="sxs-lookup"><span data-stu-id="1e4de-185">Type</span></span>                           | <span data-ttu-id="1e4de-186">Описание</span><span class="sxs-lookup"><span data-stu-id="1e4de-186">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="1e4de-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="1e4de-187">driveItem</span></span>         | <span data-ttu-id="1e4de-188">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-188">[driveItem][]</span></span>                  | <span data-ttu-id="1e4de-189">Для библиотек документов связь **driveItem** предоставляет listItem как **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="1e4de-189">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="1e4de-190">fields</span><span class="sxs-lookup"><span data-stu-id="1e4de-190">fields</span></span>            | <span data-ttu-id="1e4de-191">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-191">[fieldValueSet][]</span></span>              | <span data-ttu-id="1e4de-192">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="1e4de-192">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="1e4de-193">versions</span><span class="sxs-lookup"><span data-stu-id="1e4de-193">versions</span></span>          | <span data-ttu-id="1e4de-194">Коллекция [listItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="1e4de-194">[listItemVersion][] collection</span></span> | <span data-ttu-id="1e4de-195">Список предыдущих версий элемента списка.</span><span class="sxs-lookup"><span data-stu-id="1e4de-195">The list of previous versions of the list item.</span></span>

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listItemVersion.md
[sharepointIds]: sharepointIds.md

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
