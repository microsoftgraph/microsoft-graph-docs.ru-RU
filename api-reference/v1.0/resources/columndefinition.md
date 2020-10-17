---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
description: Ниже показано представление ресурса ColumnDefinition в формате JSON.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aae4b71055c7a6574cc4abbaa506fad8961991d9
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581228"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="dc689-103">Ресурс ColumnDefinition</span><span class="sxs-lookup"><span data-stu-id="dc689-103">ColumnDefinition resource</span></span>

<span data-ttu-id="dc689-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc689-104">Namespace: microsoft.graph</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc689-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dc689-105">JSON representation</span></span>

<span data-ttu-id="dc689-106">Ниже показано представление ресурса ColumnDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc689-106">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dc689-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc689-107">Properties</span></span>

<span data-ttu-id="dc689-108">Ниже перечислены свойства ресурса **columnDefinition**.</span><span class="sxs-lookup"><span data-stu-id="dc689-108">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="dc689-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dc689-109">Property name</span></span>           | <span data-ttu-id="dc689-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dc689-110">Type</span></span>    | <span data-ttu-id="dc689-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dc689-111">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="dc689-112">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="dc689-112">**columnGroup**</span></span>         | <span data-ttu-id="dc689-113">строка</span><span class="sxs-lookup"><span data-stu-id="dc689-113">string</span></span>  | <span data-ttu-id="dc689-114">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="dc689-114">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="dc689-115">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="dc689-115">Helps organize related columns.</span></span>
| <span data-ttu-id="dc689-116">**description**</span><span class="sxs-lookup"><span data-stu-id="dc689-116">**description**</span></span>         | <span data-ttu-id="dc689-117">string</span><span class="sxs-lookup"><span data-stu-id="dc689-117">string</span></span>  | <span data-ttu-id="dc689-118">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="dc689-118">The user-facing description of the column.</span></span>
| <span data-ttu-id="dc689-119">**displayName**</span><span class="sxs-lookup"><span data-stu-id="dc689-119">**displayName**</span></span>         | <span data-ttu-id="dc689-120">string</span><span class="sxs-lookup"><span data-stu-id="dc689-120">string</span></span>  | <span data-ttu-id="dc689-121">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="dc689-121">The user-facing name of the column.</span></span>
| <span data-ttu-id="dc689-122">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="dc689-122">**enforceUniqueValues**</span></span> | <span data-ttu-id="dc689-123">логический</span><span class="sxs-lookup"><span data-stu-id="dc689-123">boolean</span></span> | <span data-ttu-id="dc689-124">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="dc689-124">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="dc689-125">**hidden**</span><span class="sxs-lookup"><span data-stu-id="dc689-125">**hidden**</span></span>              | <span data-ttu-id="dc689-126">логический</span><span class="sxs-lookup"><span data-stu-id="dc689-126">boolean</span></span> | <span data-ttu-id="dc689-127">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="dc689-127">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="dc689-128">**id**</span><span class="sxs-lookup"><span data-stu-id="dc689-128">**id**</span></span>                  | <span data-ttu-id="dc689-129">string</span><span class="sxs-lookup"><span data-stu-id="dc689-129">string</span></span>  | <span data-ttu-id="dc689-130">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="dc689-130">The unique identifier for the column.</span></span>
| <span data-ttu-id="dc689-131">**indexed**</span><span class="sxs-lookup"><span data-stu-id="dc689-131">**indexed**</span></span>             | <span data-ttu-id="dc689-132">логический</span><span class="sxs-lookup"><span data-stu-id="dc689-132">boolean</span></span> | <span data-ttu-id="dc689-133">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="dc689-133">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="dc689-134">**name**</span><span class="sxs-lookup"><span data-stu-id="dc689-134">**name**</span></span>                | <span data-ttu-id="dc689-135">string</span><span class="sxs-lookup"><span data-stu-id="dc689-135">string</span></span>  | <span data-ttu-id="dc689-136">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="dc689-136">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="dc689-137">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="dc689-137">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="dc689-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="dc689-138">**readOnly**</span></span>            | <span data-ttu-id="dc689-139">логический</span><span class="sxs-lookup"><span data-stu-id="dc689-139">bool</span></span>    | <span data-ttu-id="dc689-140">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="dc689-140">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="dc689-141">**required**</span><span class="sxs-lookup"><span data-stu-id="dc689-141">**required**</span></span>            | <span data-ttu-id="dc689-142">логический</span><span class="sxs-lookup"><span data-stu-id="dc689-142">boolean</span></span> | <span data-ttu-id="dc689-143">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="dc689-143">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="dc689-144">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="dc689-144">Columns can hold data of various types.</span></span>
<span data-ttu-id="dc689-145">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="dc689-145">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="dc689-146">Эти свойства являются взаимоисключающими. Для столбца можно указать только одно из них.</span><span class="sxs-lookup"><span data-stu-id="dc689-146">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="dc689-147">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dc689-147">Property name</span></span>     | <span data-ttu-id="dc689-148">Тип</span><span class="sxs-lookup"><span data-stu-id="dc689-148">Type</span></span>                    | <span data-ttu-id="dc689-149">Описание</span><span class="sxs-lookup"><span data-stu-id="dc689-149">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="dc689-150">**boolean**</span><span class="sxs-lookup"><span data-stu-id="dc689-150">**boolean**</span></span>       | <span data-ttu-id="dc689-151">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc689-151">[booleanColumn][]</span></span>       | <span data-ttu-id="dc689-152">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="dc689-152">This column stores boolean values.</span></span>
| <span data-ttu-id="dc689-153">**calculated**</span><span class="sxs-lookup"><span data-stu-id="dc689-153">**calculated**</span></span>    | <span data-ttu-id="dc689-154">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc689-154">[calculatedColumn][]</span></span>    | <span data-ttu-id="dc689-155">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="dc689-155">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="dc689-156">**choice**</span><span class="sxs-lookup"><span data-stu-id="dc689-156">**choice**</span></span>        | <span data-ttu-id="dc689-157">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc689-157">[choiceColumn][]</span></span>        | <span data-ttu-id="dc689-158">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="dc689-158">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="dc689-159">**currency**</span><span class="sxs-lookup"><span data-stu-id="dc689-159">**currency**</span></span>      | <span data-ttu-id="dc689-160">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc689-160">[currencyColumn][]</span></span>      | <span data-ttu-id="dc689-161">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="dc689-161">This column stores currency values.</span></span>
| <span data-ttu-id="dc689-162">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="dc689-162">**dateTime**</span></span>      | <span data-ttu-id="dc689-163">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc689-163">[dateTimeColumn][]</span></span>      | <span data-ttu-id="dc689-164">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="dc689-164">This column stores DateTime values.</span></span>
| <span data-ttu-id="dc689-165">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="dc689-165">**defaultValue**</span></span>  | <span data-ttu-id="dc689-166">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="dc689-166">[defaultColumnValue][]</span></span>  | <span data-ttu-id="dc689-167">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="dc689-167">The default value for this column.</span></span>
| <span data-ttu-id="dc689-168">**географическое положение**</span><span class="sxs-lookup"><span data-stu-id="dc689-168">**geolocation**</span></span>   | <span data-ttu-id="dc689-169">[жеолокатионколумн][]</span><span class="sxs-lookup"><span data-stu-id="dc689-169">[geolocationColumn][]</span></span>   | <span data-ttu-id="dc689-170">В этом столбце хранится географическое положение.</span><span class="sxs-lookup"><span data-stu-id="dc689-170">This column stores a geolocation.</span></span>
| <span data-ttu-id="dc689-171">**lookup**</span><span class="sxs-lookup"><span data-stu-id="dc689-171">**lookup**</span></span>        | <span data-ttu-id="dc689-172">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc689-172">[lookupColumn][]</span></span>        | <span data-ttu-id="dc689-173">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="dc689-173">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="dc689-174">**number**</span><span class="sxs-lookup"><span data-stu-id="dc689-174">**number**</span></span>        | <span data-ttu-id="dc689-175">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc689-175">[numberColumn][]</span></span>        | <span data-ttu-id="dc689-176">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="dc689-176">This column stores number values.</span></span>
| <span data-ttu-id="dc689-177">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="dc689-177">**personOrGroup**</span></span> | <span data-ttu-id="dc689-178">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc689-178">[personOrGroupColumn][]</span></span> | <span data-ttu-id="dc689-179">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="dc689-179">This column stores Person or Group values.</span></span>
| <span data-ttu-id="dc689-180">**text**</span><span class="sxs-lookup"><span data-stu-id="dc689-180">**text**</span></span>          | <span data-ttu-id="dc689-181">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc689-181">[textColumn][]</span></span>          | <span data-ttu-id="dc689-182">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="dc689-182">This column stores text values.</span></span>

<span data-ttu-id="dc689-183">Примечание. Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dc689-183">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="dc689-184">Хотя наиболее распространенные типы полей представлены выше, этот API все еще не содержит.</span><span class="sxs-lookup"><span data-stu-id="dc689-184">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="dc689-185">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="dc689-185">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="dc689-186">Примечания</span><span class="sxs-lookup"><span data-stu-id="dc689-186">Remarks</span></span>

<span data-ttu-id="dc689-187">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="dc689-187">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="dc689-188">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="dc689-188">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="dc689-189">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="dc689-189">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->