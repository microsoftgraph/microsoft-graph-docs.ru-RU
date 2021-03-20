---
author: JeremyKelley
description: Вот представление JSON ресурса columnDefinition.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: cddab6ee01cea34902ee892e593e0e81b3cde8af
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961302"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="4a64b-103">тип ресурса columnDefinition</span><span class="sxs-lookup"><span data-stu-id="4a64b-103">columnDefinition resource type</span></span>

<span data-ttu-id="4a64b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a64b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a64b-105">Представляет столбец на [сайте,][] [списке или][] [contentType.][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-105">Represents a column in a [site][], [list][] or [contentType][].</span></span>

## <a name="methods"></a><span data-ttu-id="4a64b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4a64b-106">Methods</span></span>
|<span data-ttu-id="4a64b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4a64b-107">Method</span></span>|<span data-ttu-id="4a64b-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="4a64b-108">Return type</span></span>|<span data-ttu-id="4a64b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4a64b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4a64b-110">Список столбцов на сайте</span><span class="sxs-lookup"><span data-stu-id="4a64b-110">List columns in a site</span></span>](../api/site-list-columns.md)|<span data-ttu-id="4a64b-111">[коллекция columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a64b-111">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="4a64b-112">Получите список объектов [columnDefinition](../resources/columndefinition.md) и их свойств на [сайте.](../resources/site.md)</span><span class="sxs-lookup"><span data-stu-id="4a64b-112">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="4a64b-113">Список столбцов в списке</span><span class="sxs-lookup"><span data-stu-id="4a64b-113">List columns in a list</span></span>](../api/list-list-columns.md)|<span data-ttu-id="4a64b-114">[коллекция columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a64b-114">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="4a64b-115">Получите список объектов [columnDefinition](../resources/columndefinition.md) и их свойств в [списке.](../resources/list.md)</span><span class="sxs-lookup"><span data-stu-id="4a64b-115">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="4a64b-116">Список столбцов в типе контента</span><span class="sxs-lookup"><span data-stu-id="4a64b-116">List columns in a content type</span></span>](../api/contenttype-list-columns.md)|<span data-ttu-id="4a64b-117">[коллекция columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a64b-117">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="4a64b-118">Получите список объектов [columnDefinition](../resources/columndefinition.md) и их свойств в [типе контента.](../resources/contenttype.md)</span><span class="sxs-lookup"><span data-stu-id="4a64b-118">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="4a64b-119">Создание columnDefinition для сайта</span><span class="sxs-lookup"><span data-stu-id="4a64b-119">Create columnDefinition for a site</span></span>](../api/site-post-columns.md)|[<span data-ttu-id="4a64b-120">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="4a64b-120">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="4a64b-121">Создание нового [объекта columnDefinition](../resources/columndefinition.md) на [сайте.](../resources/site.md)</span><span class="sxs-lookup"><span data-stu-id="4a64b-121">Create a new [columnDefinition](../resources/columndefinition.md) object in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="4a64b-122">Создание columnDefinition для списка</span><span class="sxs-lookup"><span data-stu-id="4a64b-122">Create columnDefinition for a list</span></span>](../api/list-post-columns.md)|[<span data-ttu-id="4a64b-123">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="4a64b-123">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="4a64b-124">Создайте новый [объект columnDefinition](../resources/columndefinition.md) в [списке](../resources/list.md).</span><span class="sxs-lookup"><span data-stu-id="4a64b-124">Create a new [columnDefinition](../resources/columndefinition.md) object in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="4a64b-125">Создание columnDefinition для типа контента</span><span class="sxs-lookup"><span data-stu-id="4a64b-125">Create columnDefinition for a content type</span></span>](../api/contenttype-post-columns.md)|[<span data-ttu-id="4a64b-126">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="4a64b-126">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="4a64b-127">Создание нового [объекта columnDefinition](../resources/columndefinition.md) в [типе контента.](../resources/contenttype.md)</span><span class="sxs-lookup"><span data-stu-id="4a64b-127">Create a new [columnDefinition](../resources/columndefinition.md) object in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="4a64b-128">Получить columnDefinition</span><span class="sxs-lookup"><span data-stu-id="4a64b-128">Get columnDefinition</span></span>](../api/columndefinition-get.md)|[<span data-ttu-id="4a64b-129">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="4a64b-129">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="4a64b-130">Ознакомьтесь с свойствами и отношениями объекта [columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a64b-130">Read the properties and relationships of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="4a64b-131">Обновление столбцаDefinition</span><span class="sxs-lookup"><span data-stu-id="4a64b-131">Update columnDefinition</span></span>](../api/columndefinition-update.md)|[<span data-ttu-id="4a64b-132">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="4a64b-132">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="4a64b-133">Обновление свойств объекта [columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a64b-133">Update the properties of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="4a64b-134">Удаление columnDefinition</span><span class="sxs-lookup"><span data-stu-id="4a64b-134">Delete columnDefinition</span></span>](../api/columndefinition-delete.md)|<span data-ttu-id="4a64b-135">Нет</span><span class="sxs-lookup"><span data-stu-id="4a64b-135">None</span></span>|<span data-ttu-id="4a64b-136">Удаляет объект [columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a64b-136">Deletes a [columnDefinition](../resources/columndefinition.md) object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a64b-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a64b-137">JSON representation</span></span>

<span data-ttu-id="4a64b-138">Вот представление JSON ресурса columnDefinition.</span><span class="sxs-lookup"><span data-stu-id="4a64b-138">Here is a JSON representation of a columnDefinition resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": true,
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" },
  "isDeletable" : false,
  "propagateChanges": false,
  "isReorderable": false,
  "isSealed": false,
  "validation": { "@odata.type": "microsoft.graph.columnValidation" },
  "hyperlinkOrPicture": { "@odata.type": "microsoft.graph.hyperlinkOrPictureColumn" },
  "term": { "@odata.type": "microsoft.graph.termColumn" },
  "sourceContentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "thumbnail": { "@odata.type": "microsoft.graph.thumbnailColumn" },
  "type": { "@odata.type": "microsoft.graph.columnTypes" },
  "contentApprovalStatus": { "@odata.type": "microsoft.graph.contentApprovalStatusColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="4a64b-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a64b-139">Properties</span></span>

<span data-ttu-id="4a64b-140">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="4a64b-140">Columns can hold data of various types.</span></span>
<span data-ttu-id="4a64b-141">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="4a64b-141">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="4a64b-142">Свойства типа (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) являются взаимоисключающими : столбец может иметь только один из указанных.</span><span class="sxs-lookup"><span data-stu-id="4a64b-142">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="4a64b-143">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4a64b-143">Property name</span></span>           | <span data-ttu-id="4a64b-144">Тип</span><span class="sxs-lookup"><span data-stu-id="4a64b-144">Type</span></span>    | <span data-ttu-id="4a64b-145">Описание</span><span class="sxs-lookup"><span data-stu-id="4a64b-145">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="4a64b-146">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="4a64b-146">**columnGroup**</span></span>         | <span data-ttu-id="4a64b-147">строка</span><span class="sxs-lookup"><span data-stu-id="4a64b-147">string</span></span>  | <span data-ttu-id="4a64b-148">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="4a64b-148">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="4a64b-149">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="4a64b-149">Helps organize related columns.</span></span>
| <span data-ttu-id="4a64b-150">**description**</span><span class="sxs-lookup"><span data-stu-id="4a64b-150">**description**</span></span>         | <span data-ttu-id="4a64b-151">string</span><span class="sxs-lookup"><span data-stu-id="4a64b-151">string</span></span>  | <span data-ttu-id="4a64b-152">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="4a64b-152">The user-facing description of the column.</span></span>
| <span data-ttu-id="4a64b-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="4a64b-153">**displayName**</span></span>         | <span data-ttu-id="4a64b-154">string</span><span class="sxs-lookup"><span data-stu-id="4a64b-154">string</span></span>  | <span data-ttu-id="4a64b-155">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="4a64b-155">The user-facing name of the column.</span></span>
| <span data-ttu-id="4a64b-156">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="4a64b-156">**enforceUniqueValues**</span></span> | <span data-ttu-id="4a64b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64b-157">Boolean</span></span> | <span data-ttu-id="4a64b-158">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="4a64b-158">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="4a64b-159">**hidden**</span><span class="sxs-lookup"><span data-stu-id="4a64b-159">**hidden**</span></span>              | <span data-ttu-id="4a64b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64b-160">Boolean</span></span> | <span data-ttu-id="4a64b-161">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="4a64b-161">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="4a64b-162">**id**</span><span class="sxs-lookup"><span data-stu-id="4a64b-162">**id**</span></span>                  | <span data-ttu-id="4a64b-163">string</span><span class="sxs-lookup"><span data-stu-id="4a64b-163">string</span></span>  | <span data-ttu-id="4a64b-164">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="4a64b-164">The unique identifier for the column.</span></span>
| <span data-ttu-id="4a64b-165">**indexed**</span><span class="sxs-lookup"><span data-stu-id="4a64b-165">**indexed**</span></span>             | <span data-ttu-id="4a64b-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64b-166">Boolean</span></span> | <span data-ttu-id="4a64b-167">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="4a64b-167">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="4a64b-168">**name**</span><span class="sxs-lookup"><span data-stu-id="4a64b-168">**name**</span></span>                | <span data-ttu-id="4a64b-169">string</span><span class="sxs-lookup"><span data-stu-id="4a64b-169">string</span></span>  | <span data-ttu-id="4a64b-170">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="4a64b-170">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="4a64b-171">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="4a64b-171">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="4a64b-172">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="4a64b-172">**readOnly**</span></span>            | <span data-ttu-id="4a64b-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64b-173">Boolean</span></span>    | <span data-ttu-id="4a64b-174">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="4a64b-174">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="4a64b-175">**required**</span><span class="sxs-lookup"><span data-stu-id="4a64b-175">**required**</span></span>            | <span data-ttu-id="4a64b-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64b-176">Boolean</span></span> | <span data-ttu-id="4a64b-177">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="4a64b-177">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="4a64b-178">**boolean**</span><span class="sxs-lookup"><span data-stu-id="4a64b-178">**boolean**</span></span>       | <span data-ttu-id="4a64b-179">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-179">[booleanColumn][]</span></span>       | <span data-ttu-id="4a64b-180">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="4a64b-180">This column stores boolean values.</span></span>
| <span data-ttu-id="4a64b-181">**calculated**</span><span class="sxs-lookup"><span data-stu-id="4a64b-181">**calculated**</span></span>    | <span data-ttu-id="4a64b-182">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-182">[calculatedColumn][]</span></span>    | <span data-ttu-id="4a64b-183">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="4a64b-183">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="4a64b-184">**choice**</span><span class="sxs-lookup"><span data-stu-id="4a64b-184">**choice**</span></span>        | <span data-ttu-id="4a64b-185">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-185">[choiceColumn][]</span></span>        | <span data-ttu-id="4a64b-186">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="4a64b-186">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="4a64b-187">**currency**</span><span class="sxs-lookup"><span data-stu-id="4a64b-187">**currency**</span></span>      | <span data-ttu-id="4a64b-188">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-188">[currencyColumn][]</span></span>      | <span data-ttu-id="4a64b-189">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="4a64b-189">This column stores currency values.</span></span>
| <span data-ttu-id="4a64b-190">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="4a64b-190">**dateTime**</span></span>      | <span data-ttu-id="4a64b-191">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-191">[dateTimeColumn][]</span></span>      | <span data-ttu-id="4a64b-192">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="4a64b-192">This column stores DateTime values.</span></span>
| <span data-ttu-id="4a64b-193">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="4a64b-193">**defaultValue**</span></span>  | <span data-ttu-id="4a64b-194">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-194">[defaultColumnValue][]</span></span>  | <span data-ttu-id="4a64b-195">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="4a64b-195">The default value for this column.</span></span>
| <span data-ttu-id="4a64b-196">**геолокация**</span><span class="sxs-lookup"><span data-stu-id="4a64b-196">**geolocation**</span></span>   | <span data-ttu-id="4a64b-197">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-197">[geolocationColumn][]</span></span>   | <span data-ttu-id="4a64b-198">В этом столбце хранится геолокация.</span><span class="sxs-lookup"><span data-stu-id="4a64b-198">This column stores a geolocation.</span></span>
| <span data-ttu-id="4a64b-199">**lookup**</span><span class="sxs-lookup"><span data-stu-id="4a64b-199">**lookup**</span></span>        | <span data-ttu-id="4a64b-200">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-200">[lookupColumn][]</span></span>        | <span data-ttu-id="4a64b-201">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="4a64b-201">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="4a64b-202">**number**</span><span class="sxs-lookup"><span data-stu-id="4a64b-202">**number**</span></span>        | <span data-ttu-id="4a64b-203">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-203">[numberColumn][]</span></span>        | <span data-ttu-id="4a64b-204">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="4a64b-204">This column stores number values.</span></span>
| <span data-ttu-id="4a64b-205">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="4a64b-205">**personOrGroup**</span></span> | <span data-ttu-id="4a64b-206">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-206">[personOrGroupColumn][]</span></span> | <span data-ttu-id="4a64b-207">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="4a64b-207">This column stores Person or Group values.</span></span>
| <span data-ttu-id="4a64b-208">**text**</span><span class="sxs-lookup"><span data-stu-id="4a64b-208">**text**</span></span>          | <span data-ttu-id="4a64b-209">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-209">[textColumn][]</span></span>          | <span data-ttu-id="4a64b-210">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="4a64b-210">This column stores text values.</span></span>
| <span data-ttu-id="4a64b-211">**isDeletable**</span><span class="sxs-lookup"><span data-stu-id="4a64b-211">**isDeletable**</span></span>       | <span data-ttu-id="4a64b-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64b-212">Boolean</span></span> | <span data-ttu-id="4a64b-213">Указывает, можно ли удалить этот столбец.</span><span class="sxs-lookup"><span data-stu-id="4a64b-213">Indicates whether this column can be deleted.</span></span>
| <span data-ttu-id="4a64b-214">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="4a64b-214">**propagateChanges**</span></span>     | <span data-ttu-id="4a64b-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64b-215">Boolean</span></span> | <span data-ttu-id="4a64b-216">Если изменения "True" в этом столбце будут распространяться в списки, реализующих столбец.</span><span class="sxs-lookup"><span data-stu-id="4a64b-216">If 'True' changes to this column will be propagated to lists that implement the column.</span></span> 
| <span data-ttu-id="4a64b-217">**isReorderable**</span><span class="sxs-lookup"><span data-stu-id="4a64b-217">**isReorderable**</span></span>         | <span data-ttu-id="4a64b-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64b-218">Boolean</span></span> | <span data-ttu-id="4a64b-219">Указывает, можно ли переуказать значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="4a64b-219">Indicates whether values in the column can be reordered.</span></span> <span data-ttu-id="4a64b-220">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a64b-220">Read-only.</span></span>
| <span data-ttu-id="4a64b-221">**isSealed**</span><span class="sxs-lookup"><span data-stu-id="4a64b-221">**isSealed**</span></span>              | <span data-ttu-id="4a64b-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64b-222">Boolean</span></span> | <span data-ttu-id="4a64b-223">Указывает, можно ли изменить столбец.</span><span class="sxs-lookup"><span data-stu-id="4a64b-223">Specifies whether column can be changed.</span></span>
| <span data-ttu-id="4a64b-224">**проверка**</span><span class="sxs-lookup"><span data-stu-id="4a64b-224">**validation**</span></span>   |  <span data-ttu-id="4a64b-225">[columnValidation][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-225">[columnValidation][]</span></span>    | <span data-ttu-id="4a64b-226">В этом столбце хранится формула проверки и сообщение для столбца.</span><span class="sxs-lookup"><span data-stu-id="4a64b-226">This column stores validation formula and message for the column.</span></span> 
| <span data-ttu-id="4a64b-227">**hyperlinkOrPicture**</span><span class="sxs-lookup"><span data-stu-id="4a64b-227">**hyperlinkOrPicture**</span></span>  | <span data-ttu-id="4a64b-228">[hyperlinkOrPictureColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-228">[hyperlinkOrPictureColumn][]</span></span> | <span data-ttu-id="4a64b-229">В этом столбце хранится гиперссылка или значения изображения.</span><span class="sxs-lookup"><span data-stu-id="4a64b-229">This column stores hyperlink or picture values.</span></span> 
| <span data-ttu-id="4a64b-230">**термин**</span><span class="sxs-lookup"><span data-stu-id="4a64b-230">**term**</span></span>     | <span data-ttu-id="4a64b-231">[termColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-231">[termColumn][]</span></span> | <span data-ttu-id="4a64b-232">В этом столбце хранится таксономия терминов.</span><span class="sxs-lookup"><span data-stu-id="4a64b-232">This column stores taxonomy terms.</span></span>
| <span data-ttu-id="4a64b-233">**sourceContentType**</span><span class="sxs-lookup"><span data-stu-id="4a64b-233">**sourceContentType**</span></span>   |<span data-ttu-id="4a64b-234">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-234">[contentTypeInfo][]</span></span>  | <span data-ttu-id="4a64b-235">ContentType, от которого наследуется этот столбец.</span><span class="sxs-lookup"><span data-stu-id="4a64b-235">ContentType from which this column is inherited from.</span></span> <span data-ttu-id="4a64b-236">Используется только при извлечении столбцов contentTypes.</span><span class="sxs-lookup"><span data-stu-id="4a64b-236">Used only while fetching contentTypes columns.</span></span>
| <span data-ttu-id="4a64b-237">**thumbnail**</span><span class="sxs-lookup"><span data-stu-id="4a64b-237">**thumbnail**</span></span>           |<span data-ttu-id="4a64b-238">[thumbnailColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-238">[thumbnailColumn][]</span></span>      | <span data-ttu-id="4a64b-239">В этом столбце хранится эскизные значения.</span><span class="sxs-lookup"><span data-stu-id="4a64b-239">This column stores thumbnail values.</span></span>
| <span data-ttu-id="4a64b-240">**type**</span><span class="sxs-lookup"><span data-stu-id="4a64b-240">**type**</span></span>         | <span data-ttu-id="4a64b-241">columnTypes</span><span class="sxs-lookup"><span data-stu-id="4a64b-241">columnTypes</span></span>  | <span data-ttu-id="4a64b-242">Для столбцов сайта тип столбца.</span><span class="sxs-lookup"><span data-stu-id="4a64b-242">For site columns, the type of column.</span></span> <span data-ttu-id="4a64b-243">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="4a64b-243">Read-only</span></span>
| <span data-ttu-id="4a64b-244">**contentApprovalStatus**</span><span class="sxs-lookup"><span data-stu-id="4a64b-244">**contentApprovalStatus**</span></span>| <span data-ttu-id="4a64b-245">[contentApprovalStatusColumn][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-245">[contentApprovalStatusColumn][]</span></span>     | <span data-ttu-id="4a64b-246">В этом столбце сохраняется состояние утверждения контента.</span><span class="sxs-lookup"><span data-stu-id="4a64b-246">This column stores content approval status.</span></span>

## <a name="relationships"></a><span data-ttu-id="4a64b-247">Связи</span><span class="sxs-lookup"><span data-stu-id="4a64b-247">Relationships</span></span>

| <span data-ttu-id="4a64b-248">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4a64b-248">Property name</span></span>   | <span data-ttu-id="4a64b-249">Тип</span><span class="sxs-lookup"><span data-stu-id="4a64b-249">Type</span></span>                      | <span data-ttu-id="4a64b-250">Описание</span><span class="sxs-lookup"><span data-stu-id="4a64b-250">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="4a64b-251">**sourceColumn**</span><span class="sxs-lookup"><span data-stu-id="4a64b-251">**sourceColumn**</span></span> | <span data-ttu-id="4a64b-252">[columnDefinition][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-252">[columnDefinition][]</span></span> | <span data-ttu-id="4a64b-253">Столбец исходный для столбца типа контента.</span><span class="sxs-lookup"><span data-stu-id="4a64b-253">The source column for content type column.</span></span>

><span data-ttu-id="4a64b-254">**Примечание:** Эти свойства соответствуют переумериям [SPFieldType в SharePoint.][]</span><span class="sxs-lookup"><span data-stu-id="4a64b-254">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="4a64b-255">Хотя наиболее распространенные типы полей представлены в предыдущей таблице, этот API бета-версии по-прежнему отсутствует.</span><span class="sxs-lookup"><span data-stu-id="4a64b-255">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="4a64b-256">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="4a64b-256">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="4a64b-257">Примечания</span><span class="sxs-lookup"><span data-stu-id="4a64b-257">Remarks</span></span>

<span data-ttu-id="4a64b-258">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="4a64b-258">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="4a64b-259">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="4a64b-259">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="4a64b-260">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="4a64b-260">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[columnDefinition]: columnDefinition.md
[contentType]: contenttype.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[list]: list.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[site]: site.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md
[termColumn]: termColumn.md
[contentApprovalStatusColumn]: contentApprovalStatusColumn.md
[thumbnailColumn]: thumbnailColumn.md
[hyperlinkOrPictureColumn]: hyperlinkOrPictureColumn.md
[columnValidation]: columnValidation.md
[contentTypeInfo]: contentTypeInfo.md

[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": []
}
-->