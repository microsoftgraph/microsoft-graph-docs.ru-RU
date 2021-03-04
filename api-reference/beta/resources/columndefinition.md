---
author: JeremyKelley
description: Вот представление JSON ресурса columnDefinition.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: aab34ebe8a0cb7539775ba3e7b07e8ad7b3c357b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444341"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="e7b17-103">тип ресурса columnDefinition</span><span class="sxs-lookup"><span data-stu-id="e7b17-103">columnDefinition resource type</span></span>

<span data-ttu-id="e7b17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7b17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="e7b17-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7b17-105">JSON representation</span></span>

<span data-ttu-id="e7b17-106">Вот представление JSON ресурса columnDefinition.</span><span class="sxs-lookup"><span data-stu-id="e7b17-106">Here is a JSON representation of a columnDefinition resource.</span></span>

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
  "enforceUniqueValues": true,
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
  "text": { "@odata.type": "microsoft.graph.textColumn" },
  "isDeletable" : false,
  "propagateChanges": false,
  "isReorderable": false,
  "isSealed": false,
  "validation": { "@odata.type": "microsoft.graph.columnValidation" },
  "hyperlinkOrPicture": { "@odata.type": "microsoft.graph.hyperlinkOrPictureColumn" },
  "term": { "@odata.type": "microsoft.graph.termColumn" },
  "sourceContentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "thumbnail": { "@odata.type": "microsoft.graph.thumbnailColumn" },
  "type": { "@odata.type": "microsoft.graph.columnTypes" },
  "contentApprovalStatus": { "@odata.type": "microsoft.graph.contentApprovalStatusColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="e7b17-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7b17-107">Properties</span></span>

<span data-ttu-id="e7b17-108">В столбцах могут храниться данные различных типов.</span><span class="sxs-lookup"><span data-stu-id="e7b17-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="e7b17-109">Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.</span><span class="sxs-lookup"><span data-stu-id="e7b17-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="e7b17-110">Свойства типа (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) являются взаимоисключающими : столбец может иметь только один из указанных.</span><span class="sxs-lookup"><span data-stu-id="e7b17-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="e7b17-111">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e7b17-111">Property name</span></span>           | <span data-ttu-id="e7b17-112">Тип</span><span class="sxs-lookup"><span data-stu-id="e7b17-112">Type</span></span>    | <span data-ttu-id="e7b17-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e7b17-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="e7b17-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="e7b17-114">**columnGroup**</span></span>         | <span data-ttu-id="e7b17-115">строка</span><span class="sxs-lookup"><span data-stu-id="e7b17-115">string</span></span>  | <span data-ttu-id="e7b17-116">Для столбцов сайтов это имя группы, к которой принадлежит данный столбец.</span><span class="sxs-lookup"><span data-stu-id="e7b17-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="e7b17-117">Помогает упорядочивать связанные столбцы.</span><span class="sxs-lookup"><span data-stu-id="e7b17-117">Helps organize related columns.</span></span>
| <span data-ttu-id="e7b17-118">**description**</span><span class="sxs-lookup"><span data-stu-id="e7b17-118">**description**</span></span>         | <span data-ttu-id="e7b17-119">string</span><span class="sxs-lookup"><span data-stu-id="e7b17-119">string</span></span>  | <span data-ttu-id="e7b17-120">Описание столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="e7b17-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="e7b17-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e7b17-121">**displayName**</span></span>         | <span data-ttu-id="e7b17-122">string</span><span class="sxs-lookup"><span data-stu-id="e7b17-122">string</span></span>  | <span data-ttu-id="e7b17-123">Имя столбца, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="e7b17-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="e7b17-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="e7b17-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="e7b17-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7b17-125">Boolean</span></span> | <span data-ttu-id="e7b17-126">Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="e7b17-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="e7b17-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="e7b17-127">**hidden**</span></span>              | <span data-ttu-id="e7b17-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7b17-128">Boolean</span></span> | <span data-ttu-id="e7b17-129">Указывает, отображается ли столбец в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="e7b17-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="e7b17-130">**id**</span><span class="sxs-lookup"><span data-stu-id="e7b17-130">**id**</span></span>                  | <span data-ttu-id="e7b17-131">string</span><span class="sxs-lookup"><span data-stu-id="e7b17-131">string</span></span>  | <span data-ttu-id="e7b17-132">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="e7b17-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="e7b17-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="e7b17-133">**indexed**</span></span>             | <span data-ttu-id="e7b17-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7b17-134">Boolean</span></span> | <span data-ttu-id="e7b17-135">Указывает, можно ли использовать значения столбцов для сортировки и поиска.</span><span class="sxs-lookup"><span data-stu-id="e7b17-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="e7b17-136">**name**</span><span class="sxs-lookup"><span data-stu-id="e7b17-136">**name**</span></span>                | <span data-ttu-id="e7b17-137">string</span><span class="sxs-lookup"><span data-stu-id="e7b17-137">string</span></span>  | <span data-ttu-id="e7b17-138">Используемое в API имя столбца из свойства [fields][] объекта [listItem][].</span><span class="sxs-lookup"><span data-stu-id="e7b17-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="e7b17-139">Имя, которое видит пользователь, указывается в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="e7b17-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="e7b17-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="e7b17-140">**readOnly**</span></span>            | <span data-ttu-id="e7b17-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7b17-141">Boolean</span></span>    | <span data-ttu-id="e7b17-142">Указывает, можно ли менять значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="e7b17-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="e7b17-143">**required**</span><span class="sxs-lookup"><span data-stu-id="e7b17-143">**required**</span></span>            | <span data-ttu-id="e7b17-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7b17-144">Boolean</span></span> | <span data-ttu-id="e7b17-145">Указывает, является ли значение в столбце обязательным.</span><span class="sxs-lookup"><span data-stu-id="e7b17-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="e7b17-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e7b17-146">**boolean**</span></span>       | <span data-ttu-id="e7b17-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-147">[booleanColumn][]</span></span>       | <span data-ttu-id="e7b17-148">В этом столбце хранятся логические значения.</span><span class="sxs-lookup"><span data-stu-id="e7b17-148">This column stores boolean values.</span></span>
| <span data-ttu-id="e7b17-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="e7b17-149">**calculated**</span></span>    | <span data-ttu-id="e7b17-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="e7b17-151">Данные в этом столбце вычисляются относительно других столбцов.</span><span class="sxs-lookup"><span data-stu-id="e7b17-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="e7b17-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="e7b17-152">**choice**</span></span>        | <span data-ttu-id="e7b17-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-153">[choiceColumn][]</span></span>        | <span data-ttu-id="e7b17-154">В этом столбце хранятся данные из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="e7b17-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="e7b17-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="e7b17-155">**currency**</span></span>      | <span data-ttu-id="e7b17-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-156">[currencyColumn][]</span></span>      | <span data-ttu-id="e7b17-157">В этом столбце хранятся денежные значения.</span><span class="sxs-lookup"><span data-stu-id="e7b17-157">This column stores currency values.</span></span>
| <span data-ttu-id="e7b17-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="e7b17-158">**dateTime**</span></span>      | <span data-ttu-id="e7b17-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="e7b17-160">В этом столбце хранятся значения даты и времени.</span><span class="sxs-lookup"><span data-stu-id="e7b17-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="e7b17-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="e7b17-161">**defaultValue**</span></span>  | <span data-ttu-id="e7b17-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="e7b17-163">Значение по умолчанию для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="e7b17-163">The default value for this column.</span></span>
| <span data-ttu-id="e7b17-164">**геолокация**</span><span class="sxs-lookup"><span data-stu-id="e7b17-164">**geolocation**</span></span>   | <span data-ttu-id="e7b17-165">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="e7b17-166">В этом столбце хранится геолокация.</span><span class="sxs-lookup"><span data-stu-id="e7b17-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="e7b17-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="e7b17-167">**lookup**</span></span>        | <span data-ttu-id="e7b17-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-168">[lookupColumn][]</span></span>        | <span data-ttu-id="e7b17-169">Данные в этом столбце берутся из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="e7b17-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="e7b17-170">**number**</span><span class="sxs-lookup"><span data-stu-id="e7b17-170">**number**</span></span>        | <span data-ttu-id="e7b17-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-171">[numberColumn][]</span></span>        | <span data-ttu-id="e7b17-172">В этом столбце хранятся числовые значения.</span><span class="sxs-lookup"><span data-stu-id="e7b17-172">This column stores number values.</span></span>
| <span data-ttu-id="e7b17-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="e7b17-173">**personOrGroup**</span></span> | <span data-ttu-id="e7b17-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="e7b17-175">В этом столбце хранятся значения людей или групп.</span><span class="sxs-lookup"><span data-stu-id="e7b17-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="e7b17-176">**text**</span><span class="sxs-lookup"><span data-stu-id="e7b17-176">**text**</span></span>          | <span data-ttu-id="e7b17-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-177">[textColumn][]</span></span>          | <span data-ttu-id="e7b17-178">В этом столбце хранятся текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="e7b17-178">This column stores text values.</span></span>
| <span data-ttu-id="e7b17-179">**isDeletable**</span><span class="sxs-lookup"><span data-stu-id="e7b17-179">**isDeletable**</span></span>       | <span data-ttu-id="e7b17-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7b17-180">Boolean</span></span> | <span data-ttu-id="e7b17-181">Указывает, можно ли удалить этот столбец.</span><span class="sxs-lookup"><span data-stu-id="e7b17-181">Indicates whether this column can be deleted.</span></span>
| <span data-ttu-id="e7b17-182">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="e7b17-182">**propagateChanges**</span></span>     | <span data-ttu-id="e7b17-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7b17-183">Boolean</span></span> | <span data-ttu-id="e7b17-184">Если изменения "True" в этом столбце будут распространяться в списки, реализующих столбец.</span><span class="sxs-lookup"><span data-stu-id="e7b17-184">If 'True' changes to this column will be propagated to lists that implement the column.</span></span> 
| <span data-ttu-id="e7b17-185">**isReorderable**</span><span class="sxs-lookup"><span data-stu-id="e7b17-185">**isReorderable**</span></span>         | <span data-ttu-id="e7b17-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7b17-186">Boolean</span></span> | <span data-ttu-id="e7b17-187">Указывает, можно ли переуказать значения в столбце.</span><span class="sxs-lookup"><span data-stu-id="e7b17-187">Indicates whether values in the column can be reordered.</span></span> <span data-ttu-id="e7b17-188">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7b17-188">Read-only.</span></span>
| <span data-ttu-id="e7b17-189">**isSealed**</span><span class="sxs-lookup"><span data-stu-id="e7b17-189">**isSealed**</span></span>              | <span data-ttu-id="e7b17-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7b17-190">Boolean</span></span> | <span data-ttu-id="e7b17-191">Указывает, можно ли изменить столбец.</span><span class="sxs-lookup"><span data-stu-id="e7b17-191">Specifies whether column can be changed.</span></span>
| <span data-ttu-id="e7b17-192">**проверка**</span><span class="sxs-lookup"><span data-stu-id="e7b17-192">**validation**</span></span>   |  <span data-ttu-id="e7b17-193">[columnValidation][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-193">[columnValidation][]</span></span>    | <span data-ttu-id="e7b17-194">В этом столбце хранится формула проверки и сообщение для столбца.</span><span class="sxs-lookup"><span data-stu-id="e7b17-194">This column stores validation formula and message for the column.</span></span> 
| <span data-ttu-id="e7b17-195">**hyperlinkOrPicture**</span><span class="sxs-lookup"><span data-stu-id="e7b17-195">**hyperlinkOrPicture**</span></span>  | <span data-ttu-id="e7b17-196">[hyperlinkOrPictureColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-196">[hyperlinkOrPictureColumn][]</span></span> | <span data-ttu-id="e7b17-197">В этом столбце хранится гиперссылка или значения изображения.</span><span class="sxs-lookup"><span data-stu-id="e7b17-197">This column stores hyperlink or picture values.</span></span> 
| <span data-ttu-id="e7b17-198">**термин**</span><span class="sxs-lookup"><span data-stu-id="e7b17-198">**term**</span></span>     | <span data-ttu-id="e7b17-199">[termColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-199">[termColumn][]</span></span> | <span data-ttu-id="e7b17-200">В этом столбце хранится таксономия терминов.</span><span class="sxs-lookup"><span data-stu-id="e7b17-200">This column stores taxonomy terms.</span></span>
| <span data-ttu-id="e7b17-201">**sourceContentType**</span><span class="sxs-lookup"><span data-stu-id="e7b17-201">**sourceContentType**</span></span>   |<span data-ttu-id="e7b17-202">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-202">[contentTypeInfo][]</span></span>  | <span data-ttu-id="e7b17-203">ContentType, от которого наследуется этот столбец.</span><span class="sxs-lookup"><span data-stu-id="e7b17-203">ContentType from which this column is inherited from.</span></span> <span data-ttu-id="e7b17-204">Используется только при извлечении столбцов contentTypes.</span><span class="sxs-lookup"><span data-stu-id="e7b17-204">Used only while fetching contentTypes columns.</span></span>
| <span data-ttu-id="e7b17-205">**thumbnail**</span><span class="sxs-lookup"><span data-stu-id="e7b17-205">**thumbnail**</span></span>           |<span data-ttu-id="e7b17-206">[thumbnailColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-206">[thumbnailColumn][]</span></span>      | <span data-ttu-id="e7b17-207">В этом столбце хранится эскизные значения.</span><span class="sxs-lookup"><span data-stu-id="e7b17-207">This column stores thumbnail values.</span></span>
| <span data-ttu-id="e7b17-208">**тип**</span><span class="sxs-lookup"><span data-stu-id="e7b17-208">**type**</span></span>         | <span data-ttu-id="e7b17-209">columnTypes</span><span class="sxs-lookup"><span data-stu-id="e7b17-209">columnTypes</span></span>  | <span data-ttu-id="e7b17-210">Для столбцов сайта тип столбца.</span><span class="sxs-lookup"><span data-stu-id="e7b17-210">For site columns, the type of column.</span></span> <span data-ttu-id="e7b17-211">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="e7b17-211">Read-only</span></span>
| <span data-ttu-id="e7b17-212">**contentApprovalStatus**</span><span class="sxs-lookup"><span data-stu-id="e7b17-212">**contentApprovalStatus**</span></span>| <span data-ttu-id="e7b17-213">[contentApprovalStatusColumn][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-213">[contentApprovalStatusColumn][]</span></span>     | <span data-ttu-id="e7b17-214">В этом столбце сохраняется состояние утверждения контента.</span><span class="sxs-lookup"><span data-stu-id="e7b17-214">This column stores content approval status.</span></span>

## <a name="relationships"></a><span data-ttu-id="e7b17-215">Связи</span><span class="sxs-lookup"><span data-stu-id="e7b17-215">Relationships</span></span>

| <span data-ttu-id="e7b17-216">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e7b17-216">Property name</span></span>   | <span data-ttu-id="e7b17-217">Тип</span><span class="sxs-lookup"><span data-stu-id="e7b17-217">Type</span></span>                      | <span data-ttu-id="e7b17-218">Описание</span><span class="sxs-lookup"><span data-stu-id="e7b17-218">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="e7b17-219">**sourceColumn**</span><span class="sxs-lookup"><span data-stu-id="e7b17-219">**sourceColumn**</span></span> | <span data-ttu-id="e7b17-220">[columnDefinition][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-220">[columnDefinition][]</span></span> | <span data-ttu-id="e7b17-221">Столбец исходный для столбца типа контента.</span><span class="sxs-lookup"><span data-stu-id="e7b17-221">The source column for content type column.</span></span>

><span data-ttu-id="e7b17-222">**Примечание:** Эти свойства соответствуют переумериям [SPFieldType в SharePoint.][]</span><span class="sxs-lookup"><span data-stu-id="e7b17-222">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="e7b17-223">Хотя наиболее распространенные типы полей представлены в предыдущей таблице, этот API бета-версии по-прежнему отсутствует.</span><span class="sxs-lookup"><span data-stu-id="e7b17-223">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="e7b17-224">При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.</span><span class="sxs-lookup"><span data-stu-id="e7b17-224">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="e7b17-225">Примечания</span><span class="sxs-lookup"><span data-stu-id="e7b17-225">Remarks</span></span>

<span data-ttu-id="e7b17-226">По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.</span><span class="sxs-lookup"><span data-stu-id="e7b17-226">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="e7b17-227">Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="e7b17-227">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="e7b17-228">Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.</span><span class="sxs-lookup"><span data-stu-id="e7b17-228">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[columnDefinition]: columnDefinition.md
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
[termColumn]: termColumn.md
[contentApprovalStatusColumn]: contentApprovalStatusColumn.md
[thumbnailColumn]: thumbnailColumn.md
[hyperlinkOrPictureColumn]: hyperlinkOrPictureColumn.md
[columnValidation]: columnValidation.md
[contentTypeInfo]: contentTypeInfo.md

[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)

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