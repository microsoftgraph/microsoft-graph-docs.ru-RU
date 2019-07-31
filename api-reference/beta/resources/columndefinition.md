---
author: JeremyKelley
description: Ниже показано представление ресурса columnDefinition в формате JSON.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7f60d33f8fbfe76c9dfd0ca02c98df96ca6ab380
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973302"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="affde-103">Тип ресурса columnDefinition</span><span class="sxs-lookup"><span data-stu-id="affde-103">columnDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="affde-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="affde-104">JSON representation</span></span>

<span data-ttu-id="affde-105">Ниже показано представление ресурса columnDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="affde-105">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="affde-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="affde-106">Properties</span></span>

<span data-ttu-id="affde-107">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="affde-107">Columns can hold data of various types.</span></span>
<span data-ttu-id="affde-108">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="affde-108">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="affde-109">Свойства, связанные с типами (Boolean, вычисляемые, Choice, Currency, dateTime, Lookup, Number, Персонорграуп, Text), являются взаимно исключающими — столбец может содержать только один из них.</span><span class="sxs-lookup"><span data-stu-id="affde-109">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="affde-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="affde-110">Property name</span></span>           | <span data-ttu-id="affde-111">Тип</span><span class="sxs-lookup"><span data-stu-id="affde-111">Type</span></span>    | <span data-ttu-id="affde-112">Описание</span><span class="sxs-lookup"><span data-stu-id="affde-112">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="affde-113">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="affde-113">**columnGroup**</span></span>         | <span data-ttu-id="affde-114">строка</span><span class="sxs-lookup"><span data-stu-id="affde-114">string</span></span>  | <span data-ttu-id="affde-115">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="affde-115">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="affde-116">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="affde-116">Helps organize related columns.</span></span>
| <span data-ttu-id="affde-117">**description**</span><span class="sxs-lookup"><span data-stu-id="affde-117">**description**</span></span>         | <span data-ttu-id="affde-118">строка</span><span class="sxs-lookup"><span data-stu-id="affde-118">string</span></span>  | <span data-ttu-id="affde-119">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="affde-119">The user-facing description of the column.</span></span>
| <span data-ttu-id="affde-120">**displayName**</span><span class="sxs-lookup"><span data-stu-id="affde-120">**displayName**</span></span>         | <span data-ttu-id="affde-121">string</span><span class="sxs-lookup"><span data-stu-id="affde-121">string</span></span>  | <span data-ttu-id="affde-122">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="affde-122">The user-facing name of the column.</span></span>
| <span data-ttu-id="affde-123">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="affde-123">**enforceUniqueValues**</span></span> | <span data-ttu-id="affde-124">boolean</span><span class="sxs-lookup"><span data-stu-id="affde-124">boolean</span></span> | <span data-ttu-id="affde-125">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="affde-125">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="affde-126">**hidden**</span><span class="sxs-lookup"><span data-stu-id="affde-126">**hidden**</span></span>              | <span data-ttu-id="affde-127">boolean</span><span class="sxs-lookup"><span data-stu-id="affde-127">boolean</span></span> | <span data-ttu-id="affde-128">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="affde-128">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="affde-129">**id**</span><span class="sxs-lookup"><span data-stu-id="affde-129">**id**</span></span>                  | <span data-ttu-id="affde-130">string</span><span class="sxs-lookup"><span data-stu-id="affde-130">string</span></span>  | <span data-ttu-id="affde-131">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="affde-131">The unique identifier for the column.</span></span>
| <span data-ttu-id="affde-132">**indexed**</span><span class="sxs-lookup"><span data-stu-id="affde-132">**indexed**</span></span>             | <span data-ttu-id="affde-133">boolean</span><span class="sxs-lookup"><span data-stu-id="affde-133">boolean</span></span> | <span data-ttu-id="affde-134">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="affde-134">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="affde-135">**name**</span><span class="sxs-lookup"><span data-stu-id="affde-135">**name**</span></span>                | <span data-ttu-id="affde-136">string</span><span class="sxs-lookup"><span data-stu-id="affde-136">string</span></span>  | <span data-ttu-id="affde-137">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="affde-137">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="affde-138">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="affde-138">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="affde-139">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="affde-139">**readOnly**</span></span>            | <span data-ttu-id="affde-140">логический</span><span class="sxs-lookup"><span data-stu-id="affde-140">bool</span></span>    | <span data-ttu-id="affde-141">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="affde-141">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="affde-142">**required**</span><span class="sxs-lookup"><span data-stu-id="affde-142">**required**</span></span>            | <span data-ttu-id="affde-143">логический</span><span class="sxs-lookup"><span data-stu-id="affde-143">boolean</span></span> | <span data-ttu-id="affde-144">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="affde-144">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="affde-145">**boolean**</span><span class="sxs-lookup"><span data-stu-id="affde-145">**boolean**</span></span>       | <span data-ttu-id="affde-146">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="affde-146">[booleanColumn][]</span></span>       | <span data-ttu-id="affde-147">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="affde-147">This column stores boolean values.</span></span>
| <span data-ttu-id="affde-148">**calculated**</span><span class="sxs-lookup"><span data-stu-id="affde-148">**calculated**</span></span>    | <span data-ttu-id="affde-149">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="affde-149">[calculatedColumn][]</span></span>    | <span data-ttu-id="affde-150">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="affde-150">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="affde-151">**choice**</span><span class="sxs-lookup"><span data-stu-id="affde-151">**choice**</span></span>        | <span data-ttu-id="affde-152">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="affde-152">[choiceColumn][]</span></span>        | <span data-ttu-id="affde-153">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="affde-153">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="affde-154">**currency**</span><span class="sxs-lookup"><span data-stu-id="affde-154">**currency**</span></span>      | <span data-ttu-id="affde-155">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="affde-155">[currencyColumn][]</span></span>      | <span data-ttu-id="affde-156">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="affde-156">This column stores currency values.</span></span>
| <span data-ttu-id="affde-157">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="affde-157">**dateTime**</span></span>      | <span data-ttu-id="affde-158">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="affde-158">[dateTimeColumn][]</span></span>      | <span data-ttu-id="affde-159">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="affde-159">This column stores DateTime values.</span></span>
| <span data-ttu-id="affde-160">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="affde-160">**defaultValue**</span></span>  | <span data-ttu-id="affde-161">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="affde-161">[defaultColumnValue][]</span></span>  | <span data-ttu-id="affde-162">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="affde-162">The default value for this column.</span></span>
| <span data-ttu-id="affde-163">**географическое положение**</span><span class="sxs-lookup"><span data-stu-id="affde-163">**geolocation**</span></span>   | <span data-ttu-id="affde-164">[Жеолокатионколумн][]</span><span class="sxs-lookup"><span data-stu-id="affde-164">[geolocationColumn][]</span></span>   | <span data-ttu-id="affde-165">В этом столбце хранится географическое положение.</span><span class="sxs-lookup"><span data-stu-id="affde-165">This column stores a geolocation.</span></span>
| <span data-ttu-id="affde-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="affde-166">**lookup**</span></span>        | <span data-ttu-id="affde-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="affde-167">[lookupColumn][]</span></span>        | <span data-ttu-id="affde-168">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="affde-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="affde-169">**number**</span><span class="sxs-lookup"><span data-stu-id="affde-169">**number**</span></span>        | <span data-ttu-id="affde-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="affde-170">[numberColumn][]</span></span>        | <span data-ttu-id="affde-171">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="affde-171">This column stores number values.</span></span>
| <span data-ttu-id="affde-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="affde-172">**personOrGroup**</span></span> | <span data-ttu-id="affde-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="affde-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="affde-174">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="affde-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="affde-175">**text**</span><span class="sxs-lookup"><span data-stu-id="affde-175">**text**</span></span>          | <span data-ttu-id="affde-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="affde-176">[textColumn][]</span></span>          | <span data-ttu-id="affde-177">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="affde-177">This column stores text values.</span></span>

><span data-ttu-id="affde-178">**Примечание:** Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="affde-178">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="affde-179">Несмотря на то, что наиболее распространенные типы полей представлены в предыдущей таблице, этот API по-прежнему отсутствует.</span><span class="sxs-lookup"><span data-stu-id="affde-179">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="affde-180">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="affde-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="affde-181">Примечания</span><span class="sxs-lookup"><span data-stu-id="affde-181">Remarks</span></span>

<span data-ttu-id="affde-182">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="affde-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="affde-183">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="affde-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="affde-184">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="affde-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[Жеолокатионколумн]: geolocationcolumn.md
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
