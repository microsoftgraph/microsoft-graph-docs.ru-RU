---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: 5db835b9720f9fa711d683dd505e8325b27d79d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844494"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="3a838-102">Тип ресурса columnDefinition</span><span class="sxs-lookup"><span data-stu-id="3a838-102">columnDefinition resource type</span></span>

> <span data-ttu-id="3a838-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a838-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a838-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a838-104">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a838-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a838-105">JSON representation</span></span>

<span data-ttu-id="3a838-106">Ниже представлена JSON columnDefinition ресурса.</span><span class="sxs-lookup"><span data-stu-id="3a838-106">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3a838-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a838-107">Properties</span></span>

<span data-ttu-id="3a838-108">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="3a838-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="3a838-109">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="3a838-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="3a838-110">Тип свойства, связанные с (типа boolean, вычисляемых, выбор, валюты, даты и времени, подстановки, номер, personOrGroup, текст) являются взаимоисключающими (столбец может иметь только один из них указан).</span><span class="sxs-lookup"><span data-stu-id="3a838-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="3a838-111">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="3a838-111">Property name</span></span>           | <span data-ttu-id="3a838-112">Тип</span><span class="sxs-lookup"><span data-stu-id="3a838-112">Type</span></span>    | <span data-ttu-id="3a838-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3a838-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="3a838-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="3a838-114">**columnGroup**</span></span>         | <span data-ttu-id="3a838-115">строка</span><span class="sxs-lookup"><span data-stu-id="3a838-115">string</span></span>  | <span data-ttu-id="3a838-116">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="3a838-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="3a838-117">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="3a838-117">Helps organize related columns.</span></span>
| <span data-ttu-id="3a838-118">**description**</span><span class="sxs-lookup"><span data-stu-id="3a838-118">**description**</span></span>         | <span data-ttu-id="3a838-119">строка</span><span class="sxs-lookup"><span data-stu-id="3a838-119">string</span></span>  | <span data-ttu-id="3a838-120">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="3a838-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="3a838-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="3a838-121">**displayName**</span></span>         | <span data-ttu-id="3a838-122">строка</span><span class="sxs-lookup"><span data-stu-id="3a838-122">string</span></span>  | <span data-ttu-id="3a838-123">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="3a838-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="3a838-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="3a838-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="3a838-125">логический</span><span class="sxs-lookup"><span data-stu-id="3a838-125">boolean</span></span> | <span data-ttu-id="3a838-126">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="3a838-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="3a838-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="3a838-127">**hidden**</span></span>              | <span data-ttu-id="3a838-128">логический</span><span class="sxs-lookup"><span data-stu-id="3a838-128">boolean</span></span> | <span data-ttu-id="3a838-129">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="3a838-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="3a838-130">**id**</span><span class="sxs-lookup"><span data-stu-id="3a838-130">**id**</span></span>                  | <span data-ttu-id="3a838-131">строка</span><span class="sxs-lookup"><span data-stu-id="3a838-131">string</span></span>  | <span data-ttu-id="3a838-132">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="3a838-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="3a838-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="3a838-133">**indexed**</span></span>             | <span data-ttu-id="3a838-134">логический</span><span class="sxs-lookup"><span data-stu-id="3a838-134">boolean</span></span> | <span data-ttu-id="3a838-135">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="3a838-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="3a838-136">**name**</span><span class="sxs-lookup"><span data-stu-id="3a838-136">**name**</span></span>                | <span data-ttu-id="3a838-137">строка</span><span class="sxs-lookup"><span data-stu-id="3a838-137">string</span></span>  | <span data-ttu-id="3a838-138">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="3a838-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="3a838-139">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="3a838-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="3a838-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="3a838-140">**readOnly**</span></span>            | <span data-ttu-id="3a838-141">логический</span><span class="sxs-lookup"><span data-stu-id="3a838-141">bool</span></span>    | <span data-ttu-id="3a838-142">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="3a838-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="3a838-143">**required**</span><span class="sxs-lookup"><span data-stu-id="3a838-143">**required**</span></span>            | <span data-ttu-id="3a838-144">логический</span><span class="sxs-lookup"><span data-stu-id="3a838-144">boolean</span></span> | <span data-ttu-id="3a838-145">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="3a838-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="3a838-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="3a838-146">**boolean**</span></span>       | <span data-ttu-id="3a838-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="3a838-147">[booleanColumn][]</span></span>       | <span data-ttu-id="3a838-148">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="3a838-148">This column stores boolean values.</span></span>
| <span data-ttu-id="3a838-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="3a838-149">**calculated**</span></span>    | <span data-ttu-id="3a838-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="3a838-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="3a838-151">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="3a838-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="3a838-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="3a838-152">**choice**</span></span>        | <span data-ttu-id="3a838-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="3a838-153">[choiceColumn][]</span></span>        | <span data-ttu-id="3a838-154">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="3a838-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="3a838-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="3a838-155">**currency**</span></span>      | <span data-ttu-id="3a838-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="3a838-156">[currencyColumn][]</span></span>      | <span data-ttu-id="3a838-157">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="3a838-157">This column stores currency values.</span></span>
| <span data-ttu-id="3a838-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="3a838-158">**dateTime**</span></span>      | <span data-ttu-id="3a838-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="3a838-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="3a838-160">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="3a838-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="3a838-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="3a838-161">**defaultValue**</span></span>  | <span data-ttu-id="3a838-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="3a838-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="3a838-163">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="3a838-163">The default value for this column.</span></span>
| <span data-ttu-id="3a838-164">**географическое положение**</span><span class="sxs-lookup"><span data-stu-id="3a838-164">**geolocation**</span></span>   | <span data-ttu-id="3a838-165">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="3a838-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="3a838-166">В этом столбце хранятся географического расположения.</span><span class="sxs-lookup"><span data-stu-id="3a838-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="3a838-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="3a838-167">**lookup**</span></span>        | <span data-ttu-id="3a838-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="3a838-168">[lookupColumn][]</span></span>        | <span data-ttu-id="3a838-169">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="3a838-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="3a838-170">**number**</span><span class="sxs-lookup"><span data-stu-id="3a838-170">**number**</span></span>        | <span data-ttu-id="3a838-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="3a838-171">[numberColumn][]</span></span>        | <span data-ttu-id="3a838-172">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="3a838-172">This column stores number values.</span></span>
| <span data-ttu-id="3a838-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="3a838-173">**personOrGroup**</span></span> | <span data-ttu-id="3a838-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="3a838-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="3a838-175">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="3a838-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="3a838-176">**text**</span><span class="sxs-lookup"><span data-stu-id="3a838-176">**text**</span></span>          | <span data-ttu-id="3a838-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="3a838-177">[textColumn][]</span></span>          | <span data-ttu-id="3a838-178">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="3a838-178">This column stores text values.</span></span>

><span data-ttu-id="3a838-179">**Примечание:** Эти свойства соответствуют перечисление [SPFieldType][] SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3a838-179">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="3a838-180">Хотя в предыдущей таблице представлены наиболее распространенные типы полей, бета-версии API по-прежнему отсутствует некоторые.</span><span class="sxs-lookup"><span data-stu-id="3a838-180">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="3a838-181">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="3a838-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="3a838-182">Примечания</span><span class="sxs-lookup"><span data-stu-id="3a838-182">Remarks</span></span>

<span data-ttu-id="3a838-183">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="3a838-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="3a838-184">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="3a838-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="3a838-185">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="3a838-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
