---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
description: Ниже показано представление ресурса ColumnDefinition в формате JSON.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3a02721c5289b1d49077e1b2d9fa1017f0c53021
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032874"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="c7cf0-103">Ресурс ColumnDefinition</span><span class="sxs-lookup"><span data-stu-id="c7cf0-103">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7cf0-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c7cf0-104">JSON representation</span></span>

<span data-ttu-id="c7cf0-105">Ниже показано представление ресурса ColumnDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-105">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="c7cf0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7cf0-106">Properties</span></span>

<span data-ttu-id="c7cf0-107">Ниже перечислены свойства ресурса **columnDefinition**.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-107">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="c7cf0-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c7cf0-108">Property name</span></span>           | <span data-ttu-id="c7cf0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c7cf0-109">Type</span></span>    | <span data-ttu-id="c7cf0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c7cf0-110">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="c7cf0-111">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-111">**columnGroup**</span></span>         | <span data-ttu-id="c7cf0-112">строка</span><span class="sxs-lookup"><span data-stu-id="c7cf0-112">string</span></span>  | <span data-ttu-id="c7cf0-113">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-113">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="c7cf0-114">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-114">Helps organize related columns.</span></span>
| <span data-ttu-id="c7cf0-115">**description**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-115">**description**</span></span>         | <span data-ttu-id="c7cf0-116">строка</span><span class="sxs-lookup"><span data-stu-id="c7cf0-116">string</span></span>  | <span data-ttu-id="c7cf0-117">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-117">The user-facing description of the column.</span></span>
| <span data-ttu-id="c7cf0-118">**displayName**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-118">**displayName**</span></span>         | <span data-ttu-id="c7cf0-119">string</span><span class="sxs-lookup"><span data-stu-id="c7cf0-119">string</span></span>  | <span data-ttu-id="c7cf0-120">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-120">The user-facing name of the column.</span></span>
| <span data-ttu-id="c7cf0-121">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-121">**enforceUniqueValues**</span></span> | <span data-ttu-id="c7cf0-122">boolean</span><span class="sxs-lookup"><span data-stu-id="c7cf0-122">boolean</span></span> | <span data-ttu-id="c7cf0-123">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-123">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="c7cf0-124">**hidden**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-124">**hidden**</span></span>              | <span data-ttu-id="c7cf0-125">boolean</span><span class="sxs-lookup"><span data-stu-id="c7cf0-125">boolean</span></span> | <span data-ttu-id="c7cf0-126">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-126">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="c7cf0-127">**id**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-127">**id**</span></span>                  | <span data-ttu-id="c7cf0-128">string</span><span class="sxs-lookup"><span data-stu-id="c7cf0-128">string</span></span>  | <span data-ttu-id="c7cf0-129">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-129">The unique identifier for the column.</span></span>
| <span data-ttu-id="c7cf0-130">**indexed**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-130">**indexed**</span></span>             | <span data-ttu-id="c7cf0-131">boolean</span><span class="sxs-lookup"><span data-stu-id="c7cf0-131">boolean</span></span> | <span data-ttu-id="c7cf0-132">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-132">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="c7cf0-133">**name**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-133">**name**</span></span>                | <span data-ttu-id="c7cf0-134">string</span><span class="sxs-lookup"><span data-stu-id="c7cf0-134">string</span></span>  | <span data-ttu-id="c7cf0-135">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="c7cf0-135">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="c7cf0-136">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-136">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="c7cf0-137">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-137">**readOnly**</span></span>            | <span data-ttu-id="c7cf0-138">логический</span><span class="sxs-lookup"><span data-stu-id="c7cf0-138">bool</span></span>    | <span data-ttu-id="c7cf0-139">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-139">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="c7cf0-140">**required**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-140">**required**</span></span>            | <span data-ttu-id="c7cf0-141">логический</span><span class="sxs-lookup"><span data-stu-id="c7cf0-141">boolean</span></span> | <span data-ttu-id="c7cf0-142">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-142">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="c7cf0-143">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-143">Columns can hold data of various types.</span></span>
<span data-ttu-id="c7cf0-144">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-144">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="c7cf0-145">Эти свойства являются взаимоисключающими. Для столбца можно указать только одно из них.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-145">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="c7cf0-146">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c7cf0-146">Property name</span></span>     | <span data-ttu-id="c7cf0-147">Тип</span><span class="sxs-lookup"><span data-stu-id="c7cf0-147">Type</span></span>                    | <span data-ttu-id="c7cf0-148">Описание</span><span class="sxs-lookup"><span data-stu-id="c7cf0-148">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="c7cf0-149">**boolean**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-149">**boolean**</span></span>       | <span data-ttu-id="c7cf0-150">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="c7cf0-150">[booleanColumn][]</span></span>       | <span data-ttu-id="c7cf0-151">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-151">This column stores boolean values.</span></span>
| <span data-ttu-id="c7cf0-152">**calculated**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-152">**calculated**</span></span>    | <span data-ttu-id="c7cf0-153">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="c7cf0-153">[calculatedColumn][]</span></span>    | <span data-ttu-id="c7cf0-154">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-154">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="c7cf0-155">**choice**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-155">**choice**</span></span>        | <span data-ttu-id="c7cf0-156">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="c7cf0-156">[choiceColumn][]</span></span>        | <span data-ttu-id="c7cf0-157">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-157">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="c7cf0-158">**currency**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-158">**currency**</span></span>      | <span data-ttu-id="c7cf0-159">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="c7cf0-159">[currencyColumn][]</span></span>      | <span data-ttu-id="c7cf0-160">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-160">This column stores currency values.</span></span>
| <span data-ttu-id="c7cf0-161">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-161">**dateTime**</span></span>      | <span data-ttu-id="c7cf0-162">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="c7cf0-162">[dateTimeColumn][]</span></span>      | <span data-ttu-id="c7cf0-163">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-163">This column stores DateTime values.</span></span>
| <span data-ttu-id="c7cf0-164">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-164">**defaultValue**</span></span>  | <span data-ttu-id="c7cf0-165">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="c7cf0-165">[defaultColumnValue][]</span></span>  | <span data-ttu-id="c7cf0-166">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-166">The default value for this column.</span></span>
| <span data-ttu-id="c7cf0-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-167">**lookup**</span></span>        | <span data-ttu-id="c7cf0-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="c7cf0-168">[lookupColumn][]</span></span>        | <span data-ttu-id="c7cf0-169">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="c7cf0-170">**number**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-170">**number**</span></span>        | <span data-ttu-id="c7cf0-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="c7cf0-171">[numberColumn][]</span></span>        | <span data-ttu-id="c7cf0-172">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-172">This column stores number values.</span></span>
| <span data-ttu-id="c7cf0-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-173">**personOrGroup**</span></span> | <span data-ttu-id="c7cf0-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="c7cf0-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="c7cf0-175">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="c7cf0-176">**text**</span><span class="sxs-lookup"><span data-stu-id="c7cf0-176">**text**</span></span>          | <span data-ttu-id="c7cf0-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="c7cf0-177">[textColumn][]</span></span>          | <span data-ttu-id="c7cf0-178">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-178">This column stores text values.</span></span>

<span data-ttu-id="c7cf0-179">Примечание. Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-179">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="c7cf0-180">Хотя наиболее распространенные типы полей представлены выше, этот API все еще не содержит.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-180">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="c7cf0-181">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="c7cf0-182">Примечания</span><span class="sxs-lookup"><span data-stu-id="c7cf0-182">Remarks</span></span>

<span data-ttu-id="c7cf0-183">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="c7cf0-184">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="c7cf0-185">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="c7cf0-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
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
