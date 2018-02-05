---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 0f5afaeff29da6f3a6330975adece44731e014bc
ms.sourcegitcommit: 4bdff5fdaea824c7c1204ec7dd641abc282d32a1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2018
---
# <a name="listitem-resource"></a><span data-ttu-id="785b2-102">Ресурс ListItem</span><span class="sxs-lookup"><span data-stu-id="785b2-102">ListItem resource</span></span>

<span data-ttu-id="785b2-103">Этот ресурс представляет элемент объекта **[list][]** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="785b2-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="785b2-104">Значения столбцов в списке доступны через словарь `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="785b2-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="785b2-105">Задачи для ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="785b2-105">Tasks on a listItem</span></span>

<span data-ttu-id="785b2-106">Ниже перечислены задачи, доступные для ресурсов **listItem**.</span><span class="sxs-lookup"><span data-stu-id="785b2-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="785b2-107">Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="785b2-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="785b2-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="785b2-108">Common task</span></span>                    | <span data-ttu-id="785b2-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="785b2-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="785b2-110">[Получение][]</span><span class="sxs-lookup"><span data-stu-id="785b2-110">[Get][]</span></span>                        | <span data-ttu-id="785b2-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="785b2-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="785b2-112">[Получение значений столбцов][Получение]</span><span class="sxs-lookup"><span data-stu-id="785b2-112">[Get column values][Get]</span></span>       | <span data-ttu-id="785b2-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="785b2-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="785b2-114">[Создание][]</span><span class="sxs-lookup"><span data-stu-id="785b2-114">[Create][]</span></span>                     | <span data-ttu-id="785b2-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="785b2-115">POST /items</span></span>
| <span data-ttu-id="785b2-116">[Удаление][]</span><span class="sxs-lookup"><span data-stu-id="785b2-116">[Delete][]</span></span>                     | <span data-ttu-id="785b2-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="785b2-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="785b2-118">[Обновление][]</span><span class="sxs-lookup"><span data-stu-id="785b2-118">[Update][]</span></span>                     | <span data-ttu-id="785b2-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="785b2-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="785b2-120">[Обновление значений столбцов][Обновление]</span><span class="sxs-lookup"><span data-stu-id="785b2-120">[Update column values][Update]</span></span> | <span data-ttu-id="785b2-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="785b2-121">PATCH /items/{item-id}/fields</span></span>

[Получение]: ../api/listItem_get.md
[Создание]: ../api/listItem_create.md
[Удаление]: ../api/listItem_delete.md
[Обновление]: ../api/listItem_update.md

## <a name="json-representation"></a><span data-ttu-id="785b2-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="785b2-126">JSON representation</span></span>

<span data-ttu-id="785b2-127">Ниже показано представление ресурса **listItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="785b2-127">Here is a JSON representation of a **listItem** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.listItem",
       "keyProperty": "id" } -->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentType" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },

  /* relationships */
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="785b2-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="785b2-128">Properties</span></span>

<span data-ttu-id="785b2-129">Ниже перечислены свойства ресурса **listItem**.</span><span class="sxs-lookup"><span data-stu-id="785b2-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="785b2-130">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="785b2-130">Property name</span></span> | <span data-ttu-id="785b2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="785b2-131">Type</span></span>                | <span data-ttu-id="785b2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="785b2-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="785b2-133">contentType</span><span class="sxs-lookup"><span data-stu-id="785b2-133">contentType</span></span>   | <span data-ttu-id="785b2-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="785b2-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="785b2-135">Тип контента для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="785b2-135">The content type of this list item</span></span>
| <span data-ttu-id="785b2-136">fields</span><span class="sxs-lookup"><span data-stu-id="785b2-136">fields</span></span>        | <span data-ttu-id="785b2-137">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="785b2-137">[fieldValueSet][]</span></span>   | <span data-ttu-id="785b2-138">Значения столбцов, установленные для данного элемента списка.</span><span class="sxs-lookup"><span data-stu-id="785b2-138">The values of the columns set on this list item.</span></span>

