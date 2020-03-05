---
author: JeremyKelley
description: Ниже показано представление ресурса columnDefinition в формате JSON.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d36c7460b5ee50a6230cdacc5514e200920e31c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507630"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="0da2c-103">Тип ресурса columnDefinition</span><span class="sxs-lookup"><span data-stu-id="0da2c-103">columnDefinition resource type</span></span>

<span data-ttu-id="0da2c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0da2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="0da2c-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0da2c-105">JSON representation</span></span>

<span data-ttu-id="0da2c-106">Ниже показано представление ресурса columnDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0da2c-106">Here is a JSON representation of a columnDefinition resource.</span></span>

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
  "enforceUniqueValues": "true",
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
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="0da2c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0da2c-107">Properties</span></span>

<span data-ttu-id="0da2c-108">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="0da2c-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="0da2c-109">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="0da2c-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="0da2c-110">Свойства, связанные с типами (Boolean, вычисляемые, Choice, Currency, dateTime, Lookup, Number, Персонорграуп, Text), являются взаимно исключающими — столбец может содержать только один из них.</span><span class="sxs-lookup"><span data-stu-id="0da2c-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="0da2c-111">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="0da2c-111">Property name</span></span>           | <span data-ttu-id="0da2c-112">Тип</span><span class="sxs-lookup"><span data-stu-id="0da2c-112">Type</span></span>    | <span data-ttu-id="0da2c-113">Описание</span><span class="sxs-lookup"><span data-stu-id="0da2c-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="0da2c-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="0da2c-114">**columnGroup**</span></span>         | <span data-ttu-id="0da2c-115">строка</span><span class="sxs-lookup"><span data-stu-id="0da2c-115">string</span></span>  | <span data-ttu-id="0da2c-116">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="0da2c-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="0da2c-117">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="0da2c-117">Helps organize related columns.</span></span>
| <span data-ttu-id="0da2c-118">**description**</span><span class="sxs-lookup"><span data-stu-id="0da2c-118">**description**</span></span>         | <span data-ttu-id="0da2c-119">строка</span><span class="sxs-lookup"><span data-stu-id="0da2c-119">string</span></span>  | <span data-ttu-id="0da2c-120">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="0da2c-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="0da2c-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="0da2c-121">**displayName**</span></span>         | <span data-ttu-id="0da2c-122">string</span><span class="sxs-lookup"><span data-stu-id="0da2c-122">string</span></span>  | <span data-ttu-id="0da2c-123">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="0da2c-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="0da2c-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="0da2c-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="0da2c-125">boolean</span><span class="sxs-lookup"><span data-stu-id="0da2c-125">boolean</span></span> | <span data-ttu-id="0da2c-126">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="0da2c-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="0da2c-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="0da2c-127">**hidden**</span></span>              | <span data-ttu-id="0da2c-128">boolean</span><span class="sxs-lookup"><span data-stu-id="0da2c-128">boolean</span></span> | <span data-ttu-id="0da2c-129">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="0da2c-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="0da2c-130">**id**</span><span class="sxs-lookup"><span data-stu-id="0da2c-130">**id**</span></span>                  | <span data-ttu-id="0da2c-131">строка</span><span class="sxs-lookup"><span data-stu-id="0da2c-131">string</span></span>  | <span data-ttu-id="0da2c-132">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="0da2c-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="0da2c-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="0da2c-133">**indexed**</span></span>             | <span data-ttu-id="0da2c-134">boolean</span><span class="sxs-lookup"><span data-stu-id="0da2c-134">boolean</span></span> | <span data-ttu-id="0da2c-135">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="0da2c-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="0da2c-136">**name**</span><span class="sxs-lookup"><span data-stu-id="0da2c-136">**name**</span></span>                | <span data-ttu-id="0da2c-137">string</span><span class="sxs-lookup"><span data-stu-id="0da2c-137">string</span></span>  | <span data-ttu-id="0da2c-138">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="0da2c-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="0da2c-139">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="0da2c-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="0da2c-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="0da2c-140">**readOnly**</span></span>            | <span data-ttu-id="0da2c-141">логический</span><span class="sxs-lookup"><span data-stu-id="0da2c-141">bool</span></span>    | <span data-ttu-id="0da2c-142">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="0da2c-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="0da2c-143">**required**</span><span class="sxs-lookup"><span data-stu-id="0da2c-143">**required**</span></span>            | <span data-ttu-id="0da2c-144">логический</span><span class="sxs-lookup"><span data-stu-id="0da2c-144">boolean</span></span> | <span data-ttu-id="0da2c-145">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="0da2c-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="0da2c-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="0da2c-146">**boolean**</span></span>       | <span data-ttu-id="0da2c-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="0da2c-147">[booleanColumn][]</span></span>       | <span data-ttu-id="0da2c-148">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="0da2c-148">This column stores boolean values.</span></span>
| <span data-ttu-id="0da2c-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="0da2c-149">**calculated**</span></span>    | <span data-ttu-id="0da2c-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="0da2c-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="0da2c-151">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="0da2c-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="0da2c-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="0da2c-152">**choice**</span></span>        | <span data-ttu-id="0da2c-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="0da2c-153">[choiceColumn][]</span></span>        | <span data-ttu-id="0da2c-154">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="0da2c-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="0da2c-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="0da2c-155">**currency**</span></span>      | <span data-ttu-id="0da2c-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="0da2c-156">[currencyColumn][]</span></span>      | <span data-ttu-id="0da2c-157">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="0da2c-157">This column stores currency values.</span></span>
| <span data-ttu-id="0da2c-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="0da2c-158">**dateTime**</span></span>      | <span data-ttu-id="0da2c-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="0da2c-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="0da2c-160">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="0da2c-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="0da2c-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="0da2c-161">**defaultValue**</span></span>  | <span data-ttu-id="0da2c-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="0da2c-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="0da2c-163">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="0da2c-163">The default value for this column.</span></span>
| <span data-ttu-id="0da2c-164">**географическое положение**</span><span class="sxs-lookup"><span data-stu-id="0da2c-164">**geolocation**</span></span>   | <span data-ttu-id="0da2c-165">[жеолокатионколумн][]</span><span class="sxs-lookup"><span data-stu-id="0da2c-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="0da2c-166">В этом столбце хранится географическое положение.</span><span class="sxs-lookup"><span data-stu-id="0da2c-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="0da2c-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="0da2c-167">**lookup**</span></span>        | <span data-ttu-id="0da2c-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="0da2c-168">[lookupColumn][]</span></span>        | <span data-ttu-id="0da2c-169">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="0da2c-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="0da2c-170">**number**</span><span class="sxs-lookup"><span data-stu-id="0da2c-170">**number**</span></span>        | <span data-ttu-id="0da2c-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="0da2c-171">[numberColumn][]</span></span>        | <span data-ttu-id="0da2c-172">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="0da2c-172">This column stores number values.</span></span>
| <span data-ttu-id="0da2c-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="0da2c-173">**personOrGroup**</span></span> | <span data-ttu-id="0da2c-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="0da2c-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="0da2c-175">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="0da2c-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="0da2c-176">**text**</span><span class="sxs-lookup"><span data-stu-id="0da2c-176">**text**</span></span>          | <span data-ttu-id="0da2c-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="0da2c-177">[textColumn][]</span></span>          | <span data-ttu-id="0da2c-178">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="0da2c-178">This column stores text values.</span></span>

><span data-ttu-id="0da2c-179">**Примечание:** Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0da2c-179">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="0da2c-180">Несмотря на то, что наиболее распространенные типы полей представлены в предыдущей таблице, этот API по-прежнему отсутствует.</span><span class="sxs-lookup"><span data-stu-id="0da2c-180">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="0da2c-181">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="0da2c-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="0da2c-182">Примечания</span><span class="sxs-lookup"><span data-stu-id="0da2c-182">Remarks</span></span>

<span data-ttu-id="0da2c-183">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="0da2c-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="0da2c-184">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="0da2c-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="0da2c-185">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="0da2c-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[жеолокатионколумн]: geolocationcolumn.md
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx

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
