---
author: JeremyKelley
description: Ресурс numberColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой числа.
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0f6ed1c8aca8909b50f47f539e0569a4b68dad89
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522549"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="11d44-103">Тип ресурса numberColumn</span><span class="sxs-lookup"><span data-stu-id="11d44-103">NumberColumn resource type</span></span>

<span data-ttu-id="11d44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11d44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11d44-105">Ресурс **numberColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой числа.</span><span class="sxs-lookup"><span data-stu-id="11d44-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11d44-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="11d44-106">JSON representation</span></span>

<span data-ttu-id="11d44-107">Ниже показано представление ресурса **numberColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11d44-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="11d44-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="11d44-108">Properties</span></span>

| <span data-ttu-id="11d44-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="11d44-109">Property name</span></span>      | <span data-ttu-id="11d44-110">Тип</span><span class="sxs-lookup"><span data-stu-id="11d44-110">Type</span></span>   | <span data-ttu-id="11d44-111">Описание</span><span class="sxs-lookup"><span data-stu-id="11d44-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="11d44-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="11d44-112">**decimalPlaces**</span></span>  | <span data-ttu-id="11d44-113">string</span><span class="sxs-lookup"><span data-stu-id="11d44-113">string</span></span> | <span data-ttu-id="11d44-114">Количество десятичных разрядов, которые необходимо отображать.</span><span class="sxs-lookup"><span data-stu-id="11d44-114">How many decimal places to display.</span></span> <span data-ttu-id="11d44-115">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="11d44-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="11d44-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="11d44-116">**displayAs**</span></span>      | <span data-ttu-id="11d44-117">string</span><span class="sxs-lookup"><span data-stu-id="11d44-117">string</span></span> | <span data-ttu-id="11d44-118">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="11d44-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="11d44-119">Должно иметь тип `number` или `percentage`.</span><span class="sxs-lookup"><span data-stu-id="11d44-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="11d44-120">Если тип не указан, считается, что значение имеет тип `number`.</span><span class="sxs-lookup"><span data-stu-id="11d44-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="11d44-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="11d44-121">**maximum**</span></span>        | <span data-ttu-id="11d44-122">double</span><span class="sxs-lookup"><span data-stu-id="11d44-122">double</span></span> | <span data-ttu-id="11d44-123">Максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="11d44-123">The maximum permitted value.</span></span>
| <span data-ttu-id="11d44-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="11d44-124">**minimum**</span></span>        | <span data-ttu-id="11d44-125">double</span><span class="sxs-lookup"><span data-stu-id="11d44-125">double</span></span> | <span data-ttu-id="11d44-126">Минимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="11d44-126">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="11d44-127">Значения decimalPlaces</span><span class="sxs-lookup"><span data-stu-id="11d44-127">DecimalPlaces values</span></span>

| <span data-ttu-id="11d44-128">Значение</span><span class="sxs-lookup"><span data-stu-id="11d44-128">Value</span></span>          | <span data-ttu-id="11d44-129">Описание</span><span class="sxs-lookup"><span data-stu-id="11d44-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="11d44-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="11d44-130">**automatic**</span></span>  | <span data-ttu-id="11d44-131">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="11d44-131">Default.</span></span> <span data-ttu-id="11d44-132">Автоматическое отображение необходимого количества десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="11d44-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="11d44-133">**none**</span><span class="sxs-lookup"><span data-stu-id="11d44-133">**none**</span></span>       | <span data-ttu-id="11d44-134">Не отображать десятичные разряды.</span><span class="sxs-lookup"><span data-stu-id="11d44-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="11d44-135">**one**</span><span class="sxs-lookup"><span data-stu-id="11d44-135">**one**</span></span>        | <span data-ttu-id="11d44-136">Всегда отображать один десятичный разряд.</span><span class="sxs-lookup"><span data-stu-id="11d44-136">Always display one decimal place.</span></span>
| <span data-ttu-id="11d44-137">**two**</span><span class="sxs-lookup"><span data-stu-id="11d44-137">**two**</span></span>        | <span data-ttu-id="11d44-138">Всегда отображать два десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="11d44-138">Always display two decimal places.</span></span>
| <span data-ttu-id="11d44-139">**three**</span><span class="sxs-lookup"><span data-stu-id="11d44-139">**three**</span></span>      | <span data-ttu-id="11d44-140">Всегда отображать три десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="11d44-140">Always display three decimal places.</span></span>
| <span data-ttu-id="11d44-141">**four**</span><span class="sxs-lookup"><span data-stu-id="11d44-141">**four**</span></span>       | <span data-ttu-id="11d44-142">Всегда отображать четыре десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="11d44-142">Always display four decimal places.</span></span>
| <span data-ttu-id="11d44-143">**five**</span><span class="sxs-lookup"><span data-stu-id="11d44-143">**five**</span></span>       | <span data-ttu-id="11d44-144">Всегда отображать пять десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="11d44-144">Always display five decimal places.</span></span>

<span data-ttu-id="11d44-145">Примечание. Свойства **decimalPlaces** и **displayAs** указывают способ отображения значений, а не то, в каком виде они хранятся.</span><span class="sxs-lookup"><span data-stu-id="11d44-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="11d44-146">Эти свойства можно обновлять.</span><span class="sxs-lookup"><span data-stu-id="11d44-146">These properties may be updated.</span></span>

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
