---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: e5942ddee4b505243cb64121862ce9e89e52d245
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="columndefinition-resource"></a><span data-ttu-id="05ea6-102">Ресурс ColumnDefinition</span><span class="sxs-lookup"><span data-stu-id="05ea6-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="05ea6-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="05ea6-103">JSON representation</span></span>

<span data-ttu-id="05ea6-104">Ниже показано представление ресурса ColumnDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05ea6-104">Here is a JSON representation of a {type} resource.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnDefinition",
       "keyProperty": "id", "optionalProperties": [ ] } -->

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

## <a name="properties"></a><span data-ttu-id="05ea6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="05ea6-105">Properties</span></span>

<span data-ttu-id="05ea6-106">Ниже перечислены свойства ресурса **columnDefinition**.</span><span class="sxs-lookup"><span data-stu-id="05ea6-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="05ea6-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="05ea6-107">Property name</span></span>           | <span data-ttu-id="05ea6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="05ea6-108">Type</span></span>    | <span data-ttu-id="05ea6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="05ea6-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="05ea6-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="05ea6-110">**columnGroup**</span></span>         | <span data-ttu-id="05ea6-111">строка</span><span class="sxs-lookup"><span data-stu-id="05ea6-111">string</span></span>  | <span data-ttu-id="05ea6-112">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="05ea6-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="05ea6-113">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="05ea6-113">Helps organize related columns.</span></span>
| <span data-ttu-id="05ea6-114">**description**</span><span class="sxs-lookup"><span data-stu-id="05ea6-114">**description**</span></span>         | <span data-ttu-id="05ea6-115">строка</span><span class="sxs-lookup"><span data-stu-id="05ea6-115">string</span></span>  | <span data-ttu-id="05ea6-116">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="05ea6-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="05ea6-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="05ea6-117">**displayName**</span></span>         | <span data-ttu-id="05ea6-118">строка</span><span class="sxs-lookup"><span data-stu-id="05ea6-118">string</span></span>  | <span data-ttu-id="05ea6-119">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="05ea6-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="05ea6-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="05ea6-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="05ea6-121">логический</span><span class="sxs-lookup"><span data-stu-id="05ea6-121">boolean</span></span> | <span data-ttu-id="05ea6-122">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="05ea6-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="05ea6-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="05ea6-123">**hidden**</span></span>              | <span data-ttu-id="05ea6-124">логический</span><span class="sxs-lookup"><span data-stu-id="05ea6-124">boolean</span></span> | <span data-ttu-id="05ea6-125">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="05ea6-125">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="05ea6-126">**id**</span><span class="sxs-lookup"><span data-stu-id="05ea6-126">**id**</span></span>                  | <span data-ttu-id="05ea6-127">строка</span><span class="sxs-lookup"><span data-stu-id="05ea6-127">string</span></span>  | <span data-ttu-id="05ea6-128">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="05ea6-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="05ea6-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="05ea6-129">**Indexed**</span></span>             | <span data-ttu-id="05ea6-130">логический</span><span class="sxs-lookup"><span data-stu-id="05ea6-130">boolean</span></span> | <span data-ttu-id="05ea6-131">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="05ea6-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="05ea6-132">**name**</span><span class="sxs-lookup"><span data-stu-id="05ea6-132">**name**</span></span>                | <span data-ttu-id="05ea6-133">строка</span><span class="sxs-lookup"><span data-stu-id="05ea6-133">string</span></span>  | <span data-ttu-id="05ea6-134">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="05ea6-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="05ea6-135">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="05ea6-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="05ea6-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="05ea6-136">**Read-only.**</span></span>            | <span data-ttu-id="05ea6-137">логический</span><span class="sxs-lookup"><span data-stu-id="05ea6-137">bool</span></span>    | <span data-ttu-id="05ea6-138">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="05ea6-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="05ea6-139">**required**</span><span class="sxs-lookup"><span data-stu-id="05ea6-139">**Required**</span></span>            | <span data-ttu-id="05ea6-140">логический</span><span class="sxs-lookup"><span data-stu-id="05ea6-140">boolean</span></span> | <span data-ttu-id="05ea6-141">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="05ea6-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="05ea6-142">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="05ea6-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="05ea6-143">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="05ea6-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="05ea6-144">Эти свойства являются взаимоисключающими. Для столбца можно указать только одно из них.</span><span class="sxs-lookup"><span data-stu-id="05ea6-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="05ea6-145">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="05ea6-145">Property name</span></span>     | <span data-ttu-id="05ea6-146">Тип</span><span class="sxs-lookup"><span data-stu-id="05ea6-146">Type</span></span>                    | <span data-ttu-id="05ea6-147">Описание</span><span class="sxs-lookup"><span data-stu-id="05ea6-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="05ea6-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="05ea6-148">**Boolean**</span></span>       | <span data-ttu-id="05ea6-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="05ea6-149">[booleanColumn][]</span></span>       | <span data-ttu-id="05ea6-150">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="05ea6-150">This column stores boolean values.</span></span>
| <span data-ttu-id="05ea6-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="05ea6-151">**Calculated**</span></span>    | <span data-ttu-id="05ea6-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="05ea6-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="05ea6-153">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="05ea6-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="05ea6-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="05ea6-154">**Choice**</span></span>        | <span data-ttu-id="05ea6-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="05ea6-155">[choiceColumn][]</span></span>        | <span data-ttu-id="05ea6-156">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="05ea6-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="05ea6-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="05ea6-157">**Currency**</span></span>      | <span data-ttu-id="05ea6-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="05ea6-158">[currencyColumn][]</span></span>      | <span data-ttu-id="05ea6-159">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="05ea6-159">This column stores currency values.</span></span>
| <span data-ttu-id="05ea6-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="05ea6-160">**Date/Time**</span></span>      | <span data-ttu-id="05ea6-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="05ea6-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="05ea6-162">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="05ea6-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="05ea6-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="05ea6-163">**DefaultValue**</span></span>  | <span data-ttu-id="05ea6-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="05ea6-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="05ea6-165">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="05ea6-165">The default value for this column.</span></span>
| <span data-ttu-id="05ea6-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="05ea6-166">**Lookup**</span></span>        | <span data-ttu-id="05ea6-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="05ea6-167">[lookupColumn][]</span></span>        | <span data-ttu-id="05ea6-168">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="05ea6-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="05ea6-169">**number**</span><span class="sxs-lookup"><span data-stu-id="05ea6-169">**number**</span></span>        | <span data-ttu-id="05ea6-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="05ea6-170">[numberColumn][]</span></span>        | <span data-ttu-id="05ea6-171">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="05ea6-171">This column stores number values.</span></span>
| <span data-ttu-id="05ea6-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="05ea6-172">**personOrGroup**</span></span> | <span data-ttu-id="05ea6-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="05ea6-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="05ea6-174">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="05ea6-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="05ea6-175">**text**</span><span class="sxs-lookup"><span data-stu-id="05ea6-175">**text**</span></span>          | <span data-ttu-id="05ea6-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="05ea6-176">[textColumn][]</span></span>          | <span data-ttu-id="05ea6-177">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="05ea6-177">This column stores text values.</span></span>

<span data-ttu-id="05ea6-178">Примечание. Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="05ea6-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="05ea6-179">Выше перечислены наиболее распространенные типы полей, но в бета-версии API по-прежнему не хватает некоторых типов.</span><span class="sxs-lookup"><span data-stu-id="05ea6-179">While the most common field types are represented above, this beta API is still missing some.</span></span>
<span data-ttu-id="05ea6-180">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="05ea6-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="05ea6-181">Примечания</span><span class="sxs-lookup"><span data-stu-id="05ea6-181">Remarks</span></span>

<span data-ttu-id="05ea6-182">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="05ea6-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="05ea6-183">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="05ea6-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="05ea6-184">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="05ea6-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleanColumn.md
[calculatedColumn]: calculatedColumn.md
[choiceColumn]: choiceColumn.md
[currencyColumn]: currencyColumn.md
[dateTimeColumn]: dateTimeColumn.md
[defaultColumnValue]: defaultColumnValue.md
[lookupColumn]: lookupColumn.md
[numberColumn]: numberColumn.md
[personOrGroupColumn]: personOrGroupColumn.md
[textColumn]: textColumn.md
[fieldValueSet]: fieldValueSet.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/en-us/library/microsoft.sharepoint.spfieldtype.aspx

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
