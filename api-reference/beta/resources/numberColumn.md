---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: a0f5d13381c82a42159d0802d850d9996aaf8b54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855183"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="6eb31-102">Тип ресурса numberColumn</span><span class="sxs-lookup"><span data-stu-id="6eb31-102">NumberColumn resource type</span></span>

> <span data-ttu-id="6eb31-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6eb31-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6eb31-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6eb31-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6eb31-105">Ресурс **numberColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой числа.</span><span class="sxs-lookup"><span data-stu-id="6eb31-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6eb31-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6eb31-106">JSON representation</span></span>

<span data-ttu-id="6eb31-107">Ниже показано представление ресурса **numberColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6eb31-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="6eb31-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6eb31-108">Properties</span></span>

| <span data-ttu-id="6eb31-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6eb31-109">Property name</span></span>      | <span data-ttu-id="6eb31-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6eb31-110">Type</span></span>   | <span data-ttu-id="6eb31-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb31-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="6eb31-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="6eb31-112">**decimalPlaces**</span></span>  | <span data-ttu-id="6eb31-113">строка</span><span class="sxs-lookup"><span data-stu-id="6eb31-113">string</span></span> | <span data-ttu-id="6eb31-114">Количество десятичных разрядов, которые необходимо отображать.</span><span class="sxs-lookup"><span data-stu-id="6eb31-114">How many decimal places to display.</span></span> <span data-ttu-id="6eb31-115">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="6eb31-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="6eb31-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="6eb31-116">**displayAs**</span></span>      | <span data-ttu-id="6eb31-117">строка</span><span class="sxs-lookup"><span data-stu-id="6eb31-117">string</span></span> | <span data-ttu-id="6eb31-118">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="6eb31-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="6eb31-119">Должно иметь тип `number` или `percentage`.</span><span class="sxs-lookup"><span data-stu-id="6eb31-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="6eb31-120">Если тип не указан, считается, что значение имеет тип `number`.</span><span class="sxs-lookup"><span data-stu-id="6eb31-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="6eb31-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="6eb31-121">**maximum**</span></span>        | <span data-ttu-id="6eb31-122">double</span><span class="sxs-lookup"><span data-stu-id="6eb31-122">double</span></span> | <span data-ttu-id="6eb31-123">Максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="6eb31-123">The maximum permitted value.</span></span>
| <span data-ttu-id="6eb31-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="6eb31-124">**minimum**</span></span>        | <span data-ttu-id="6eb31-125">double</span><span class="sxs-lookup"><span data-stu-id="6eb31-125">double</span></span> | <span data-ttu-id="6eb31-126">Минимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="6eb31-126">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="6eb31-127">Значения decimalPlaces</span><span class="sxs-lookup"><span data-stu-id="6eb31-127">DecimalPlaces values</span></span>

| <span data-ttu-id="6eb31-128">Значение</span><span class="sxs-lookup"><span data-stu-id="6eb31-128">Value</span></span>          | <span data-ttu-id="6eb31-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb31-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="6eb31-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="6eb31-130">**automatic**</span></span>  | <span data-ttu-id="6eb31-131">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6eb31-131">Default.</span></span> <span data-ttu-id="6eb31-132">Автоматическое отображение необходимого количества десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="6eb31-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="6eb31-133">**none**</span><span class="sxs-lookup"><span data-stu-id="6eb31-133">**none**</span></span>       | <span data-ttu-id="6eb31-134">Не отображать десятичные разряды.</span><span class="sxs-lookup"><span data-stu-id="6eb31-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="6eb31-135">**one**</span><span class="sxs-lookup"><span data-stu-id="6eb31-135">**one**</span></span>        | <span data-ttu-id="6eb31-136">Всегда отображать один десятичный разряд.</span><span class="sxs-lookup"><span data-stu-id="6eb31-136">Always display one decimal place.</span></span>
| <span data-ttu-id="6eb31-137">**two**</span><span class="sxs-lookup"><span data-stu-id="6eb31-137">**two**</span></span>        | <span data-ttu-id="6eb31-138">Всегда отображать два десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="6eb31-138">Always display two decimal places.</span></span>
| <span data-ttu-id="6eb31-139">**three**</span><span class="sxs-lookup"><span data-stu-id="6eb31-139">**three**</span></span>      | <span data-ttu-id="6eb31-140">Всегда отображать три десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="6eb31-140">Always display three decimal places.</span></span>
| <span data-ttu-id="6eb31-141">**four**</span><span class="sxs-lookup"><span data-stu-id="6eb31-141">**four**</span></span>       | <span data-ttu-id="6eb31-142">Всегда отображать четыре десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="6eb31-142">Always display four decimal places.</span></span>
| <span data-ttu-id="6eb31-143">**five**</span><span class="sxs-lookup"><span data-stu-id="6eb31-143">**five**</span></span>       | <span data-ttu-id="6eb31-144">Всегда отображать пять десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="6eb31-144">Always display five decimal places.</span></span>

<span data-ttu-id="6eb31-145">Примечание. Свойства **decimalPlaces** и **displayAs** указывают способ отображения значений, а не то, в каком виде они хранятся.</span><span class="sxs-lookup"><span data-stu-id="6eb31-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="6eb31-146">Эти свойства можно обновлять.</span><span class="sxs-lookup"><span data-stu-id="6eb31-146">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
