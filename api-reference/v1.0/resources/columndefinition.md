---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 96587cc1b3badf2d5fcc90bc7c1d2b1cfb710f6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025273"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="90827-102">Ресурс ColumnDefinition</span><span class="sxs-lookup"><span data-stu-id="90827-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="90827-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="90827-103">JSON representation</span></span>

<span data-ttu-id="90827-104">Ниже показано представление ресурса ColumnDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90827-104">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="90827-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="90827-105">Properties</span></span>

<span data-ttu-id="90827-106">Ниже перечислены свойства ресурса **columnDefinition**.</span><span class="sxs-lookup"><span data-stu-id="90827-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="90827-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="90827-107">Property name</span></span>           | <span data-ttu-id="90827-108">Тип</span><span class="sxs-lookup"><span data-stu-id="90827-108">Type</span></span>    | <span data-ttu-id="90827-109">Описание</span><span class="sxs-lookup"><span data-stu-id="90827-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="90827-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="90827-110">**columnGroup**</span></span>         | <span data-ttu-id="90827-111">строка</span><span class="sxs-lookup"><span data-stu-id="90827-111">string</span></span>  | <span data-ttu-id="90827-112">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="90827-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="90827-113">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="90827-113">Helps organize related columns.</span></span>
| <span data-ttu-id="90827-114">**description**</span><span class="sxs-lookup"><span data-stu-id="90827-114">**description**</span></span>         | <span data-ttu-id="90827-115">строка</span><span class="sxs-lookup"><span data-stu-id="90827-115">string</span></span>  | <span data-ttu-id="90827-116">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="90827-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="90827-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="90827-117">**displayName**</span></span>         | <span data-ttu-id="90827-118">строка</span><span class="sxs-lookup"><span data-stu-id="90827-118">string</span></span>  | <span data-ttu-id="90827-119">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="90827-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="90827-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="90827-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="90827-121">логический</span><span class="sxs-lookup"><span data-stu-id="90827-121">boolean</span></span> | <span data-ttu-id="90827-122">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="90827-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="90827-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="90827-123">**hidden**</span></span>              | <span data-ttu-id="90827-124">логический</span><span class="sxs-lookup"><span data-stu-id="90827-124">boolean</span></span> | <span data-ttu-id="90827-125">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="90827-125">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="90827-126">**id**</span><span class="sxs-lookup"><span data-stu-id="90827-126">**id**</span></span>                  | <span data-ttu-id="90827-127">строка</span><span class="sxs-lookup"><span data-stu-id="90827-127">string</span></span>  | <span data-ttu-id="90827-128">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="90827-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="90827-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="90827-129">**indexed**</span></span>             | <span data-ttu-id="90827-130">логический</span><span class="sxs-lookup"><span data-stu-id="90827-130">boolean</span></span> | <span data-ttu-id="90827-131">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="90827-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="90827-132">**name**</span><span class="sxs-lookup"><span data-stu-id="90827-132">**name**</span></span>                | <span data-ttu-id="90827-133">строка</span><span class="sxs-lookup"><span data-stu-id="90827-133">string</span></span>  | <span data-ttu-id="90827-134">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="90827-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="90827-135">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="90827-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="90827-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="90827-136">**readOnly**</span></span>            | <span data-ttu-id="90827-137">логический</span><span class="sxs-lookup"><span data-stu-id="90827-137">bool</span></span>    | <span data-ttu-id="90827-138">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="90827-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="90827-139">**required**</span><span class="sxs-lookup"><span data-stu-id="90827-139">**required**</span></span>            | <span data-ttu-id="90827-140">логический</span><span class="sxs-lookup"><span data-stu-id="90827-140">boolean</span></span> | <span data-ttu-id="90827-141">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="90827-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="90827-142">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="90827-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="90827-143">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="90827-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="90827-144">Эти свойства являются взаимоисключающими. Для столбца можно указать только одно из них.</span><span class="sxs-lookup"><span data-stu-id="90827-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="90827-145">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="90827-145">Property name</span></span>     | <span data-ttu-id="90827-146">Тип</span><span class="sxs-lookup"><span data-stu-id="90827-146">Type</span></span>                    | <span data-ttu-id="90827-147">Описание</span><span class="sxs-lookup"><span data-stu-id="90827-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="90827-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="90827-148">**boolean**</span></span>       | <span data-ttu-id="90827-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="90827-149">[booleanColumn][]</span></span>       | <span data-ttu-id="90827-150">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="90827-150">This column stores boolean values.</span></span>
| <span data-ttu-id="90827-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="90827-151">**calculated**</span></span>    | <span data-ttu-id="90827-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="90827-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="90827-153">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="90827-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="90827-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="90827-154">**choice**</span></span>        | <span data-ttu-id="90827-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="90827-155">[choiceColumn][]</span></span>        | <span data-ttu-id="90827-156">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="90827-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="90827-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="90827-157">**currency**</span></span>      | <span data-ttu-id="90827-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="90827-158">[currencyColumn][]</span></span>      | <span data-ttu-id="90827-159">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="90827-159">This column stores currency values.</span></span>
| <span data-ttu-id="90827-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="90827-160">**dateTime**</span></span>      | <span data-ttu-id="90827-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="90827-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="90827-162">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="90827-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="90827-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="90827-163">**defaultValue**</span></span>  | <span data-ttu-id="90827-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="90827-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="90827-165">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="90827-165">The default value for this column.</span></span>
| <span data-ttu-id="90827-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="90827-166">**lookup**</span></span>        | <span data-ttu-id="90827-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="90827-167">[lookupColumn][]</span></span>        | <span data-ttu-id="90827-168">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="90827-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="90827-169">**number**</span><span class="sxs-lookup"><span data-stu-id="90827-169">**number**</span></span>        | <span data-ttu-id="90827-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="90827-170">[numberColumn][]</span></span>        | <span data-ttu-id="90827-171">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="90827-171">This column stores number values.</span></span>
| <span data-ttu-id="90827-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="90827-172">**personOrGroup**</span></span> | <span data-ttu-id="90827-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="90827-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="90827-174">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="90827-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="90827-175">**text**</span><span class="sxs-lookup"><span data-stu-id="90827-175">**text**</span></span>          | <span data-ttu-id="90827-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="90827-176">[textColumn][]</span></span>          | <span data-ttu-id="90827-177">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="90827-177">This column stores text values.</span></span>

<span data-ttu-id="90827-178">Примечание. Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="90827-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="90827-179">Во время наиболее распространенные типы полей, представленные выше, этот интерфейс API не пропущены некоторые.</span><span class="sxs-lookup"><span data-stu-id="90827-179">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="90827-180">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="90827-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="90827-181">Примечания</span><span class="sxs-lookup"><span data-stu-id="90827-181">Remarks</span></span>

<span data-ttu-id="90827-182">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="90827-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="90827-183">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="90827-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="90827-184">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="90827-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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
