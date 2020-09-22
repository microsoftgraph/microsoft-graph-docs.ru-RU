---
author: JeremyKelley
description: Ресурс numberColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой числа.
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 49c3dce15297187bcda20e20ae339dba86d154db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988963"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="a4e73-103">Тип ресурса numberColumn</span><span class="sxs-lookup"><span data-stu-id="a4e73-103">NumberColumn resource type</span></span>

<span data-ttu-id="a4e73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4e73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4e73-105">Ресурс **numberColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой числа.</span><span class="sxs-lookup"><span data-stu-id="a4e73-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4e73-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a4e73-106">JSON representation</span></span>

<span data-ttu-id="a4e73-107">Ниже показано представление ресурса **numberColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4e73-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="a4e73-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4e73-108">Properties</span></span>

| <span data-ttu-id="a4e73-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a4e73-109">Property name</span></span>      | <span data-ttu-id="a4e73-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e73-110">Type</span></span>   | <span data-ttu-id="a4e73-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e73-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="a4e73-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="a4e73-112">**decimalPlaces**</span></span>  | <span data-ttu-id="a4e73-113">string</span><span class="sxs-lookup"><span data-stu-id="a4e73-113">string</span></span> | <span data-ttu-id="a4e73-114">Количество десятичных разрядов, которые необходимо отображать.</span><span class="sxs-lookup"><span data-stu-id="a4e73-114">How many decimal places to display.</span></span> <span data-ttu-id="a4e73-115">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="a4e73-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="a4e73-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="a4e73-116">**displayAs**</span></span>      | <span data-ttu-id="a4e73-117">string</span><span class="sxs-lookup"><span data-stu-id="a4e73-117">string</span></span> | <span data-ttu-id="a4e73-118">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="a4e73-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="a4e73-119">Должно иметь тип `number` или `percentage`.</span><span class="sxs-lookup"><span data-stu-id="a4e73-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="a4e73-120">Если тип не указан, считается, что значение имеет тип `number`.</span><span class="sxs-lookup"><span data-stu-id="a4e73-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="a4e73-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="a4e73-121">**maximum**</span></span>        | <span data-ttu-id="a4e73-122">double</span><span class="sxs-lookup"><span data-stu-id="a4e73-122">double</span></span> | <span data-ttu-id="a4e73-123">Максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="a4e73-123">The maximum permitted value.</span></span>
| <span data-ttu-id="a4e73-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="a4e73-124">**minimum**</span></span>        | <span data-ttu-id="a4e73-125">double</span><span class="sxs-lookup"><span data-stu-id="a4e73-125">double</span></span> | <span data-ttu-id="a4e73-126">Минимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="a4e73-126">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="a4e73-127">Значения decimalPlaces</span><span class="sxs-lookup"><span data-stu-id="a4e73-127">DecimalPlaces values</span></span>

| <span data-ttu-id="a4e73-128">Значение</span><span class="sxs-lookup"><span data-stu-id="a4e73-128">Value</span></span>          | <span data-ttu-id="a4e73-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e73-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="a4e73-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="a4e73-130">**automatic**</span></span>  | <span data-ttu-id="a4e73-131">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a4e73-131">Default.</span></span> <span data-ttu-id="a4e73-132">Автоматическое отображение необходимого количества десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="a4e73-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="a4e73-133">**none**</span><span class="sxs-lookup"><span data-stu-id="a4e73-133">**none**</span></span>       | <span data-ttu-id="a4e73-134">Не отображать десятичные разряды.</span><span class="sxs-lookup"><span data-stu-id="a4e73-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="a4e73-135">**one**</span><span class="sxs-lookup"><span data-stu-id="a4e73-135">**one**</span></span>        | <span data-ttu-id="a4e73-136">Всегда отображать один десятичный разряд.</span><span class="sxs-lookup"><span data-stu-id="a4e73-136">Always display one decimal place.</span></span>
| <span data-ttu-id="a4e73-137">**two**</span><span class="sxs-lookup"><span data-stu-id="a4e73-137">**two**</span></span>        | <span data-ttu-id="a4e73-138">Всегда отображать два десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="a4e73-138">Always display two decimal places.</span></span>
| <span data-ttu-id="a4e73-139">**three**</span><span class="sxs-lookup"><span data-stu-id="a4e73-139">**three**</span></span>      | <span data-ttu-id="a4e73-140">Всегда отображать три десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="a4e73-140">Always display three decimal places.</span></span>
| <span data-ttu-id="a4e73-141">**four**</span><span class="sxs-lookup"><span data-stu-id="a4e73-141">**four**</span></span>       | <span data-ttu-id="a4e73-142">Всегда отображать четыре десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="a4e73-142">Always display four decimal places.</span></span>
| <span data-ttu-id="a4e73-143">**five**</span><span class="sxs-lookup"><span data-stu-id="a4e73-143">**five**</span></span>       | <span data-ttu-id="a4e73-144">Всегда отображать пять десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="a4e73-144">Always display five decimal places.</span></span>

<span data-ttu-id="a4e73-145">Примечание. Свойства **decimalPlaces** и **displayAs** указывают способ отображения значений, а не то, в каком виде они хранятся.</span><span class="sxs-lookup"><span data-stu-id="a4e73-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="a4e73-146">Эти свойства можно обновлять.</span><span class="sxs-lookup"><span data-stu-id="a4e73-146">These properties may be updated.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": []
}
-->


