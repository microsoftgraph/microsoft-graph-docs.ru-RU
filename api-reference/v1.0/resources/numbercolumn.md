---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 3bc5ef0c2764fc941959a69ae58402ce3717e7b3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027667"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="ba9b2-102">Тип ресурса numberColumn</span><span class="sxs-lookup"><span data-stu-id="ba9b2-102">NumberColumn resource type</span></span>

<span data-ttu-id="ba9b2-103">Ресурс **numberColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой числа.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba9b2-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ba9b2-104">JSON representation</span></span>

<span data-ttu-id="ba9b2-105">Ниже показано представление ресурса **numberColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="ba9b2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba9b2-106">Properties</span></span>

| <span data-ttu-id="ba9b2-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ba9b2-107">Property name</span></span>      | <span data-ttu-id="ba9b2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ba9b2-108">Type</span></span>   | <span data-ttu-id="ba9b2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ba9b2-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="ba9b2-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="ba9b2-110">**decimalPlaces**</span></span>  | <span data-ttu-id="ba9b2-111">string</span><span class="sxs-lookup"><span data-stu-id="ba9b2-111">string</span></span> | <span data-ttu-id="ba9b2-112">Количество десятичных разрядов, которые необходимо отображать.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-112">How many decimal places to display.</span></span> <span data-ttu-id="ba9b2-113">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="ba9b2-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="ba9b2-114">**displayAs**</span></span>      | <span data-ttu-id="ba9b2-115">string</span><span class="sxs-lookup"><span data-stu-id="ba9b2-115">string</span></span> | <span data-ttu-id="ba9b2-116">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="ba9b2-117">Должно иметь тип `number` или `percentage`.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="ba9b2-118">Если тип не указан, считается, что значение имеет тип `number`.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="ba9b2-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="ba9b2-119">**maximum**</span></span>        | <span data-ttu-id="ba9b2-120">double</span><span class="sxs-lookup"><span data-stu-id="ba9b2-120">double</span></span> | <span data-ttu-id="ba9b2-121">Максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-121">The maximum permitted value.</span></span>
| <span data-ttu-id="ba9b2-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="ba9b2-122">**minimum**</span></span>        | <span data-ttu-id="ba9b2-123">double</span><span class="sxs-lookup"><span data-stu-id="ba9b2-123">double</span></span> | <span data-ttu-id="ba9b2-124">Минимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-124">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="ba9b2-125">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="ba9b2-125">DecimalPlaces</span></span>

| <span data-ttu-id="ba9b2-126">Значение</span><span class="sxs-lookup"><span data-stu-id="ba9b2-126">Value</span></span>          | <span data-ttu-id="ba9b2-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ba9b2-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="ba9b2-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="ba9b2-128">**automatic**</span></span>  | <span data-ttu-id="ba9b2-129">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-129">Default.</span></span> <span data-ttu-id="ba9b2-130">Автоматическое отображение необходимого количества десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="ba9b2-131">**none**</span><span class="sxs-lookup"><span data-stu-id="ba9b2-131">**none**</span></span>       | <span data-ttu-id="ba9b2-132">Не отображать десятичные разряды.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="ba9b2-133">**one**</span><span class="sxs-lookup"><span data-stu-id="ba9b2-133">**one**</span></span>        | <span data-ttu-id="ba9b2-134">Всегда отображать один десятичный разряд.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-134">Always display one decimal place.</span></span>
| <span data-ttu-id="ba9b2-135">**two**</span><span class="sxs-lookup"><span data-stu-id="ba9b2-135">**two**</span></span>        | <span data-ttu-id="ba9b2-136">Всегда отображать два десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-136">Always display two decimal places.</span></span>
| <span data-ttu-id="ba9b2-137">**three**</span><span class="sxs-lookup"><span data-stu-id="ba9b2-137">**three**</span></span>      | <span data-ttu-id="ba9b2-138">Всегда отображать три десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-138">Always display three decimal places.</span></span>
| <span data-ttu-id="ba9b2-139">**four**</span><span class="sxs-lookup"><span data-stu-id="ba9b2-139">**four**</span></span>       | <span data-ttu-id="ba9b2-140">Всегда отображать четыре десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-140">Always display four decimal places.</span></span>
| <span data-ttu-id="ba9b2-141">**five**</span><span class="sxs-lookup"><span data-stu-id="ba9b2-141">**five**</span></span>       | <span data-ttu-id="ba9b2-142">Всегда отображать пять десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-142">Always display five decimal places.</span></span>

<span data-ttu-id="ba9b2-143">Примечание. Свойства **decimalPlaces** и **displayAs** указывают способ отображения значений, а не то, в каком виде они хранятся.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="ba9b2-144">Эти свойства можно обновлять.</span><span class="sxs-lookup"><span data-stu-id="ba9b2-144">These properties may be updated.</span></span>

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
