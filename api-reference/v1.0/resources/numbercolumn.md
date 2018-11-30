---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 8aa366e3c4f59fc5d22f945c863bab4f91373b67
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="d123d-102">Тип ресурса numberColumn</span><span class="sxs-lookup"><span data-stu-id="d123d-102">NumberColumn resource type</span></span>

<span data-ttu-id="d123d-103">Ресурс **numberColumn** в ресурсе [columnDefinition](columnDefinition.md) указывает, что значения столбца представляют собой числа.</span><span class="sxs-lookup"><span data-stu-id="d123d-103">The **numberColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d123d-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d123d-104">JSON representation</span></span>

<span data-ttu-id="d123d-105">Ниже показано представление ресурса **numberColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d123d-105">Here is a JSON representation of a **drive** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="d123d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d123d-106">Properties</span></span>

| <span data-ttu-id="d123d-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="d123d-107">Property name</span></span>      | <span data-ttu-id="d123d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d123d-108">Type</span></span>   | <span data-ttu-id="d123d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d123d-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="d123d-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="d123d-110">**decimalPlaces**</span></span>  | <span data-ttu-id="d123d-111">строка</span><span class="sxs-lookup"><span data-stu-id="d123d-111">string</span></span> | <span data-ttu-id="d123d-112">Количество десятичных разрядов, которые необходимо отображать.</span><span class="sxs-lookup"><span data-stu-id="d123d-112">How many decimal places to display.</span></span> <span data-ttu-id="d123d-113">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="d123d-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="d123d-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="d123d-114">**displayAs**</span></span>      | <span data-ttu-id="d123d-115">строка</span><span class="sxs-lookup"><span data-stu-id="d123d-115">string</span></span> | <span data-ttu-id="d123d-116">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="d123d-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="d123d-117">Должно относиться к типу `number` или `percentage`.</span><span class="sxs-lookup"><span data-stu-id="d123d-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="d123d-118">Если тип не указан, считается, что значение относится к типу `number`.</span><span class="sxs-lookup"><span data-stu-id="d123d-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="d123d-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="d123d-119">**maximum**</span></span>        | <span data-ttu-id="d123d-120">double</span><span class="sxs-lookup"><span data-stu-id="d123d-120">double</span></span> | <span data-ttu-id="d123d-121">Максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="d123d-121">The maximum permitted value.</span></span>
| <span data-ttu-id="d123d-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="d123d-122">**minimum**</span></span>        | <span data-ttu-id="d123d-123">double</span><span class="sxs-lookup"><span data-stu-id="d123d-123">double</span></span> | <span data-ttu-id="d123d-124">Минимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="d123d-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="d123d-125">Значения decimalPlaces</span><span class="sxs-lookup"><span data-stu-id="d123d-125">DecimalPlaces values</span></span>

| <span data-ttu-id="d123d-126">Значение</span><span class="sxs-lookup"><span data-stu-id="d123d-126">Value</span></span>          | <span data-ttu-id="d123d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d123d-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="d123d-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="d123d-128">**"automatic"**</span></span>  | <span data-ttu-id="d123d-129">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d123d-129">Default</span></span> <span data-ttu-id="d123d-130">Автоматическое отображение необходимого количества десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="d123d-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="d123d-131">**none**</span><span class="sxs-lookup"><span data-stu-id="d123d-131">**None**</span></span>       | <span data-ttu-id="d123d-132">Не отображать десятичные разряды.</span><span class="sxs-lookup"><span data-stu-id="d123d-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="d123d-133">**one**</span><span class="sxs-lookup"><span data-stu-id="d123d-133">**One**</span></span>        | <span data-ttu-id="d123d-134">Всегда отображать один десятичный разряд.</span><span class="sxs-lookup"><span data-stu-id="d123d-134">Always display one decimal place.</span></span>
| <span data-ttu-id="d123d-135">**two**</span><span class="sxs-lookup"><span data-stu-id="d123d-135">**Two**</span></span>        | <span data-ttu-id="d123d-136">Всегда отображать два десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="d123d-136">Always display two decimal places.</span></span>
| <span data-ttu-id="d123d-137">**three**</span><span class="sxs-lookup"><span data-stu-id="d123d-137">**Three**</span></span>      | <span data-ttu-id="d123d-138">Всегда отображать три десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="d123d-138">Always display three decimal places.</span></span>
| <span data-ttu-id="d123d-139">**four**</span><span class="sxs-lookup"><span data-stu-id="d123d-139">**Four**</span></span>       | <span data-ttu-id="d123d-140">Всегда отображать четыре десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="d123d-140">Always display four decimal places.</span></span>
| <span data-ttu-id="d123d-141">**five**</span><span class="sxs-lookup"><span data-stu-id="d123d-141">**five**</span></span>       | <span data-ttu-id="d123d-142">Всегда отображать пять десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="d123d-142">Always display five decimal places.</span></span>

<span data-ttu-id="d123d-143">Примечание. Свойства **decimalPlaces** и **displayAs** указывают способ отображения значений, а не то, в каком виде они хранятся.</span><span class="sxs-lookup"><span data-stu-id="d123d-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="d123d-144">Эти свойства можно обновлять.</span><span class="sxs-lookup"><span data-stu-id="d123d-144">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
