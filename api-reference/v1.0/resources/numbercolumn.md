---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
description: Ресурс numberColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой числа.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f2d8955ac71a7a6e9979542f08e4d0634274b69b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083024"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="c95b5-103">Тип ресурса numberColumn</span><span class="sxs-lookup"><span data-stu-id="c95b5-103">NumberColumn resource type</span></span>

<span data-ttu-id="c95b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c95b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c95b5-105">Ресурс **numberColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой числа.</span><span class="sxs-lookup"><span data-stu-id="c95b5-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c95b5-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c95b5-106">JSON representation</span></span>

<span data-ttu-id="c95b5-107">Ниже показано представление ресурса **numberColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c95b5-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="c95b5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c95b5-108">Properties</span></span>

| <span data-ttu-id="c95b5-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c95b5-109">Property name</span></span>      | <span data-ttu-id="c95b5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c95b5-110">Type</span></span>   | <span data-ttu-id="c95b5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c95b5-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="c95b5-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="c95b5-112">**decimalPlaces**</span></span>  | <span data-ttu-id="c95b5-113">string</span><span class="sxs-lookup"><span data-stu-id="c95b5-113">string</span></span> | <span data-ttu-id="c95b5-114">Количество десятичных разрядов, которые необходимо отображать.</span><span class="sxs-lookup"><span data-stu-id="c95b5-114">How many decimal places to display.</span></span> <span data-ttu-id="c95b5-115">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="c95b5-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="c95b5-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="c95b5-116">**displayAs**</span></span>      | <span data-ttu-id="c95b5-117">string</span><span class="sxs-lookup"><span data-stu-id="c95b5-117">string</span></span> | <span data-ttu-id="c95b5-118">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="c95b5-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="c95b5-119">Должно иметь тип `number` или `percentage`.</span><span class="sxs-lookup"><span data-stu-id="c95b5-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="c95b5-120">Если тип не указан, считается, что значение имеет тип `number`.</span><span class="sxs-lookup"><span data-stu-id="c95b5-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="c95b5-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="c95b5-121">**maximum**</span></span>        | <span data-ttu-id="c95b5-122">double</span><span class="sxs-lookup"><span data-stu-id="c95b5-122">double</span></span> | <span data-ttu-id="c95b5-123">Максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="c95b5-123">The maximum permitted value.</span></span>
| <span data-ttu-id="c95b5-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="c95b5-124">**minimum**</span></span>        | <span data-ttu-id="c95b5-125">double</span><span class="sxs-lookup"><span data-stu-id="c95b5-125">double</span></span> | <span data-ttu-id="c95b5-126">Минимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="c95b5-126">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="c95b5-127">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="c95b5-127">DecimalPlaces</span></span>

| <span data-ttu-id="c95b5-128">Значение</span><span class="sxs-lookup"><span data-stu-id="c95b5-128">Value</span></span>          | <span data-ttu-id="c95b5-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c95b5-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="c95b5-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="c95b5-130">**automatic**</span></span>  | <span data-ttu-id="c95b5-131">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c95b5-131">Default.</span></span> <span data-ttu-id="c95b5-132">Автоматическое отображение необходимого количества десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="c95b5-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="c95b5-133">**none**</span><span class="sxs-lookup"><span data-stu-id="c95b5-133">**none**</span></span>       | <span data-ttu-id="c95b5-134">Не отображать десятичные разряды.</span><span class="sxs-lookup"><span data-stu-id="c95b5-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="c95b5-135">**one**</span><span class="sxs-lookup"><span data-stu-id="c95b5-135">**one**</span></span>        | <span data-ttu-id="c95b5-136">Всегда отображать один десятичный разряд.</span><span class="sxs-lookup"><span data-stu-id="c95b5-136">Always display one decimal place.</span></span>
| <span data-ttu-id="c95b5-137">**two**</span><span class="sxs-lookup"><span data-stu-id="c95b5-137">**two**</span></span>        | <span data-ttu-id="c95b5-138">Всегда отображать два десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="c95b5-138">Always display two decimal places.</span></span>
| <span data-ttu-id="c95b5-139">**three**</span><span class="sxs-lookup"><span data-stu-id="c95b5-139">**three**</span></span>      | <span data-ttu-id="c95b5-140">Всегда отображать три десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="c95b5-140">Always display three decimal places.</span></span>
| <span data-ttu-id="c95b5-141">**four**</span><span class="sxs-lookup"><span data-stu-id="c95b5-141">**four**</span></span>       | <span data-ttu-id="c95b5-142">Всегда отображать четыре десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="c95b5-142">Always display four decimal places.</span></span>
| <span data-ttu-id="c95b5-143">**five**</span><span class="sxs-lookup"><span data-stu-id="c95b5-143">**five**</span></span>       | <span data-ttu-id="c95b5-144">Всегда отображать пять десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="c95b5-144">Always display five decimal places.</span></span>

<span data-ttu-id="c95b5-145">Примечание. Свойства **decimalPlaces** и **displayAs** указывают способ отображения значений, а не то, в каком виде они хранятся.</span><span class="sxs-lookup"><span data-stu-id="c95b5-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="c95b5-146">Эти свойства можно обновлять.</span><span class="sxs-lookup"><span data-stu-id="c95b5-146">These properties may be updated.</span></span>

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

