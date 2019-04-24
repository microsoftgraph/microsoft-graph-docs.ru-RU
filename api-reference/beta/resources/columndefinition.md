---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: ddd6b3c6d3048bf7a6d3ab2dbc8ff7259651ee2f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460626"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="eeae1-102">Тип ресурса columnDefinition</span><span class="sxs-lookup"><span data-stu-id="eeae1-102">columnDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="eeae1-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eeae1-103">JSON representation</span></span>

<span data-ttu-id="eeae1-104">Ниже показано представление ресурса columnDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eeae1-104">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="eeae1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="eeae1-105">Properties</span></span>

<span data-ttu-id="eeae1-106">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="eeae1-106">Columns can hold data of various types.</span></span>
<span data-ttu-id="eeae1-107">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="eeae1-107">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="eeae1-108">Свойства, связанные с типами (Boolean, вычисляемые, Choice, Currency, dateTime, Lookup, Number, Персонорграуп, Text), являются взаимно исключающими — столбец может содержать только один из них.</span><span class="sxs-lookup"><span data-stu-id="eeae1-108">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="eeae1-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="eeae1-109">Property name</span></span>           | <span data-ttu-id="eeae1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eeae1-110">Type</span></span>    | <span data-ttu-id="eeae1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eeae1-111">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="eeae1-112">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="eeae1-112">**columnGroup**</span></span>         | <span data-ttu-id="eeae1-113">строка</span><span class="sxs-lookup"><span data-stu-id="eeae1-113">string</span></span>  | <span data-ttu-id="eeae1-114">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="eeae1-114">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="eeae1-115">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="eeae1-115">Helps organize related columns.</span></span>
| <span data-ttu-id="eeae1-116">**description**</span><span class="sxs-lookup"><span data-stu-id="eeae1-116">**description**</span></span>         | <span data-ttu-id="eeae1-117">строка</span><span class="sxs-lookup"><span data-stu-id="eeae1-117">string</span></span>  | <span data-ttu-id="eeae1-118">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="eeae1-118">The user-facing description of the column.</span></span>
| <span data-ttu-id="eeae1-119">**displayName**</span><span class="sxs-lookup"><span data-stu-id="eeae1-119">**displayName**</span></span>         | <span data-ttu-id="eeae1-120">string</span><span class="sxs-lookup"><span data-stu-id="eeae1-120">string</span></span>  | <span data-ttu-id="eeae1-121">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="eeae1-121">The user-facing name of the column.</span></span>
| <span data-ttu-id="eeae1-122">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="eeae1-122">**enforceUniqueValues**</span></span> | <span data-ttu-id="eeae1-123">логический</span><span class="sxs-lookup"><span data-stu-id="eeae1-123">boolean</span></span> | <span data-ttu-id="eeae1-124">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="eeae1-124">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="eeae1-125">**hidden**</span><span class="sxs-lookup"><span data-stu-id="eeae1-125">**hidden**</span></span>              | <span data-ttu-id="eeae1-126">boolean</span><span class="sxs-lookup"><span data-stu-id="eeae1-126">boolean</span></span> | <span data-ttu-id="eeae1-127">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="eeae1-127">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="eeae1-128">**id**</span><span class="sxs-lookup"><span data-stu-id="eeae1-128">**id**</span></span>                  | <span data-ttu-id="eeae1-129">string</span><span class="sxs-lookup"><span data-stu-id="eeae1-129">string</span></span>  | <span data-ttu-id="eeae1-130">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="eeae1-130">The unique identifier for the column.</span></span>
| <span data-ttu-id="eeae1-131">**indexed**</span><span class="sxs-lookup"><span data-stu-id="eeae1-131">**indexed**</span></span>             | <span data-ttu-id="eeae1-132">логический</span><span class="sxs-lookup"><span data-stu-id="eeae1-132">boolean</span></span> | <span data-ttu-id="eeae1-133">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="eeae1-133">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="eeae1-134">**name**</span><span class="sxs-lookup"><span data-stu-id="eeae1-134">**name**</span></span>                | <span data-ttu-id="eeae1-135">string</span><span class="sxs-lookup"><span data-stu-id="eeae1-135">string</span></span>  | <span data-ttu-id="eeae1-136">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="eeae1-136">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="eeae1-137">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="eeae1-137">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="eeae1-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="eeae1-138">**readOnly**</span></span>            | <span data-ttu-id="eeae1-139">логический</span><span class="sxs-lookup"><span data-stu-id="eeae1-139">bool</span></span>    | <span data-ttu-id="eeae1-140">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="eeae1-140">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="eeae1-141">**required**</span><span class="sxs-lookup"><span data-stu-id="eeae1-141">**required**</span></span>            | <span data-ttu-id="eeae1-142">логический</span><span class="sxs-lookup"><span data-stu-id="eeae1-142">boolean</span></span> | <span data-ttu-id="eeae1-143">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="eeae1-143">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="eeae1-144">**boolean**</span><span class="sxs-lookup"><span data-stu-id="eeae1-144">**boolean**</span></span>       | <span data-ttu-id="eeae1-145">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="eeae1-145">[booleanColumn][]</span></span>       | <span data-ttu-id="eeae1-146">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="eeae1-146">This column stores boolean values.</span></span>
| <span data-ttu-id="eeae1-147">**calculated**</span><span class="sxs-lookup"><span data-stu-id="eeae1-147">**calculated**</span></span>    | <span data-ttu-id="eeae1-148">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="eeae1-148">[calculatedColumn][]</span></span>    | <span data-ttu-id="eeae1-149">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="eeae1-149">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="eeae1-150">**choice**</span><span class="sxs-lookup"><span data-stu-id="eeae1-150">**choice**</span></span>        | <span data-ttu-id="eeae1-151">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="eeae1-151">[choiceColumn][]</span></span>        | <span data-ttu-id="eeae1-152">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="eeae1-152">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="eeae1-153">**currency**</span><span class="sxs-lookup"><span data-stu-id="eeae1-153">**currency**</span></span>      | <span data-ttu-id="eeae1-154">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="eeae1-154">[currencyColumn][]</span></span>      | <span data-ttu-id="eeae1-155">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="eeae1-155">This column stores currency values.</span></span>
| <span data-ttu-id="eeae1-156">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="eeae1-156">**dateTime**</span></span>      | <span data-ttu-id="eeae1-157">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="eeae1-157">[dateTimeColumn][]</span></span>      | <span data-ttu-id="eeae1-158">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="eeae1-158">This column stores DateTime values.</span></span>
| <span data-ttu-id="eeae1-159">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="eeae1-159">**defaultValue**</span></span>  | <span data-ttu-id="eeae1-160">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="eeae1-160">[defaultColumnValue][]</span></span>  | <span data-ttu-id="eeae1-161">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="eeae1-161">The default value for this column.</span></span>
| <span data-ttu-id="eeae1-162">**географическое положение**</span><span class="sxs-lookup"><span data-stu-id="eeae1-162">**geolocation**</span></span>   | <span data-ttu-id="eeae1-163">[Жеолокатионколумн][]</span><span class="sxs-lookup"><span data-stu-id="eeae1-163">[geolocationColumn][]</span></span>   | <span data-ttu-id="eeae1-164">В этом столбце хранится географическое положение.</span><span class="sxs-lookup"><span data-stu-id="eeae1-164">This column stores a geolocation.</span></span>
| <span data-ttu-id="eeae1-165">**lookup**</span><span class="sxs-lookup"><span data-stu-id="eeae1-165">**lookup**</span></span>        | <span data-ttu-id="eeae1-166">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="eeae1-166">[lookupColumn][]</span></span>        | <span data-ttu-id="eeae1-167">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="eeae1-167">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="eeae1-168">**number**</span><span class="sxs-lookup"><span data-stu-id="eeae1-168">**number**</span></span>        | <span data-ttu-id="eeae1-169">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="eeae1-169">[numberColumn][]</span></span>        | <span data-ttu-id="eeae1-170">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="eeae1-170">This column stores number values.</span></span>
| <span data-ttu-id="eeae1-171">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="eeae1-171">**personOrGroup**</span></span> | <span data-ttu-id="eeae1-172">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="eeae1-172">[personOrGroupColumn][]</span></span> | <span data-ttu-id="eeae1-173">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="eeae1-173">This column stores Person or Group values.</span></span>
| <span data-ttu-id="eeae1-174">**text**</span><span class="sxs-lookup"><span data-stu-id="eeae1-174">**text**</span></span>          | <span data-ttu-id="eeae1-175">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="eeae1-175">[textColumn][]</span></span>          | <span data-ttu-id="eeae1-176">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="eeae1-176">This column stores text values.</span></span>

><span data-ttu-id="eeae1-177">**Примечание:** Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eeae1-177">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="eeae1-178">Несмотря на то, что наиболее распространенные типы полей представлены в предыдущей таблице, этот API по-прежнему отсутствует.</span><span class="sxs-lookup"><span data-stu-id="eeae1-178">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="eeae1-179">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="eeae1-179">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="eeae1-180">Примечания</span><span class="sxs-lookup"><span data-stu-id="eeae1-180">Remarks</span></span>

<span data-ttu-id="eeae1-181">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="eeae1-181">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="eeae1-182">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="eeae1-182">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="eeae1-183">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="eeae1-183">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/columndefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
