---
author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
description: Ресурс numberColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой числа.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 89b5c81f94895e248dfd4c5f75983bacf352f9e8
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238633"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="8d892-103">Тип ресурса numberColumn</span><span class="sxs-lookup"><span data-stu-id="8d892-103">NumberColumn resource type</span></span>

<span data-ttu-id="8d892-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d892-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d892-105">Ресурс **numberColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой числа.</span><span class="sxs-lookup"><span data-stu-id="8d892-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d892-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8d892-106">JSON representation</span></span>

<span data-ttu-id="8d892-107">Ниже показано представление ресурса **numberColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d892-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="8d892-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d892-108">Properties</span></span>

| <span data-ttu-id="8d892-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8d892-109">Property name</span></span>      | <span data-ttu-id="8d892-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8d892-110">Type</span></span>   | <span data-ttu-id="8d892-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8d892-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="8d892-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="8d892-112">**decimalPlaces**</span></span>  | <span data-ttu-id="8d892-113">string</span><span class="sxs-lookup"><span data-stu-id="8d892-113">string</span></span> | <span data-ttu-id="8d892-114">Количество десятичных разрядов, которые необходимо отображать.</span><span class="sxs-lookup"><span data-stu-id="8d892-114">How many decimal places to display.</span></span> <span data-ttu-id="8d892-115">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="8d892-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="8d892-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="8d892-116">**displayAs**</span></span>      | <span data-ttu-id="8d892-117">string</span><span class="sxs-lookup"><span data-stu-id="8d892-117">string</span></span> | <span data-ttu-id="8d892-118">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="8d892-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="8d892-119">Должно иметь тип `number` или `percentage`.</span><span class="sxs-lookup"><span data-stu-id="8d892-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="8d892-120">Если тип не указан, считается, что значение имеет тип `number`.</span><span class="sxs-lookup"><span data-stu-id="8d892-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="8d892-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="8d892-121">**maximum**</span></span>        | <span data-ttu-id="8d892-122">double</span><span class="sxs-lookup"><span data-stu-id="8d892-122">double</span></span> | <span data-ttu-id="8d892-123">Максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="8d892-123">The maximum permitted value.</span></span>
| <span data-ttu-id="8d892-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="8d892-124">**minimum**</span></span>        | <span data-ttu-id="8d892-125">double</span><span class="sxs-lookup"><span data-stu-id="8d892-125">double</span></span> | <span data-ttu-id="8d892-126">Минимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="8d892-126">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="8d892-127">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="8d892-127">DecimalPlaces</span></span>

| <span data-ttu-id="8d892-128">Значение</span><span class="sxs-lookup"><span data-stu-id="8d892-128">Value</span></span>          | <span data-ttu-id="8d892-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8d892-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="8d892-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="8d892-130">**automatic**</span></span>  | <span data-ttu-id="8d892-131">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8d892-131">Default.</span></span> <span data-ttu-id="8d892-132">Автоматическое отображение необходимого количества десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="8d892-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="8d892-133">**none**</span><span class="sxs-lookup"><span data-stu-id="8d892-133">**none**</span></span>       | <span data-ttu-id="8d892-134">Не отображать десятичные разряды.</span><span class="sxs-lookup"><span data-stu-id="8d892-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="8d892-135">**one**</span><span class="sxs-lookup"><span data-stu-id="8d892-135">**one**</span></span>        | <span data-ttu-id="8d892-136">Всегда отображать один десятичный разряд.</span><span class="sxs-lookup"><span data-stu-id="8d892-136">Always display one decimal place.</span></span>
| <span data-ttu-id="8d892-137">**two**</span><span class="sxs-lookup"><span data-stu-id="8d892-137">**two**</span></span>        | <span data-ttu-id="8d892-138">Всегда отображать два десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="8d892-138">Always display two decimal places.</span></span>
| <span data-ttu-id="8d892-139">**three**</span><span class="sxs-lookup"><span data-stu-id="8d892-139">**three**</span></span>      | <span data-ttu-id="8d892-140">Всегда отображать три десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="8d892-140">Always display three decimal places.</span></span>
| <span data-ttu-id="8d892-141">**four**</span><span class="sxs-lookup"><span data-stu-id="8d892-141">**four**</span></span>       | <span data-ttu-id="8d892-142">Всегда отображать четыре десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="8d892-142">Always display four decimal places.</span></span>
| <span data-ttu-id="8d892-143">**five**</span><span class="sxs-lookup"><span data-stu-id="8d892-143">**five**</span></span>       | <span data-ttu-id="8d892-144">Всегда отображать пять десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="8d892-144">Always display five decimal places.</span></span>

<span data-ttu-id="8d892-145">Примечание. Свойства **decimalPlaces** и **displayAs** указывают способ отображения значений, а не то, в каком виде они хранятся.</span><span class="sxs-lookup"><span data-stu-id="8d892-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="8d892-146">Эти свойства можно обновлять.</span><span class="sxs-lookup"><span data-stu-id="8d892-146">These properties may be updated.</span></span>

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

