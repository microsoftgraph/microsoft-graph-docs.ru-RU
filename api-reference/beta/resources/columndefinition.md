---
author: JeremyKelley
description: Представляет столбец в сайте, списке или contentType.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 982b9751f522d34a5cdf1dd329262486d35bfb0a
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456473"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="51530-103">тип ресурса columnDefinition</span><span class="sxs-lookup"><span data-stu-id="51530-103">columnDefinition resource type</span></span>

<span data-ttu-id="51530-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51530-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51530-105">Представляет столбец на [сайте,][] [списке или][] [contentType.][]</span><span class="sxs-lookup"><span data-stu-id="51530-105">Represents a column in a [site][], [list][] or [contentType][].</span></span>

## <a name="methods"></a><span data-ttu-id="51530-106">Методы</span><span class="sxs-lookup"><span data-stu-id="51530-106">Methods</span></span>
|<span data-ttu-id="51530-107">Метод</span><span class="sxs-lookup"><span data-stu-id="51530-107">Method</span></span>|<span data-ttu-id="51530-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="51530-108">Return type</span></span>|<span data-ttu-id="51530-109">Описание</span><span class="sxs-lookup"><span data-stu-id="51530-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="51530-110">Список столбцов на сайте</span><span class="sxs-lookup"><span data-stu-id="51530-110">List columns in a site</span></span>](../api/site-list-columns.md)|<span data-ttu-id="51530-111">[коллекция columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="51530-111">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="51530-112">Получите список объектов [columnDefinition](../resources/columndefinition.md) и их свойств на [сайте.](../resources/site.md)</span><span class="sxs-lookup"><span data-stu-id="51530-112">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="51530-113">Список столбцов в списке</span><span class="sxs-lookup"><span data-stu-id="51530-113">List columns in a list</span></span>](../api/list-list-columns.md)|<span data-ttu-id="51530-114">[коллекция columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="51530-114">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="51530-115">Получите список объектов [columnDefinition](../resources/columndefinition.md) и их свойств в [списке.](../resources/list.md)</span><span class="sxs-lookup"><span data-stu-id="51530-115">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="51530-116">Список столбцов в типе контента</span><span class="sxs-lookup"><span data-stu-id="51530-116">List columns in a content type</span></span>](../api/contenttype-list-columns.md)|<span data-ttu-id="51530-117">[коллекция columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="51530-117">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="51530-118">Получите список объектов [columnDefinition](../resources/columndefinition.md) и их свойств в [типе контента.](../resources/contenttype.md)</span><span class="sxs-lookup"><span data-stu-id="51530-118">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="51530-119">Создание columnDefinition для сайта</span><span class="sxs-lookup"><span data-stu-id="51530-119">Create columnDefinition for a site</span></span>](../api/site-post-columns.md)|[<span data-ttu-id="51530-120">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="51530-120">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="51530-121">Создание нового [объекта columnDefinition](../resources/columndefinition.md) на [сайте.](../resources/site.md)</span><span class="sxs-lookup"><span data-stu-id="51530-121">Create a new [columnDefinition](../resources/columndefinition.md) object in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="51530-122">Создание columnDefinition для списка</span><span class="sxs-lookup"><span data-stu-id="51530-122">Create columnDefinition for a list</span></span>](../api/list-post-columns.md)|[<span data-ttu-id="51530-123">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="51530-123">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="51530-124">Создайте новый [объект columnDefinition](../resources/columndefinition.md) в [списке](../resources/list.md).</span><span class="sxs-lookup"><span data-stu-id="51530-124">Create a new [columnDefinition](../resources/columndefinition.md) object in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="51530-125">Создание columnDefinition для типа контента</span><span class="sxs-lookup"><span data-stu-id="51530-125">Create columnDefinition for a content type</span></span>](../api/contenttype-post-columns.md)|[<span data-ttu-id="51530-126">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="51530-126">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="51530-127">Создание нового [объекта columnDefinition](../resources/columndefinition.md) в [типе контента.](../resources/contenttype.md)</span><span class="sxs-lookup"><span data-stu-id="51530-127">Create a new [columnDefinition](../resources/columndefinition.md) object in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="51530-128">Получить columnDefinition</span><span class="sxs-lookup"><span data-stu-id="51530-128">Get columnDefinition</span></span>](../api/columndefinition-get.md)|[<span data-ttu-id="51530-129">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="51530-129">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="51530-130">Ознакомьтесь с свойствами и отношениями объекта [columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="51530-130">Read the properties and relationships of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="51530-131">Обновление столбцаDefinition</span><span class="sxs-lookup"><span data-stu-id="51530-131">Update columnDefinition</span></span>](../api/columndefinition-update.md)|[<span data-ttu-id="51530-132">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="51530-132">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="51530-133">Обновление свойств объекта [columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="51530-133">Update the properties of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="51530-134">Удаление columnDefinition</span><span class="sxs-lookup"><span data-stu-id="51530-134">Delete columnDefinition</span></span>](../api/columndefinition-delete.md)|<span data-ttu-id="51530-135">Нет</span><span class="sxs-lookup"><span data-stu-id="51530-135">None</span></span>|<span data-ttu-id="51530-136">Удаляет объект [columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="51530-136">Deletes a [columnDefinition](../resources/columndefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="51530-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="51530-137">Properties</span></span>

<span data-ttu-id="51530-138">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="51530-138">Columns can hold data of various types.</span></span>
<span data-ttu-id="51530-139">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="51530-139">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="51530-140">Свойства типа (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) являются взаимоисключающими : столбец может иметь только один из указанных.</span><span class="sxs-lookup"><span data-stu-id="51530-140">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="51530-141">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="51530-141">Property name</span></span>           | <span data-ttu-id="51530-142">Тип</span><span class="sxs-lookup"><span data-stu-id="51530-142">Type</span></span>    | <span data-ttu-id="51530-143">Описание</span><span class="sxs-lookup"><span data-stu-id="51530-143">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="51530-144">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="51530-144">**columnGroup**</span></span>         | <span data-ttu-id="51530-145">строка</span><span class="sxs-lookup"><span data-stu-id="51530-145">string</span></span>  | <span data-ttu-id="51530-146">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="51530-146">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="51530-147">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="51530-147">Helps organize related columns.</span></span>
| <span data-ttu-id="51530-148">**description**</span><span class="sxs-lookup"><span data-stu-id="51530-148">**description**</span></span>         | <span data-ttu-id="51530-149">string</span><span class="sxs-lookup"><span data-stu-id="51530-149">string</span></span>  | <span data-ttu-id="51530-150">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="51530-150">The user-facing description of the column.</span></span>
| <span data-ttu-id="51530-151">**displayName**</span><span class="sxs-lookup"><span data-stu-id="51530-151">**displayName**</span></span>         | <span data-ttu-id="51530-152">string</span><span class="sxs-lookup"><span data-stu-id="51530-152">string</span></span>  | <span data-ttu-id="51530-153">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="51530-153">The user-facing name of the column.</span></span>
| <span data-ttu-id="51530-154">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="51530-154">**enforceUniqueValues**</span></span> | <span data-ttu-id="51530-155">Логический</span><span class="sxs-lookup"><span data-stu-id="51530-155">Boolean</span></span> | <span data-ttu-id="51530-156">Если для этого столбца нет двух элементов `true` списка, то для этого столбца может быть одинаковое значение.</span><span class="sxs-lookup"><span data-stu-id="51530-156">If `true`, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="51530-157">**hidden**</span><span class="sxs-lookup"><span data-stu-id="51530-157">**hidden**</span></span>              | <span data-ttu-id="51530-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="51530-158">Boolean</span></span> | <span data-ttu-id="51530-159">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="51530-159">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="51530-160">**id**</span><span class="sxs-lookup"><span data-stu-id="51530-160">**id**</span></span>                  | <span data-ttu-id="51530-161">string</span><span class="sxs-lookup"><span data-stu-id="51530-161">string</span></span>  | <span data-ttu-id="51530-162">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="51530-162">The unique identifier for the column.</span></span>
| <span data-ttu-id="51530-163">**indexed**</span><span class="sxs-lookup"><span data-stu-id="51530-163">**indexed**</span></span>             | <span data-ttu-id="51530-164">Логический</span><span class="sxs-lookup"><span data-stu-id="51530-164">Boolean</span></span> | <span data-ttu-id="51530-165">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="51530-165">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="51530-166">**name**</span><span class="sxs-lookup"><span data-stu-id="51530-166">**name**</span></span>                | <span data-ttu-id="51530-167">string</span><span class="sxs-lookup"><span data-stu-id="51530-167">string</span></span>  | <span data-ttu-id="51530-168">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="51530-168">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="51530-169">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="51530-169">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="51530-170">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="51530-170">**readOnly**</span></span>            | <span data-ttu-id="51530-171">Логический</span><span class="sxs-lookup"><span data-stu-id="51530-171">Boolean</span></span>    | <span data-ttu-id="51530-172">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="51530-172">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="51530-173">**required**</span><span class="sxs-lookup"><span data-stu-id="51530-173">**required**</span></span>            | <span data-ttu-id="51530-174">Логический</span><span class="sxs-lookup"><span data-stu-id="51530-174">Boolean</span></span> | <span data-ttu-id="51530-175">Указывает, является ли значение столбца необязательным.</span><span class="sxs-lookup"><span data-stu-id="51530-175">Specifies whether the column value isn't optional.</span></span>
| <span data-ttu-id="51530-176">**boolean**</span><span class="sxs-lookup"><span data-stu-id="51530-176">**boolean**</span></span>       | <span data-ttu-id="51530-177">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-177">[booleanColumn][]</span></span>       | <span data-ttu-id="51530-178">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="51530-178">This column stores boolean values.</span></span>
| <span data-ttu-id="51530-179">**calculated**</span><span class="sxs-lookup"><span data-stu-id="51530-179">**calculated**</span></span>    | <span data-ttu-id="51530-180">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-180">[calculatedColumn][]</span></span>    | <span data-ttu-id="51530-181">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="51530-181">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="51530-182">**choice**</span><span class="sxs-lookup"><span data-stu-id="51530-182">**choice**</span></span>        | <span data-ttu-id="51530-183">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-183">[choiceColumn][]</span></span>        | <span data-ttu-id="51530-184">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="51530-184">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="51530-185">**currency**</span><span class="sxs-lookup"><span data-stu-id="51530-185">**currency**</span></span>      | <span data-ttu-id="51530-186">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-186">[currencyColumn][]</span></span>      | <span data-ttu-id="51530-187">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="51530-187">This column stores currency values.</span></span>
| <span data-ttu-id="51530-188">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="51530-188">**dateTime**</span></span>      | <span data-ttu-id="51530-189">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-189">[dateTimeColumn][]</span></span>      | <span data-ttu-id="51530-190">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="51530-190">This column stores DateTime values.</span></span>
| <span data-ttu-id="51530-191">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="51530-191">**defaultValue**</span></span>  | <span data-ttu-id="51530-192">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="51530-192">[defaultColumnValue][]</span></span>  | <span data-ttu-id="51530-193">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="51530-193">The default value for this column.</span></span>
| <span data-ttu-id="51530-194">**геолокация**</span><span class="sxs-lookup"><span data-stu-id="51530-194">**geolocation**</span></span>   | <span data-ttu-id="51530-195">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-195">[geolocationColumn][]</span></span>   | <span data-ttu-id="51530-196">В этом столбце хранится геолокация.</span><span class="sxs-lookup"><span data-stu-id="51530-196">This column stores a geolocation.</span></span>
| <span data-ttu-id="51530-197">**lookup**</span><span class="sxs-lookup"><span data-stu-id="51530-197">**lookup**</span></span>        | <span data-ttu-id="51530-198">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-198">[lookupColumn][]</span></span>        | <span data-ttu-id="51530-199">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="51530-199">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="51530-200">**number**</span><span class="sxs-lookup"><span data-stu-id="51530-200">**number**</span></span>        | <span data-ttu-id="51530-201">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-201">[numberColumn][]</span></span>        | <span data-ttu-id="51530-202">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="51530-202">This column stores number values.</span></span>
| <span data-ttu-id="51530-203">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="51530-203">**personOrGroup**</span></span> | <span data-ttu-id="51530-204">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-204">[personOrGroupColumn][]</span></span> | <span data-ttu-id="51530-205">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="51530-205">This column stores Person or Group values.</span></span>
| <span data-ttu-id="51530-206">**text**</span><span class="sxs-lookup"><span data-stu-id="51530-206">**text**</span></span>          | <span data-ttu-id="51530-207">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-207">[textColumn][]</span></span>          | <span data-ttu-id="51530-208">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="51530-208">This column stores text values.</span></span>
| <span data-ttu-id="51530-209">**isDeletable**</span><span class="sxs-lookup"><span data-stu-id="51530-209">**isDeletable**</span></span>       | <span data-ttu-id="51530-210">Логический</span><span class="sxs-lookup"><span data-stu-id="51530-210">Boolean</span></span> | <span data-ttu-id="51530-211">Указывает, можно ли удалить этот столбец.</span><span class="sxs-lookup"><span data-stu-id="51530-211">Indicates whether this column can be deleted.</span></span>
| <span data-ttu-id="51530-212">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="51530-212">**propagateChanges**</span></span>     | <span data-ttu-id="51530-213">Логический</span><span class="sxs-lookup"><span data-stu-id="51530-213">Boolean</span></span> | <span data-ttu-id="51530-214">Если `true` изменения в этом столбце будут распространяться в списки, реализующих столбец.</span><span class="sxs-lookup"><span data-stu-id="51530-214">If `true`, changes to this column will be propagated to lists that implement the column.</span></span> 
| <span data-ttu-id="51530-215">**isReorderable**</span><span class="sxs-lookup"><span data-stu-id="51530-215">**isReorderable**</span></span>         | <span data-ttu-id="51530-216">Логический</span><span class="sxs-lookup"><span data-stu-id="51530-216">Boolean</span></span> | <span data-ttu-id="51530-217">Указывает, можно ли переуказать значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="51530-217">Indicates whether values in the column can be reordered.</span></span> <span data-ttu-id="51530-218">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51530-218">Read-only.</span></span>
| <span data-ttu-id="51530-219">**isSealed**</span><span class="sxs-lookup"><span data-stu-id="51530-219">**isSealed**</span></span>              | <span data-ttu-id="51530-220">Логический</span><span class="sxs-lookup"><span data-stu-id="51530-220">Boolean</span></span> | <span data-ttu-id="51530-221">Указывает, можно ли изменить столбец.</span><span class="sxs-lookup"><span data-stu-id="51530-221">Specifies whether the column can be changed.</span></span>
| <span data-ttu-id="51530-222">**проверка**</span><span class="sxs-lookup"><span data-stu-id="51530-222">**validation**</span></span>   |  <span data-ttu-id="51530-223">[columnValidation][]</span><span class="sxs-lookup"><span data-stu-id="51530-223">[columnValidation][]</span></span>    | <span data-ttu-id="51530-224">В этом столбце хранится формула проверки и сообщение для столбца.</span><span class="sxs-lookup"><span data-stu-id="51530-224">This column stores validation formula and message for the column.</span></span> 
| <span data-ttu-id="51530-225">**hyperlinkOrPicture**</span><span class="sxs-lookup"><span data-stu-id="51530-225">**hyperlinkOrPicture**</span></span>  | <span data-ttu-id="51530-226">[hyperlinkOrPictureColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-226">[hyperlinkOrPictureColumn][]</span></span> | <span data-ttu-id="51530-227">В этом столбце хранится гиперссылка или значения изображения.</span><span class="sxs-lookup"><span data-stu-id="51530-227">This column stores hyperlink or picture values.</span></span> 
| <span data-ttu-id="51530-228">**термин**</span><span class="sxs-lookup"><span data-stu-id="51530-228">**term**</span></span>     | <span data-ttu-id="51530-229">[termColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-229">[termColumn][]</span></span> | <span data-ttu-id="51530-230">В этом столбце хранится таксономия терминов.</span><span class="sxs-lookup"><span data-stu-id="51530-230">This column stores taxonomy terms.</span></span>
| <span data-ttu-id="51530-231">**sourceContentType**</span><span class="sxs-lookup"><span data-stu-id="51530-231">**sourceContentType**</span></span>   |<span data-ttu-id="51530-232">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="51530-232">[contentTypeInfo][]</span></span>  | <span data-ttu-id="51530-233">ContentType, от которого наследуется этот столбец.</span><span class="sxs-lookup"><span data-stu-id="51530-233">ContentType from which this column is inherited from.</span></span> <span data-ttu-id="51530-234">Используется только для получения столбцов contentTypes.</span><span class="sxs-lookup"><span data-stu-id="51530-234">Used only to fetch contentTypes columns.</span></span>
| <span data-ttu-id="51530-235">**thumbnail**</span><span class="sxs-lookup"><span data-stu-id="51530-235">**thumbnail**</span></span>           |<span data-ttu-id="51530-236">[thumbnailColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-236">[thumbnailColumn][]</span></span>      | <span data-ttu-id="51530-237">В этом столбце хранится эскизные значения.</span><span class="sxs-lookup"><span data-stu-id="51530-237">This column stores thumbnail values.</span></span>
| <span data-ttu-id="51530-238">**type**</span><span class="sxs-lookup"><span data-stu-id="51530-238">**type**</span></span>         | <span data-ttu-id="51530-239">columnTypes</span><span class="sxs-lookup"><span data-stu-id="51530-239">columnTypes</span></span>  | <span data-ttu-id="51530-240">Для столбцов сайта тип столбца.</span><span class="sxs-lookup"><span data-stu-id="51530-240">For site columns, the type of column.</span></span> <span data-ttu-id="51530-241">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51530-241">Read-only.</span></span>
| <span data-ttu-id="51530-242">**contentApprovalStatus**</span><span class="sxs-lookup"><span data-stu-id="51530-242">**contentApprovalStatus**</span></span>| <span data-ttu-id="51530-243">[contentApprovalStatusColumn][]</span><span class="sxs-lookup"><span data-stu-id="51530-243">[contentApprovalStatusColumn][]</span></span>     | <span data-ttu-id="51530-244">В этом столбце сохраняется состояние утверждения контента.</span><span class="sxs-lookup"><span data-stu-id="51530-244">This column stores content approval status.</span></span>

## <a name="relationships"></a><span data-ttu-id="51530-245">Связи</span><span class="sxs-lookup"><span data-stu-id="51530-245">Relationships</span></span>

| <span data-ttu-id="51530-246">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="51530-246">Property name</span></span>   | <span data-ttu-id="51530-247">Тип</span><span class="sxs-lookup"><span data-stu-id="51530-247">Type</span></span>                      | <span data-ttu-id="51530-248">Описание</span><span class="sxs-lookup"><span data-stu-id="51530-248">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="51530-249">**sourceColumn**</span><span class="sxs-lookup"><span data-stu-id="51530-249">**sourceColumn**</span></span> | <span data-ttu-id="51530-250">[columnDefinition][]</span><span class="sxs-lookup"><span data-stu-id="51530-250">[columnDefinition][]</span></span> | <span data-ttu-id="51530-251">Столбец исходный для столбца типа контента.</span><span class="sxs-lookup"><span data-stu-id="51530-251">The source column for content type column.</span></span>

><span data-ttu-id="51530-252">**Примечание:** Эти свойства соответствуют SharePoint [SPFieldType.][]</span><span class="sxs-lookup"><span data-stu-id="51530-252">**Note:** These properties correspond to the SharePoint [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="51530-253">Обратите внимание, что наиболее распространенные типы полей представлены в предыдущей таблице.</span><span class="sxs-lookup"><span data-stu-id="51530-253">Note that the most common field types are represented in the previous table.</span></span> <span data-ttu-id="51530-254">Однако этот бета-API по-прежнему отсутствует.</span><span class="sxs-lookup"><span data-stu-id="51530-254">However, this beta API is still missing some.</span></span>
<span data-ttu-id="51530-255">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="51530-255">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="51530-256">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51530-256">JSON representation</span></span>

<span data-ttu-id="51530-257">Вот представление JSON ресурса columnDefinition.</span><span class="sxs-lookup"><span data-stu-id="51530-257">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="51530-258">Примечания</span><span class="sxs-lookup"><span data-stu-id="51530-258">Remarks</span></span>

<span data-ttu-id="51530-259">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="51530-259">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="51530-260">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="51530-260">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="51530-261">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="51530-261">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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
