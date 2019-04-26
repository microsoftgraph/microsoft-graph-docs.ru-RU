---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: c5cce4c3db7b66ff46a6bab0bbfaacd0ecc9a6cc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341424"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="e4e28-102">Тип ресурса columnDefinition</span><span class="sxs-lookup"><span data-stu-id="e4e28-102">columnDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="e4e28-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4e28-103">JSON representation</span></span>

<span data-ttu-id="e4e28-104">Ниже показано представление ресурса columnDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4e28-104">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e4e28-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4e28-105">Properties</span></span>

<span data-ttu-id="e4e28-106">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="e4e28-106">Columns can hold data of various types.</span></span>
<span data-ttu-id="e4e28-107">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="e4e28-107">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="e4e28-108">Свойства, связанные с типами (Boolean, вычисляемые, Choice, Currency, dateTime, Lookup, Number, Персонорграуп, Text), являются взаимно исключающими — столбец может содержать только один из них.</span><span class="sxs-lookup"><span data-stu-id="e4e28-108">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="e4e28-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e4e28-109">Property name</span></span>           | <span data-ttu-id="e4e28-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e4e28-110">Type</span></span>    | <span data-ttu-id="e4e28-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e4e28-111">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="e4e28-112">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="e4e28-112">**columnGroup**</span></span>         | <span data-ttu-id="e4e28-113">строка</span><span class="sxs-lookup"><span data-stu-id="e4e28-113">string</span></span>  | <span data-ttu-id="e4e28-114">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="e4e28-114">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="e4e28-115">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="e4e28-115">Helps organize related columns.</span></span>
| <span data-ttu-id="e4e28-116">**description**</span><span class="sxs-lookup"><span data-stu-id="e4e28-116">**description**</span></span>         | <span data-ttu-id="e4e28-117">строка</span><span class="sxs-lookup"><span data-stu-id="e4e28-117">string</span></span>  | <span data-ttu-id="e4e28-118">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="e4e28-118">The user-facing description of the column.</span></span>
| <span data-ttu-id="e4e28-119">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e4e28-119">**displayName**</span></span>         | <span data-ttu-id="e4e28-120">string</span><span class="sxs-lookup"><span data-stu-id="e4e28-120">string</span></span>  | <span data-ttu-id="e4e28-121">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="e4e28-121">The user-facing name of the column.</span></span>
| <span data-ttu-id="e4e28-122">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="e4e28-122">**enforceUniqueValues**</span></span> | <span data-ttu-id="e4e28-123">boolean</span><span class="sxs-lookup"><span data-stu-id="e4e28-123">boolean</span></span> | <span data-ttu-id="e4e28-124">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="e4e28-124">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="e4e28-125">**hidden**</span><span class="sxs-lookup"><span data-stu-id="e4e28-125">**hidden**</span></span>              | <span data-ttu-id="e4e28-126">boolean</span><span class="sxs-lookup"><span data-stu-id="e4e28-126">boolean</span></span> | <span data-ttu-id="e4e28-127">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="e4e28-127">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="e4e28-128">**id**</span><span class="sxs-lookup"><span data-stu-id="e4e28-128">**id**</span></span>                  | <span data-ttu-id="e4e28-129">string</span><span class="sxs-lookup"><span data-stu-id="e4e28-129">string</span></span>  | <span data-ttu-id="e4e28-130">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="e4e28-130">The unique identifier for the column.</span></span>
| <span data-ttu-id="e4e28-131">**indexed**</span><span class="sxs-lookup"><span data-stu-id="e4e28-131">**indexed**</span></span>             | <span data-ttu-id="e4e28-132">boolean</span><span class="sxs-lookup"><span data-stu-id="e4e28-132">boolean</span></span> | <span data-ttu-id="e4e28-133">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="e4e28-133">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="e4e28-134">**name**</span><span class="sxs-lookup"><span data-stu-id="e4e28-134">**name**</span></span>                | <span data-ttu-id="e4e28-135">string</span><span class="sxs-lookup"><span data-stu-id="e4e28-135">string</span></span>  | <span data-ttu-id="e4e28-136">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="e4e28-136">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="e4e28-137">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="e4e28-137">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="e4e28-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="e4e28-138">**readOnly**</span></span>            | <span data-ttu-id="e4e28-139">логический</span><span class="sxs-lookup"><span data-stu-id="e4e28-139">bool</span></span>    | <span data-ttu-id="e4e28-140">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="e4e28-140">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="e4e28-141">**required**</span><span class="sxs-lookup"><span data-stu-id="e4e28-141">**required**</span></span>            | <span data-ttu-id="e4e28-142">логический</span><span class="sxs-lookup"><span data-stu-id="e4e28-142">boolean</span></span> | <span data-ttu-id="e4e28-143">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="e4e28-143">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="e4e28-144">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e4e28-144">**boolean**</span></span>       | <span data-ttu-id="e4e28-145">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="e4e28-145">[booleanColumn][]</span></span>       | <span data-ttu-id="e4e28-146">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="e4e28-146">This column stores boolean values.</span></span>
| <span data-ttu-id="e4e28-147">**calculated**</span><span class="sxs-lookup"><span data-stu-id="e4e28-147">**calculated**</span></span>    | <span data-ttu-id="e4e28-148">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="e4e28-148">[calculatedColumn][]</span></span>    | <span data-ttu-id="e4e28-149">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="e4e28-149">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="e4e28-150">**choice**</span><span class="sxs-lookup"><span data-stu-id="e4e28-150">**choice**</span></span>        | <span data-ttu-id="e4e28-151">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="e4e28-151">[choiceColumn][]</span></span>        | <span data-ttu-id="e4e28-152">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="e4e28-152">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="e4e28-153">**currency**</span><span class="sxs-lookup"><span data-stu-id="e4e28-153">**currency**</span></span>      | <span data-ttu-id="e4e28-154">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="e4e28-154">[currencyColumn][]</span></span>      | <span data-ttu-id="e4e28-155">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="e4e28-155">This column stores currency values.</span></span>
| <span data-ttu-id="e4e28-156">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="e4e28-156">**dateTime**</span></span>      | <span data-ttu-id="e4e28-157">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="e4e28-157">[dateTimeColumn][]</span></span>      | <span data-ttu-id="e4e28-158">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="e4e28-158">This column stores DateTime values.</span></span>
| <span data-ttu-id="e4e28-159">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="e4e28-159">**defaultValue**</span></span>  | <span data-ttu-id="e4e28-160">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="e4e28-160">[defaultColumnValue][]</span></span>  | <span data-ttu-id="e4e28-161">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="e4e28-161">The default value for this column.</span></span>
| <span data-ttu-id="e4e28-162">**географическое положение**</span><span class="sxs-lookup"><span data-stu-id="e4e28-162">**geolocation**</span></span>   | <span data-ttu-id="e4e28-163">[Жеолокатионколумн][]</span><span class="sxs-lookup"><span data-stu-id="e4e28-163">[geolocationColumn][]</span></span>   | <span data-ttu-id="e4e28-164">В этом столбце хранится географическое положение.</span><span class="sxs-lookup"><span data-stu-id="e4e28-164">This column stores a geolocation.</span></span>
| <span data-ttu-id="e4e28-165">**lookup**</span><span class="sxs-lookup"><span data-stu-id="e4e28-165">**lookup**</span></span>        | <span data-ttu-id="e4e28-166">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e4e28-166">[lookupColumn][]</span></span>        | <span data-ttu-id="e4e28-167">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="e4e28-167">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="e4e28-168">**number**</span><span class="sxs-lookup"><span data-stu-id="e4e28-168">**number**</span></span>        | <span data-ttu-id="e4e28-169">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="e4e28-169">[numberColumn][]</span></span>        | <span data-ttu-id="e4e28-170">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="e4e28-170">This column stores number values.</span></span>
| <span data-ttu-id="e4e28-171">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="e4e28-171">**personOrGroup**</span></span> | <span data-ttu-id="e4e28-172">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e4e28-172">[personOrGroupColumn][]</span></span> | <span data-ttu-id="e4e28-173">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="e4e28-173">This column stores Person or Group values.</span></span>
| <span data-ttu-id="e4e28-174">**text**</span><span class="sxs-lookup"><span data-stu-id="e4e28-174">**text**</span></span>          | <span data-ttu-id="e4e28-175">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="e4e28-175">[textColumn][]</span></span>          | <span data-ttu-id="e4e28-176">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="e4e28-176">This column stores text values.</span></span>

><span data-ttu-id="e4e28-177">**Примечание:** Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e4e28-177">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="e4e28-178">Несмотря на то, что наиболее распространенные типы полей представлены в предыдущей таблице, этот API по-прежнему отсутствует.</span><span class="sxs-lookup"><span data-stu-id="e4e28-178">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="e4e28-179">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="e4e28-179">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="e4e28-180">Примечания</span><span class="sxs-lookup"><span data-stu-id="e4e28-180">Remarks</span></span>

<span data-ttu-id="e4e28-181">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="e4e28-181">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="e4e28-182">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="e4e28-182">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="e4e28-183">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="e4e28-183">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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
