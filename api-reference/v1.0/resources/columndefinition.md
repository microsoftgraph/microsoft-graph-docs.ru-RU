---
author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
description: Ниже показано представление ресурса ColumnDefinition в формате JSON.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 83f278123a8153629593c54604ce1285a48439a7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239247"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="d37bc-103">Ресурс ColumnDefinition</span><span class="sxs-lookup"><span data-stu-id="d37bc-103">ColumnDefinition resource</span></span>

<span data-ttu-id="d37bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d37bc-104">Namespace: microsoft.graph</span></span>

## <a name="json-representation"></a><span data-ttu-id="d37bc-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d37bc-105">JSON representation</span></span>

<span data-ttu-id="d37bc-106">Ниже показано представление ресурса ColumnDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d37bc-106">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d37bc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d37bc-107">Properties</span></span>

<span data-ttu-id="d37bc-108">Ниже перечислены свойства ресурса **columnDefinition**.</span><span class="sxs-lookup"><span data-stu-id="d37bc-108">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="d37bc-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="d37bc-109">Property name</span></span>           | <span data-ttu-id="d37bc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d37bc-110">Type</span></span>    | <span data-ttu-id="d37bc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d37bc-111">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="d37bc-112">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="d37bc-112">**columnGroup**</span></span>         | <span data-ttu-id="d37bc-113">строка</span><span class="sxs-lookup"><span data-stu-id="d37bc-113">string</span></span>  | <span data-ttu-id="d37bc-114">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="d37bc-114">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="d37bc-115">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="d37bc-115">Helps organize related columns.</span></span>
| <span data-ttu-id="d37bc-116">**description**</span><span class="sxs-lookup"><span data-stu-id="d37bc-116">**description**</span></span>         | <span data-ttu-id="d37bc-117">string</span><span class="sxs-lookup"><span data-stu-id="d37bc-117">string</span></span>  | <span data-ttu-id="d37bc-118">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="d37bc-118">The user-facing description of the column.</span></span>
| <span data-ttu-id="d37bc-119">**displayName**</span><span class="sxs-lookup"><span data-stu-id="d37bc-119">**displayName**</span></span>         | <span data-ttu-id="d37bc-120">string</span><span class="sxs-lookup"><span data-stu-id="d37bc-120">string</span></span>  | <span data-ttu-id="d37bc-121">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="d37bc-121">The user-facing name of the column.</span></span>
| <span data-ttu-id="d37bc-122">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="d37bc-122">**enforceUniqueValues**</span></span> | <span data-ttu-id="d37bc-123">логический</span><span class="sxs-lookup"><span data-stu-id="d37bc-123">boolean</span></span> | <span data-ttu-id="d37bc-124">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="d37bc-124">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="d37bc-125">**hidden**</span><span class="sxs-lookup"><span data-stu-id="d37bc-125">**hidden**</span></span>              | <span data-ttu-id="d37bc-126">логический</span><span class="sxs-lookup"><span data-stu-id="d37bc-126">boolean</span></span> | <span data-ttu-id="d37bc-127">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="d37bc-127">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="d37bc-128">**id**</span><span class="sxs-lookup"><span data-stu-id="d37bc-128">**id**</span></span>                  | <span data-ttu-id="d37bc-129">string</span><span class="sxs-lookup"><span data-stu-id="d37bc-129">string</span></span>  | <span data-ttu-id="d37bc-130">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="d37bc-130">The unique identifier for the column.</span></span>
| <span data-ttu-id="d37bc-131">**indexed**</span><span class="sxs-lookup"><span data-stu-id="d37bc-131">**indexed**</span></span>             | <span data-ttu-id="d37bc-132">логический</span><span class="sxs-lookup"><span data-stu-id="d37bc-132">boolean</span></span> | <span data-ttu-id="d37bc-133">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="d37bc-133">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="d37bc-134">**name**</span><span class="sxs-lookup"><span data-stu-id="d37bc-134">**name**</span></span>                | <span data-ttu-id="d37bc-135">string</span><span class="sxs-lookup"><span data-stu-id="d37bc-135">string</span></span>  | <span data-ttu-id="d37bc-136">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="d37bc-136">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="d37bc-137">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="d37bc-137">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="d37bc-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="d37bc-138">**readOnly**</span></span>            | <span data-ttu-id="d37bc-139">логический</span><span class="sxs-lookup"><span data-stu-id="d37bc-139">bool</span></span>    | <span data-ttu-id="d37bc-140">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="d37bc-140">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="d37bc-141">**required**</span><span class="sxs-lookup"><span data-stu-id="d37bc-141">**required**</span></span>            | <span data-ttu-id="d37bc-142">логический</span><span class="sxs-lookup"><span data-stu-id="d37bc-142">boolean</span></span> | <span data-ttu-id="d37bc-143">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="d37bc-143">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="d37bc-144">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="d37bc-144">Columns can hold data of various types.</span></span>
<span data-ttu-id="d37bc-145">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="d37bc-145">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="d37bc-146">Эти свойства являются взаимоисключающими. Для столбца можно указать только одно из них.</span><span class="sxs-lookup"><span data-stu-id="d37bc-146">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="d37bc-147">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="d37bc-147">Property name</span></span>     | <span data-ttu-id="d37bc-148">Тип</span><span class="sxs-lookup"><span data-stu-id="d37bc-148">Type</span></span>                    | <span data-ttu-id="d37bc-149">Описание</span><span class="sxs-lookup"><span data-stu-id="d37bc-149">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="d37bc-150">**boolean**</span><span class="sxs-lookup"><span data-stu-id="d37bc-150">**boolean**</span></span>       | <span data-ttu-id="d37bc-151">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="d37bc-151">[booleanColumn][]</span></span>       | <span data-ttu-id="d37bc-152">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="d37bc-152">This column stores boolean values.</span></span>
| <span data-ttu-id="d37bc-153">**calculated**</span><span class="sxs-lookup"><span data-stu-id="d37bc-153">**calculated**</span></span>    | <span data-ttu-id="d37bc-154">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="d37bc-154">[calculatedColumn][]</span></span>    | <span data-ttu-id="d37bc-155">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="d37bc-155">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="d37bc-156">**choice**</span><span class="sxs-lookup"><span data-stu-id="d37bc-156">**choice**</span></span>        | <span data-ttu-id="d37bc-157">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="d37bc-157">[choiceColumn][]</span></span>        | <span data-ttu-id="d37bc-158">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="d37bc-158">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="d37bc-159">**currency**</span><span class="sxs-lookup"><span data-stu-id="d37bc-159">**currency**</span></span>      | <span data-ttu-id="d37bc-160">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="d37bc-160">[currencyColumn][]</span></span>      | <span data-ttu-id="d37bc-161">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="d37bc-161">This column stores currency values.</span></span>
| <span data-ttu-id="d37bc-162">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="d37bc-162">**dateTime**</span></span>      | <span data-ttu-id="d37bc-163">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="d37bc-163">[dateTimeColumn][]</span></span>      | <span data-ttu-id="d37bc-164">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="d37bc-164">This column stores DateTime values.</span></span>
| <span data-ttu-id="d37bc-165">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="d37bc-165">**defaultValue**</span></span>  | <span data-ttu-id="d37bc-166">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="d37bc-166">[defaultColumnValue][]</span></span>  | <span data-ttu-id="d37bc-167">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="d37bc-167">The default value for this column.</span></span>
| <span data-ttu-id="d37bc-168">**geolocation**</span><span class="sxs-lookup"><span data-stu-id="d37bc-168">**geolocation**</span></span>   | <span data-ttu-id="d37bc-169">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="d37bc-169">[geolocationColumn][]</span></span>   | <span data-ttu-id="d37bc-170">В этом столбце хранится географическое местонахождение.</span><span class="sxs-lookup"><span data-stu-id="d37bc-170">This column stores a geolocation.</span></span>
| <span data-ttu-id="d37bc-171">**lookup**</span><span class="sxs-lookup"><span data-stu-id="d37bc-171">**lookup**</span></span>        | <span data-ttu-id="d37bc-172">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="d37bc-172">[lookupColumn][]</span></span>        | <span data-ttu-id="d37bc-173">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="d37bc-173">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="d37bc-174">**number**</span><span class="sxs-lookup"><span data-stu-id="d37bc-174">**number**</span></span>        | <span data-ttu-id="d37bc-175">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="d37bc-175">[numberColumn][]</span></span>        | <span data-ttu-id="d37bc-176">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="d37bc-176">This column stores number values.</span></span>
| <span data-ttu-id="d37bc-177">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="d37bc-177">**personOrGroup**</span></span> | <span data-ttu-id="d37bc-178">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="d37bc-178">[personOrGroupColumn][]</span></span> | <span data-ttu-id="d37bc-179">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="d37bc-179">This column stores Person or Group values.</span></span>
| <span data-ttu-id="d37bc-180">**text**</span><span class="sxs-lookup"><span data-stu-id="d37bc-180">**text**</span></span>          | <span data-ttu-id="d37bc-181">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="d37bc-181">[textColumn][]</span></span>          | <span data-ttu-id="d37bc-182">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="d37bc-182">This column stores text values.</span></span>

<span data-ttu-id="d37bc-183">Примечание. Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d37bc-183">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="d37bc-184">Хотя наиболее распространенные типы полей представлены выше, некоторые из них в этом API по-прежнему отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d37bc-184">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="d37bc-185">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="d37bc-185">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="d37bc-186">Примечания</span><span class="sxs-lookup"><span data-stu-id="d37bc-186">Remarks</span></span>

<span data-ttu-id="d37bc-187">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="d37bc-187">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="d37bc-188">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="d37bc-188">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="d37bc-189">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="d37bc-189">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->