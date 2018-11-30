---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 9b99abe78b009786d489ec7f0c0fdce1e2945b1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074945"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="ce7ed-102">Тип ресурса columnDefinition</span><span class="sxs-lookup"><span data-stu-id="ce7ed-102">columnDefinition resource type</span></span>

> <span data-ttu-id="ce7ed-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce7ed-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-104">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce7ed-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce7ed-105">JSON representation</span></span>

<span data-ttu-id="ce7ed-106">Ниже представлена JSON columnDefinition ресурса.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-106">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ce7ed-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce7ed-107">Properties</span></span>

<span data-ttu-id="ce7ed-108">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="ce7ed-109">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="ce7ed-110">Тип свойства, связанные с (типа boolean, вычисляемых, выбор, валюты, даты и времени, подстановки, номер, personOrGroup, текст) являются взаимоисключающими (столбец может иметь только один из них указан).</span><span class="sxs-lookup"><span data-stu-id="ce7ed-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="ce7ed-111">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ce7ed-111">Property name</span></span>           | <span data-ttu-id="ce7ed-112">Тип</span><span class="sxs-lookup"><span data-stu-id="ce7ed-112">Type</span></span>    | <span data-ttu-id="ce7ed-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ce7ed-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="ce7ed-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-114">**columnGroup**</span></span>         | <span data-ttu-id="ce7ed-115">строка</span><span class="sxs-lookup"><span data-stu-id="ce7ed-115">string</span></span>  | <span data-ttu-id="ce7ed-116">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="ce7ed-117">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-117">Helps organize related columns.</span></span>
| <span data-ttu-id="ce7ed-118">**description**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-118">**description**</span></span>         | <span data-ttu-id="ce7ed-119">строка</span><span class="sxs-lookup"><span data-stu-id="ce7ed-119">string</span></span>  | <span data-ttu-id="ce7ed-120">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="ce7ed-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-121">**displayName**</span></span>         | <span data-ttu-id="ce7ed-122">строка</span><span class="sxs-lookup"><span data-stu-id="ce7ed-122">string</span></span>  | <span data-ttu-id="ce7ed-123">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="ce7ed-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="ce7ed-125">логический</span><span class="sxs-lookup"><span data-stu-id="ce7ed-125">boolean</span></span> | <span data-ttu-id="ce7ed-126">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="ce7ed-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-127">**hidden**</span></span>              | <span data-ttu-id="ce7ed-128">логический</span><span class="sxs-lookup"><span data-stu-id="ce7ed-128">boolean</span></span> | <span data-ttu-id="ce7ed-129">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="ce7ed-130">**id**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-130">**id**</span></span>                  | <span data-ttu-id="ce7ed-131">строка</span><span class="sxs-lookup"><span data-stu-id="ce7ed-131">string</span></span>  | <span data-ttu-id="ce7ed-132">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="ce7ed-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-133">**indexed**</span></span>             | <span data-ttu-id="ce7ed-134">логический</span><span class="sxs-lookup"><span data-stu-id="ce7ed-134">boolean</span></span> | <span data-ttu-id="ce7ed-135">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="ce7ed-136">**name**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-136">**name**</span></span>                | <span data-ttu-id="ce7ed-137">строка</span><span class="sxs-lookup"><span data-stu-id="ce7ed-137">string</span></span>  | <span data-ttu-id="ce7ed-138">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="ce7ed-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="ce7ed-139">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="ce7ed-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-140">**readOnly**</span></span>            | <span data-ttu-id="ce7ed-141">bool</span><span class="sxs-lookup"><span data-stu-id="ce7ed-141">bool</span></span>    | <span data-ttu-id="ce7ed-142">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="ce7ed-143">**required**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-143">**required**</span></span>            | <span data-ttu-id="ce7ed-144">логический</span><span class="sxs-lookup"><span data-stu-id="ce7ed-144">boolean</span></span> | <span data-ttu-id="ce7ed-145">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="ce7ed-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-146">**boolean**</span></span>       | <span data-ttu-id="ce7ed-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="ce7ed-147">[booleanColumn][]</span></span>       | <span data-ttu-id="ce7ed-148">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-148">This column stores boolean values.</span></span>
| <span data-ttu-id="ce7ed-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-149">**calculated**</span></span>    | <span data-ttu-id="ce7ed-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="ce7ed-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="ce7ed-151">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="ce7ed-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-152">**choice**</span></span>        | <span data-ttu-id="ce7ed-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="ce7ed-153">[choiceColumn][]</span></span>        | <span data-ttu-id="ce7ed-154">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="ce7ed-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-155">**currency**</span></span>      | <span data-ttu-id="ce7ed-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="ce7ed-156">[currencyColumn][]</span></span>      | <span data-ttu-id="ce7ed-157">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-157">This column stores currency values.</span></span>
| <span data-ttu-id="ce7ed-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-158">**dateTime**</span></span>      | <span data-ttu-id="ce7ed-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="ce7ed-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="ce7ed-160">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="ce7ed-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-161">**defaultValue**</span></span>  | <span data-ttu-id="ce7ed-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="ce7ed-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="ce7ed-163">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-163">The default value for this column.</span></span>
| <span data-ttu-id="ce7ed-164">**географическое положение**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-164">**geolocation**</span></span>   | <span data-ttu-id="ce7ed-165">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="ce7ed-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="ce7ed-166">В этом столбце хранятся географического расположения.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="ce7ed-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-167">**lookup**</span></span>        | <span data-ttu-id="ce7ed-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="ce7ed-168">[lookupColumn][]</span></span>        | <span data-ttu-id="ce7ed-169">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="ce7ed-170">**number**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-170">**number**</span></span>        | <span data-ttu-id="ce7ed-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="ce7ed-171">[numberColumn][]</span></span>        | <span data-ttu-id="ce7ed-172">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-172">This column stores number values.</span></span>
| <span data-ttu-id="ce7ed-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-173">**personOrGroup**</span></span> | <span data-ttu-id="ce7ed-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="ce7ed-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="ce7ed-175">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="ce7ed-176">**text**</span><span class="sxs-lookup"><span data-stu-id="ce7ed-176">**text**</span></span>          | <span data-ttu-id="ce7ed-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="ce7ed-177">[textColumn][]</span></span>          | <span data-ttu-id="ce7ed-178">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-178">This column stores text values.</span></span>

><span data-ttu-id="ce7ed-179">**Примечание:** Эти свойства соответствуют перечисление [SPFieldType][] SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-179">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="ce7ed-180">Хотя в предыдущей таблице представлены наиболее распространенные типы полей, бета-версии API по-прежнему отсутствует некоторые.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-180">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="ce7ed-181">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="ce7ed-182">Примечания</span><span class="sxs-lookup"><span data-stu-id="ce7ed-182">Remarks</span></span>

<span data-ttu-id="ce7ed-183">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="ce7ed-184">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="ce7ed-185">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="ce7ed-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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
