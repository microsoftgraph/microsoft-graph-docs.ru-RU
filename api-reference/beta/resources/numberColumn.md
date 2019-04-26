---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: f70a1d71729be68fc4d5dcb3de2599ff131bb8a9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342095"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="def53-102">Тип ресурса numberColumn</span><span class="sxs-lookup"><span data-stu-id="def53-102">NumberColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="def53-103">Ресурс **numberColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой числа.</span><span class="sxs-lookup"><span data-stu-id="def53-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="def53-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="def53-104">JSON representation</span></span>

<span data-ttu-id="def53-105">Ниже показано представление ресурса **numberColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="def53-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="def53-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="def53-106">Properties</span></span>

| <span data-ttu-id="def53-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="def53-107">Property name</span></span>      | <span data-ttu-id="def53-108">Тип</span><span class="sxs-lookup"><span data-stu-id="def53-108">Type</span></span>   | <span data-ttu-id="def53-109">Описание</span><span class="sxs-lookup"><span data-stu-id="def53-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="def53-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="def53-110">**decimalPlaces**</span></span>  | <span data-ttu-id="def53-111">string</span><span class="sxs-lookup"><span data-stu-id="def53-111">string</span></span> | <span data-ttu-id="def53-112">Количество десятичных разрядов, которые необходимо отображать.</span><span class="sxs-lookup"><span data-stu-id="def53-112">How many decimal places to display.</span></span> <span data-ttu-id="def53-113">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="def53-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="def53-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="def53-114">**displayAs**</span></span>      | <span data-ttu-id="def53-115">string</span><span class="sxs-lookup"><span data-stu-id="def53-115">string</span></span> | <span data-ttu-id="def53-116">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="def53-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="def53-117">Должно иметь тип `number` или `percentage`.</span><span class="sxs-lookup"><span data-stu-id="def53-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="def53-118">Если тип не указан, считается, что значение имеет тип `number`.</span><span class="sxs-lookup"><span data-stu-id="def53-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="def53-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="def53-119">**maximum**</span></span>        | <span data-ttu-id="def53-120">double</span><span class="sxs-lookup"><span data-stu-id="def53-120">double</span></span> | <span data-ttu-id="def53-121">Максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="def53-121">The maximum permitted value.</span></span>
| <span data-ttu-id="def53-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="def53-122">**minimum**</span></span>        | <span data-ttu-id="def53-123">double</span><span class="sxs-lookup"><span data-stu-id="def53-123">double</span></span> | <span data-ttu-id="def53-124">Минимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="def53-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="def53-125">Значения decimalPlaces</span><span class="sxs-lookup"><span data-stu-id="def53-125">DecimalPlaces values</span></span>

| <span data-ttu-id="def53-126">Значение</span><span class="sxs-lookup"><span data-stu-id="def53-126">Value</span></span>          | <span data-ttu-id="def53-127">Описание</span><span class="sxs-lookup"><span data-stu-id="def53-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="def53-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="def53-128">**automatic**</span></span>  | <span data-ttu-id="def53-129">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="def53-129">Default.</span></span> <span data-ttu-id="def53-130">Автоматическое отображение необходимого количества десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="def53-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="def53-131">**none**</span><span class="sxs-lookup"><span data-stu-id="def53-131">**none**</span></span>       | <span data-ttu-id="def53-132">Не отображать десятичные разряды.</span><span class="sxs-lookup"><span data-stu-id="def53-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="def53-133">**one**</span><span class="sxs-lookup"><span data-stu-id="def53-133">**one**</span></span>        | <span data-ttu-id="def53-134">Всегда отображать один десятичный разряд.</span><span class="sxs-lookup"><span data-stu-id="def53-134">Always display one decimal place.</span></span>
| <span data-ttu-id="def53-135">**two**</span><span class="sxs-lookup"><span data-stu-id="def53-135">**two**</span></span>        | <span data-ttu-id="def53-136">Всегда отображать два десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="def53-136">Always display two decimal places.</span></span>
| <span data-ttu-id="def53-137">**three**</span><span class="sxs-lookup"><span data-stu-id="def53-137">**three**</span></span>      | <span data-ttu-id="def53-138">Всегда отображать три десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="def53-138">Always display three decimal places.</span></span>
| <span data-ttu-id="def53-139">**four**</span><span class="sxs-lookup"><span data-stu-id="def53-139">**four**</span></span>       | <span data-ttu-id="def53-140">Всегда отображать четыре десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="def53-140">Always display four decimal places.</span></span>
| <span data-ttu-id="def53-141">**five**</span><span class="sxs-lookup"><span data-stu-id="def53-141">**five**</span></span>       | <span data-ttu-id="def53-142">Всегда отображать пять десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="def53-142">Always display five decimal places.</span></span>

<span data-ttu-id="def53-143">Примечание. Свойства **decimalPlaces** и **displayAs** указывают способ отображения значений, а не то, в каком виде они хранятся.</span><span class="sxs-lookup"><span data-stu-id="def53-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="def53-144">Эти свойства можно обновлять.</span><span class="sxs-lookup"><span data-stu-id="def53-144">These properties may be updated.</span></span>

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
