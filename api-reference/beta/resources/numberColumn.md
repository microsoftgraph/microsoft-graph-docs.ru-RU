---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: edd495b62f0ccbd163ec31a2efca70923d0bc8ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463294"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="11ae0-102">Тип ресурса numberColumn</span><span class="sxs-lookup"><span data-stu-id="11ae0-102">NumberColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11ae0-103">Ресурс **numberColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой числа.</span><span class="sxs-lookup"><span data-stu-id="11ae0-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11ae0-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="11ae0-104">JSON representation</span></span>

<span data-ttu-id="11ae0-105">Ниже показано представление ресурса **numberColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11ae0-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="11ae0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="11ae0-106">Properties</span></span>

| <span data-ttu-id="11ae0-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="11ae0-107">Property name</span></span>      | <span data-ttu-id="11ae0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="11ae0-108">Type</span></span>   | <span data-ttu-id="11ae0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="11ae0-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="11ae0-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="11ae0-110">**decimalPlaces**</span></span>  | <span data-ttu-id="11ae0-111">string</span><span class="sxs-lookup"><span data-stu-id="11ae0-111">string</span></span> | <span data-ttu-id="11ae0-112">Количество десятичных разрядов, которые необходимо отображать.</span><span class="sxs-lookup"><span data-stu-id="11ae0-112">How many decimal places to display.</span></span> <span data-ttu-id="11ae0-113">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="11ae0-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="11ae0-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="11ae0-114">**displayAs**</span></span>      | <span data-ttu-id="11ae0-115">строка</span><span class="sxs-lookup"><span data-stu-id="11ae0-115">string</span></span> | <span data-ttu-id="11ae0-116">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="11ae0-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="11ae0-117">Должно иметь тип `number` или `percentage`.</span><span class="sxs-lookup"><span data-stu-id="11ae0-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="11ae0-118">Если тип не указан, считается, что значение имеет тип `number`.</span><span class="sxs-lookup"><span data-stu-id="11ae0-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="11ae0-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="11ae0-119">**maximum**</span></span>        | <span data-ttu-id="11ae0-120">double</span><span class="sxs-lookup"><span data-stu-id="11ae0-120">double</span></span> | <span data-ttu-id="11ae0-121">Максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="11ae0-121">The maximum permitted value.</span></span>
| <span data-ttu-id="11ae0-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="11ae0-122">**minimum**</span></span>        | <span data-ttu-id="11ae0-123">double</span><span class="sxs-lookup"><span data-stu-id="11ae0-123">double</span></span> | <span data-ttu-id="11ae0-124">Минимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="11ae0-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="11ae0-125">Значения decimalPlaces</span><span class="sxs-lookup"><span data-stu-id="11ae0-125">DecimalPlaces values</span></span>

| <span data-ttu-id="11ae0-126">Значение</span><span class="sxs-lookup"><span data-stu-id="11ae0-126">Value</span></span>          | <span data-ttu-id="11ae0-127">Описание</span><span class="sxs-lookup"><span data-stu-id="11ae0-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="11ae0-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="11ae0-128">**automatic**</span></span>  | <span data-ttu-id="11ae0-129">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="11ae0-129">Default.</span></span> <span data-ttu-id="11ae0-130">Автоматическое отображение необходимого количества десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="11ae0-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="11ae0-131">**none**</span><span class="sxs-lookup"><span data-stu-id="11ae0-131">**none**</span></span>       | <span data-ttu-id="11ae0-132">Не отображать десятичные разряды.</span><span class="sxs-lookup"><span data-stu-id="11ae0-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="11ae0-133">**one**</span><span class="sxs-lookup"><span data-stu-id="11ae0-133">**one**</span></span>        | <span data-ttu-id="11ae0-134">Всегда отображать один десятичный разряд.</span><span class="sxs-lookup"><span data-stu-id="11ae0-134">Always display one decimal place.</span></span>
| <span data-ttu-id="11ae0-135">**two**</span><span class="sxs-lookup"><span data-stu-id="11ae0-135">**two**</span></span>        | <span data-ttu-id="11ae0-136">Всегда отображать два десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="11ae0-136">Always display two decimal places.</span></span>
| <span data-ttu-id="11ae0-137">**three**</span><span class="sxs-lookup"><span data-stu-id="11ae0-137">**three**</span></span>      | <span data-ttu-id="11ae0-138">Всегда отображать три десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="11ae0-138">Always display three decimal places.</span></span>
| <span data-ttu-id="11ae0-139">**four**</span><span class="sxs-lookup"><span data-stu-id="11ae0-139">**four**</span></span>       | <span data-ttu-id="11ae0-140">Всегда отображать четыре десятичных разряда.</span><span class="sxs-lookup"><span data-stu-id="11ae0-140">Always display four decimal places.</span></span>
| <span data-ttu-id="11ae0-141">**five**</span><span class="sxs-lookup"><span data-stu-id="11ae0-141">**five**</span></span>       | <span data-ttu-id="11ae0-142">Всегда отображать пять десятичных разрядов.</span><span class="sxs-lookup"><span data-stu-id="11ae0-142">Always display five decimal places.</span></span>

<span data-ttu-id="11ae0-143">Примечание. Свойства **decimalPlaces** и **displayAs** указывают способ отображения значений, а не то, в каком виде они хранятся.</span><span class="sxs-lookup"><span data-stu-id="11ae0-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="11ae0-144">Эти свойства можно обновлять.</span><span class="sxs-lookup"><span data-stu-id="11ae0-144">These properties may be updated.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/numberColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
