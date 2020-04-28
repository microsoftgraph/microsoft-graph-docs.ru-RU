---
title: Тип ресурса workbookRangeView
description: Объект rangeView представляет набор видимых ячеек в родительском диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a8fb5810f43b415aee7a6151267bfd43e8644272
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519157"
---
# <a name="workbookrangeview-resource-type"></a><span data-ttu-id="037eb-103">Тип ресурса workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="037eb-103">workbookRangeView resource type</span></span>

<span data-ttu-id="037eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="037eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="037eb-105">Объект rangeView представляет набор видимых ячеек в родительском диапазоне.</span><span class="sxs-lookup"><span data-stu-id="037eb-105">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="037eb-106">Методы</span><span class="sxs-lookup"><span data-stu-id="037eb-106">Methods</span></span>

| <span data-ttu-id="037eb-107">Метод</span><span class="sxs-lookup"><span data-stu-id="037eb-107">Method</span></span>           | <span data-ttu-id="037eb-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="037eb-108">Return Type</span></span>    |<span data-ttu-id="037eb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="037eb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="037eb-110">Получение списка строк</span><span class="sxs-lookup"><span data-stu-id="037eb-110">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="037eb-111">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="037eb-111">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="037eb-112">Получение коллекции объектов workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="037eb-112">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="037eb-113">Itemat</span><span class="sxs-lookup"><span data-stu-id="037eb-113">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="037eb-114">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="037eb-114">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="037eb-115">Получение видимой ячейки из диапазона с учетом индекса.</span><span class="sxs-lookup"><span data-stu-id="037eb-115">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="037eb-116">Диапазон</span><span class="sxs-lookup"><span data-stu-id="037eb-116">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="037eb-117">workbookRange</span><span class="sxs-lookup"><span data-stu-id="037eb-117">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="037eb-118">Возвращение экземпляра range, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="037eb-118">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="037eb-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="037eb-119">Properties</span></span>
| <span data-ttu-id="037eb-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="037eb-120">Property</span></span>     | <span data-ttu-id="037eb-121">Тип</span><span class="sxs-lookup"><span data-stu-id="037eb-121">Type</span></span>   |<span data-ttu-id="037eb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="037eb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="037eb-123">columnCount</span><span class="sxs-lookup"><span data-stu-id="037eb-123">columnCount</span></span>|<span data-ttu-id="037eb-124">Int32</span><span class="sxs-lookup"><span data-stu-id="037eb-124">Int32</span></span>|<span data-ttu-id="037eb-p101">Возвращает количество видимых столбцов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="037eb-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="037eb-127">formulas</span><span class="sxs-lookup"><span data-stu-id="037eb-127">formulas</span></span>|<span data-ttu-id="037eb-128">Json</span><span class="sxs-lookup"><span data-stu-id="037eb-128">Json</span></span>|<span data-ttu-id="037eb-129">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="037eb-129">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="037eb-130">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="037eb-130">formulasLocal</span></span>|<span data-ttu-id="037eb-131">Json</span><span class="sxs-lookup"><span data-stu-id="037eb-131">Json</span></span>|<span data-ttu-id="037eb-p102">Представляет формулу в формате A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула "=SUM(A1, 1.5)" превратится в "=СУММ(A1;1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="037eb-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="037eb-134">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="037eb-134">formulasR1C1</span></span>|<span data-ttu-id="037eb-135">Json</span><span class="sxs-lookup"><span data-stu-id="037eb-135">Json</span></span>|<span data-ttu-id="037eb-136">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="037eb-136">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="037eb-137">index</span><span class="sxs-lookup"><span data-stu-id="037eb-137">index</span></span>|<span data-ttu-id="037eb-138">Int32</span><span class="sxs-lookup"><span data-stu-id="037eb-138">Int32</span></span>|<span data-ttu-id="037eb-139">Индекс диапазона.</span><span class="sxs-lookup"><span data-stu-id="037eb-139">Index of the range.</span></span>|
|<span data-ttu-id="037eb-140">numberFormat</span><span class="sxs-lookup"><span data-stu-id="037eb-140">numberFormat</span></span>|<span data-ttu-id="037eb-141">Json</span><span class="sxs-lookup"><span data-stu-id="037eb-141">Json</span></span>|<span data-ttu-id="037eb-p103">Представляет код в числовом формате Excel для заданной ячейки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="037eb-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="037eb-144">rowCount</span><span class="sxs-lookup"><span data-stu-id="037eb-144">rowCount</span></span>|<span data-ttu-id="037eb-145">Int32</span><span class="sxs-lookup"><span data-stu-id="037eb-145">Int32</span></span>|<span data-ttu-id="037eb-p104">Возвращает количество видимых строк. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="037eb-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="037eb-148">текст</span><span class="sxs-lookup"><span data-stu-id="037eb-148">text</span></span>|<span data-ttu-id="037eb-149">Json</span><span class="sxs-lookup"><span data-stu-id="037eb-149">Json</span></span>|<span data-ttu-id="037eb-p105">Текстовые значения указанного диапазона. Текстовое значение не зависит от ширины ячейки. Замена знака #, которая происходит в пользовательском интерфейсе Excel, не повлияет на текстовое значение, возвращаемое API. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="037eb-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="037eb-154">valueTypes</span><span class="sxs-lookup"><span data-stu-id="037eb-154">valueTypes</span></span>|<span data-ttu-id="037eb-155">Json</span><span class="sxs-lookup"><span data-stu-id="037eb-155">Json</span></span>|<span data-ttu-id="037eb-p106">Представляет тип данных каждой ячейки. Только для чтения. Возможные значения: Unknown, Empty, String, Integer, Double, Boolean, Error.</span><span class="sxs-lookup"><span data-stu-id="037eb-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="037eb-159">values</span><span class="sxs-lookup"><span data-stu-id="037eb-159">values</span></span>|<span data-ttu-id="037eb-160">Json</span><span class="sxs-lookup"><span data-stu-id="037eb-160">Json</span></span>|<span data-ttu-id="037eb-p107">Представляет необработанные значения указанного объекта rangeView. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="037eb-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="037eb-164">Связи</span><span class="sxs-lookup"><span data-stu-id="037eb-164">Relationships</span></span>
| <span data-ttu-id="037eb-165">Связь</span><span class="sxs-lookup"><span data-stu-id="037eb-165">Relationship</span></span> | <span data-ttu-id="037eb-166">Тип</span><span class="sxs-lookup"><span data-stu-id="037eb-166">Type</span></span>   |<span data-ttu-id="037eb-167">Описание</span><span class="sxs-lookup"><span data-stu-id="037eb-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="037eb-168">rows</span><span class="sxs-lookup"><span data-stu-id="037eb-168">rows</span></span>|<span data-ttu-id="037eb-169">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="037eb-169">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="037eb-p108">Представляет коллекцию видимых ячеек в диапазоне, сопоставленных с указанным диапазоном. Только для чтения.    Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="037eb-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="037eb-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="037eb-173">JSON representation</span></span>
<span data-ttu-id="037eb-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="037eb-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