<span data-ttu-id="785b2-139">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="785b2-139">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="785b2-140">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="785b2-140">Property name</span></span>        | <span data-ttu-id="785b2-141">Тип</span><span class="sxs-lookup"><span data-stu-id="785b2-141">Type</span></span>             | <span data-ttu-id="785b2-142">Описание</span><span class="sxs-lookup"><span data-stu-id="785b2-142">Description</span></span>
|:---------------------|:-----------------|:-----------------------------------
| <span data-ttu-id="785b2-143">id</span><span class="sxs-lookup"><span data-stu-id="785b2-143">id</span></span>                   | <span data-ttu-id="785b2-144">string</span><span class="sxs-lookup"><span data-stu-id="785b2-144">string</span></span>           | <span data-ttu-id="785b2-p103">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="785b2-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="785b2-147">name</span><span class="sxs-lookup"><span data-stu-id="785b2-147">name</span></span>                 | <span data-ttu-id="785b2-148">string</span><span class="sxs-lookup"><span data-stu-id="785b2-148">string</span></span>           | <span data-ttu-id="785b2-149">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="785b2-149">The name / title of the item.</span></span>
| <span data-ttu-id="785b2-150">createdBy</span><span class="sxs-lookup"><span data-stu-id="785b2-150">createdBy</span></span>            | <span data-ttu-id="785b2-151">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="785b2-151">[identitySet][]</span></span>  | <span data-ttu-id="785b2-152">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="785b2-152">Identity of the creator of this item.</span></span> <span data-ttu-id="785b2-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="785b2-153">Read-only.</span></span>
| <span data-ttu-id="785b2-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="785b2-154">createdDateTime</span></span>      | <span data-ttu-id="785b2-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="785b2-155">DateTimeOffset</span></span>   | <span data-ttu-id="785b2-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="785b2-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="785b2-158">description</span><span class="sxs-lookup"><span data-stu-id="785b2-158">description</span></span>          | <span data-ttu-id="785b2-159">строка</span><span class="sxs-lookup"><span data-stu-id="785b2-159">string</span></span>           | <span data-ttu-id="785b2-160">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="785b2-160">The descriptive text for the item.</span></span>
| <span data-ttu-id="785b2-161">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="785b2-161">lastModifiedBy</span></span>       | <span data-ttu-id="785b2-162">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="785b2-162">[identitySet][]</span></span>  | <span data-ttu-id="785b2-163">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="785b2-163">Identity of the last modifier of this item.</span></span> <span data-ttu-id="785b2-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="785b2-164">Read-only.</span></span>
| <span data-ttu-id="785b2-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="785b2-165">lastModifiedDateTime</span></span> | <span data-ttu-id="785b2-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="785b2-166">DateTimeOffset</span></span>   | <span data-ttu-id="785b2-p107">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="785b2-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="785b2-169">webUrl</span><span class="sxs-lookup"><span data-stu-id="785b2-169">webUrl</span></span>               | <span data-ttu-id="785b2-170">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="785b2-170">string (url)</span></span>     | <span data-ttu-id="785b2-p108">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="785b2-p108">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="785b2-173">Связи</span><span class="sxs-lookup"><span data-stu-id="785b2-173">Relationships</span></span>

 <span data-ttu-id="785b2-174">Ниже перечислены связи ресурса **listItem** с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="785b2-174">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="785b2-175">Имя связи</span><span class="sxs-lookup"><span data-stu-id="785b2-175">Relationship name</span></span> | <span data-ttu-id="785b2-176">Тип</span><span class="sxs-lookup"><span data-stu-id="785b2-176">Type</span></span>                        | <span data-ttu-id="785b2-177">Описание</span><span class="sxs-lookup"><span data-stu-id="785b2-177">Description</span></span>
|:------------------|:----------------------------|:-------------------------------
| <span data-ttu-id="785b2-178">driveItem</span><span class="sxs-lookup"><span data-stu-id="785b2-178">driveItem</span></span>         | <span data-ttu-id="785b2-179">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="785b2-179">[driveItem][]</span></span>               | <span data-ttu-id="785b2-180">Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="785b2-180">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[list]: list.md

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
