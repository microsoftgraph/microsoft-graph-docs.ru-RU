---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
description: Ресурс numberColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой числа.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9196e2508ed3109ee56c24ad72943ca50aed11bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035974"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="c9121-103">Тип ресурса numberColumn</span><span class="sxs-lookup"><span data-stu-id="c9121-103">NumberColumn resource type</span></span>

<span data-ttu-id="c9121-104">Ресурс **numberColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой числа.</span><span class="sxs-lookup"><span data-stu-id="c9121-104">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9121-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c9121-105">JSON representation</span></span>

<span data-ttu-id="c9121-106">Ниже показано представление ресурса **numberColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9121-106">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="c9121-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9121-107">Properties</span></span>

| <span data-ttu-id="c9121-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c9121-108">Property name</span></span>      | <span data-ttu-id="c9121-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c9121-109">Type</span></span>   | <span data-ttu-id="c9121-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c9121-110">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="c9121-111">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="c9121-111">**decimalPlaces**</span></span>  | <span data-ttu-id="c9121-112">string</span><span class="sxs-lookup"><span data-stu-id="c9121-112">string</span></span> | <span data-ttu-id="c9121-113">Количество десятичных разрядов, которые необходимо отображать.</span><span class="sxs-lookup"><span data-stu-id="c9121-113">How many decimal places to display.</span></span> <span data-ttu-id="c9121-114">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="c9121-114">See below for information about the possible values.</span></span>
| <span data-ttu-id="c9121-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="c9121-115">**displayAs**</span></span>      | <span data-ttu-id="c9121-116">string</span><span class="sxs-lookup"><span data-stu-id="c9121-116">string</span></span> | <span data-ttu-id="c9121-117">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="c9121-117">How the value should be presented in the UX.</span></span> <span data-ttu-id="c9121-118">Должно иметь тип `number` или `percentage`.</span><span class="sxs-lookup"><span data-stu-id="c9121-118">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="c9121-119">Если тип не указан, считается, что значение имеет тип `number`.</span><span class="sxs-lookup"><span data-stu-id="c9121-119">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="c9121-120">**maximum**</span><span class="sxs-lookup"><span data-stu-id="c9121-120">**maximum**</span></span>        | <span data-ttu-id="c9121-121">double</span><span class="sxs-lookup"><span data-stu-id="c9121-121">double</span></span> | <span data-ttu-id="c9121-122">Максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="c9121-122">The maximum permitted value.</span></span>
| <span data-ttu-id="c9121-123">**minimum**</span><span class="sxs-lookup"><span data-stu-id="c9121-123">**minimum**</span></span>        | <span data-ttu-id="c9121-124">double</span><span class="sxs-lookup"><span data-stu-id="c9121-124">double</span></span> | <span data-ttu-id="c9121-125">Минимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="c9121-125">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="c9121-126">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="c9121-126">DecimalPlaces</span></span>

| <span data-ttu-id="c9121-127">Значение</span><span class="sxs-lookup"><span data-stu-id="c9121-127">Value</span></span>          | <span data-ttu-id="c9121-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c9121-128">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="c9121-129">**automatic**</span><span class="sxs-lookup"><span data-stu-id="c9121-129">**automatic**</span></span>  | <span data-ttu-id="c9121-130">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c9121-130">Default.</span></span> <span data-ttu-id="c9121-131">Автоматическое отображение необходимого количества десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="c9121-131">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="c9121-132">**none**</span><span class="sxs-lookup"><span data-stu-id="c9121-132">**none**</span></span>       | <span data-ttu-id="c9121-133">Не отображать десятичные разряды.</span><span class="sxs-lookup"><span data-stu-id="c9121-133">Do not display any decimal places.</span></span>
| <span data-ttu-id="c9121-134">**one**</span><span class="sxs-lookup"><span data-stu-id="c9121-134">**one**</span></span>        | <span data-ttu-id="c9121-135">Всегда отображать один десятичный разряд.</span><span class="sxs-lookup"><span data-stu-id="c9121-135">Always display one decimal place.</span></span>
| <span data-ttu-id="c9121-136">**two**</span><span class="sxs-lookup"><span data-stu-id="c9121-136">**two**</span></span>        | <span data-ttu-id="c9121-137">Всегда отображать два десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="c9121-137">Always display two decimal places.</span></span>
| <span data-ttu-id="c9121-138">**three**</span><span class="sxs-lookup"><span data-stu-id="c9121-138">**three**</span></span>      | <span data-ttu-id="c9121-139">Всегда отображать три десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="c9121-139">Always display three decimal places.</span></span>
| <span data-ttu-id="c9121-140">**four**</span><span class="sxs-lookup"><span data-stu-id="c9121-140">**four**</span></span>       | <span data-ttu-id="c9121-141">Всегда отображать четыре десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="c9121-141">Always display four decimal places.</span></span>
| <span data-ttu-id="c9121-142">**five**</span><span class="sxs-lookup"><span data-stu-id="c9121-142">**five**</span></span>       | <span data-ttu-id="c9121-143">Всегда отображать пять десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="c9121-143">Always display five decimal places.</span></span>

<span data-ttu-id="c9121-144">Примечание. Свойства **decimalPlaces** и **displayAs** указывают способ отображения значений, а не то, в каком виде они хранятся.</span><span class="sxs-lookup"><span data-stu-id="c9121-144">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="c9121-145">Эти свойства можно обновлять.</span><span class="sxs-lookup"><span data-stu-id="c9121-145">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(automatic,none,one,two,three,four,five) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(number,percentage) are in resource, but () are in table"
  ],
  "tocPath": "Resources/NumberColumn"
} -->
