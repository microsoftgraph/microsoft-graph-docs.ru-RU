---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: f4e0c3002068ec7dc8ee280b8e8143af621f178c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528937"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="e0c87-102">Тип ресурса columnDefinition</span><span class="sxs-lookup"><span data-stu-id="e0c87-102">columnDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="e0c87-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e0c87-103">JSON representation</span></span>

<span data-ttu-id="e0c87-104">Ниже представлена JSON columnDefinition ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0c87-104">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e0c87-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0c87-105">Properties</span></span>

<span data-ttu-id="e0c87-106">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="e0c87-106">Columns can hold data of various types.</span></span>
<span data-ttu-id="e0c87-107">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="e0c87-107">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="e0c87-108">Тип свойства, связанные с (типа boolean, вычисляемых, выбор, валюты, даты и времени, подстановки, номер, personOrGroup, текст) являются взаимоисключающими (столбец может иметь только один из них указан).</span><span class="sxs-lookup"><span data-stu-id="e0c87-108">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="e0c87-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e0c87-109">Property name</span></span>           | <span data-ttu-id="e0c87-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e0c87-110">Type</span></span>    | <span data-ttu-id="e0c87-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e0c87-111">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="e0c87-112">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="e0c87-112">**columnGroup**</span></span>         | <span data-ttu-id="e0c87-113">string</span><span class="sxs-lookup"><span data-stu-id="e0c87-113">string</span></span>  | <span data-ttu-id="e0c87-114">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="e0c87-114">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="e0c87-115">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="e0c87-115">Helps organize related columns.</span></span>
| <span data-ttu-id="e0c87-116">**description**</span><span class="sxs-lookup"><span data-stu-id="e0c87-116">**description**</span></span>         | <span data-ttu-id="e0c87-117">string</span><span class="sxs-lookup"><span data-stu-id="e0c87-117">string</span></span>  | <span data-ttu-id="e0c87-118">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="e0c87-118">The user-facing description of the column.</span></span>
| <span data-ttu-id="e0c87-119">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e0c87-119">**displayName**</span></span>         | <span data-ttu-id="e0c87-120">строка</span><span class="sxs-lookup"><span data-stu-id="e0c87-120">string</span></span>  | <span data-ttu-id="e0c87-121">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="e0c87-121">The user-facing name of the column.</span></span>
| <span data-ttu-id="e0c87-122">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="e0c87-122">**enforceUniqueValues**</span></span> | <span data-ttu-id="e0c87-123">boolean</span><span class="sxs-lookup"><span data-stu-id="e0c87-123">boolean</span></span> | <span data-ttu-id="e0c87-124">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="e0c87-124">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="e0c87-125">**hidden**</span><span class="sxs-lookup"><span data-stu-id="e0c87-125">**hidden**</span></span>              | <span data-ttu-id="e0c87-126">boolean</span><span class="sxs-lookup"><span data-stu-id="e0c87-126">boolean</span></span> | <span data-ttu-id="e0c87-127">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="e0c87-127">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="e0c87-128">**id**</span><span class="sxs-lookup"><span data-stu-id="e0c87-128">**id**</span></span>                  | <span data-ttu-id="e0c87-129">string</span><span class="sxs-lookup"><span data-stu-id="e0c87-129">string</span></span>  | <span data-ttu-id="e0c87-130">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="e0c87-130">The unique identifier for the column.</span></span>
| <span data-ttu-id="e0c87-131">**indexed**</span><span class="sxs-lookup"><span data-stu-id="e0c87-131">**indexed**</span></span>             | <span data-ttu-id="e0c87-132">boolean</span><span class="sxs-lookup"><span data-stu-id="e0c87-132">boolean</span></span> | <span data-ttu-id="e0c87-133">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="e0c87-133">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="e0c87-134">**name**</span><span class="sxs-lookup"><span data-stu-id="e0c87-134">**name**</span></span>                | <span data-ttu-id="e0c87-135">строка</span><span class="sxs-lookup"><span data-stu-id="e0c87-135">string</span></span>  | <span data-ttu-id="e0c87-136">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="e0c87-136">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="e0c87-137">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="e0c87-137">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="e0c87-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="e0c87-138">**readOnly**</span></span>            | <span data-ttu-id="e0c87-139">логический</span><span class="sxs-lookup"><span data-stu-id="e0c87-139">bool</span></span>    | <span data-ttu-id="e0c87-140">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="e0c87-140">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="e0c87-141">**required**</span><span class="sxs-lookup"><span data-stu-id="e0c87-141">**required**</span></span>            | <span data-ttu-id="e0c87-142">логический</span><span class="sxs-lookup"><span data-stu-id="e0c87-142">boolean</span></span> | <span data-ttu-id="e0c87-143">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="e0c87-143">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="e0c87-144">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e0c87-144">**boolean**</span></span>       | <span data-ttu-id="e0c87-145">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="e0c87-145">[booleanColumn][]</span></span>       | <span data-ttu-id="e0c87-146">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="e0c87-146">This column stores boolean values.</span></span>
| <span data-ttu-id="e0c87-147">**calculated**</span><span class="sxs-lookup"><span data-stu-id="e0c87-147">**calculated**</span></span>    | <span data-ttu-id="e0c87-148">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="e0c87-148">[calculatedColumn][]</span></span>    | <span data-ttu-id="e0c87-149">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="e0c87-149">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="e0c87-150">**choice**</span><span class="sxs-lookup"><span data-stu-id="e0c87-150">**choice**</span></span>        | <span data-ttu-id="e0c87-151">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="e0c87-151">[choiceColumn][]</span></span>        | <span data-ttu-id="e0c87-152">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="e0c87-152">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="e0c87-153">**currency**</span><span class="sxs-lookup"><span data-stu-id="e0c87-153">**currency**</span></span>      | <span data-ttu-id="e0c87-154">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="e0c87-154">[currencyColumn][]</span></span>      | <span data-ttu-id="e0c87-155">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="e0c87-155">This column stores currency values.</span></span>
| <span data-ttu-id="e0c87-156">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="e0c87-156">**dateTime**</span></span>      | <span data-ttu-id="e0c87-157">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="e0c87-157">[dateTimeColumn][]</span></span>      | <span data-ttu-id="e0c87-158">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="e0c87-158">This column stores DateTime values.</span></span>
| <span data-ttu-id="e0c87-159">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="e0c87-159">**defaultValue**</span></span>  | <span data-ttu-id="e0c87-160">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="e0c87-160">[defaultColumnValue][]</span></span>  | <span data-ttu-id="e0c87-161">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="e0c87-161">The default value for this column.</span></span>
| <span data-ttu-id="e0c87-162">Географическое положение</span><span class="sxs-lookup"><span data-stu-id="e0c87-162">**geolocation**</span></span>   | <span data-ttu-id="e0c87-163">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="e0c87-163">[geolocationColumn][]</span></span>   | <span data-ttu-id="e0c87-164">В этом столбце хранятся географического расположения.</span><span class="sxs-lookup"><span data-stu-id="e0c87-164">This column stores a geolocation.</span></span>
| <span data-ttu-id="e0c87-165">**lookup**</span><span class="sxs-lookup"><span data-stu-id="e0c87-165">**lookup**</span></span>        | <span data-ttu-id="e0c87-166">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e0c87-166">[lookupColumn][]</span></span>        | <span data-ttu-id="e0c87-167">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="e0c87-167">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="e0c87-168">**number**</span><span class="sxs-lookup"><span data-stu-id="e0c87-168">**number**</span></span>        | <span data-ttu-id="e0c87-169">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="e0c87-169">[numberColumn][]</span></span>        | <span data-ttu-id="e0c87-170">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="e0c87-170">This column stores number values.</span></span>
| <span data-ttu-id="e0c87-171">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="e0c87-171">**personOrGroup**</span></span> | <span data-ttu-id="e0c87-172">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e0c87-172">[personOrGroupColumn][]</span></span> | <span data-ttu-id="e0c87-173">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="e0c87-173">This column stores Person or Group values.</span></span>
| <span data-ttu-id="e0c87-174">**text**</span><span class="sxs-lookup"><span data-stu-id="e0c87-174">**text**</span></span>          | <span data-ttu-id="e0c87-175">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="e0c87-175">[textColumn][]</span></span>          | <span data-ttu-id="e0c87-176">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="e0c87-176">This column stores text values.</span></span>

><span data-ttu-id="e0c87-177">Примечание. Эти свойства соответствуют перечислению **SPFieldType** в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e0c87-177">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="e0c87-178">Хотя в предыдущей таблице представлены наиболее распространенные типы полей, бета-версии API по-прежнему отсутствует некоторые.</span><span class="sxs-lookup"><span data-stu-id="e0c87-178">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="e0c87-179">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="e0c87-179">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="e0c87-180">Примечания</span><span class="sxs-lookup"><span data-stu-id="e0c87-180">Remarks</span></span>

<span data-ttu-id="e0c87-181">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="e0c87-181">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="e0c87-182">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="e0c87-182">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="e0c87-183">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="e0c87-183">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
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
