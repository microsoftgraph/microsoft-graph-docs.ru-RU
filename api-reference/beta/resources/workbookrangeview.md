---
title: Тип ресурсов rangeView
description: Объект rangeView представляет набор видимых ячеек в родительском диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ace424d12e38e4bb907923ea542ebd7330130d06
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643981"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="27b35-103">Тип ресурсов rangeView</span><span class="sxs-lookup"><span data-stu-id="27b35-103">rangeView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27b35-104">Объект rangeView представляет набор видимых ячеек в родительском диапазоне.</span><span class="sxs-lookup"><span data-stu-id="27b35-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="27b35-105">Методы</span><span class="sxs-lookup"><span data-stu-id="27b35-105">Methods</span></span>

| <span data-ttu-id="27b35-106">Метод</span><span class="sxs-lookup"><span data-stu-id="27b35-106">Method</span></span>           | <span data-ttu-id="27b35-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27b35-107">Return Type</span></span>    |<span data-ttu-id="27b35-108">Описание</span><span class="sxs-lookup"><span data-stu-id="27b35-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27b35-109">[Получение списка строк](../api/workbookrangeview-list-rows.md) </span><span class="sxs-lookup"><span data-stu-id="27b35-109">[List rows](../api/workbookrangeview-list-rows.md)</span></span> |<span data-ttu-id="27b35-110">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="27b35-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="27b35-111">Получение коллекции объектов workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="27b35-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="27b35-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="27b35-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="27b35-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="27b35-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="27b35-114">Получение видимой ячейки из диапазона с учетом индекса.</span><span class="sxs-lookup"><span data-stu-id="27b35-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="27b35-115">Диапазон</span><span class="sxs-lookup"><span data-stu-id="27b35-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="27b35-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="27b35-116">workbookRange</span></span>](range.md)|<span data-ttu-id="27b35-117">Возвращение экземпляра range, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="27b35-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="27b35-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="27b35-118">Properties</span></span>
| <span data-ttu-id="27b35-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="27b35-119">Property</span></span>     | <span data-ttu-id="27b35-120">Тип</span><span class="sxs-lookup"><span data-stu-id="27b35-120">Type</span></span>   |<span data-ttu-id="27b35-121">Описание</span><span class="sxs-lookup"><span data-stu-id="27b35-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27b35-122">columnCount</span><span class="sxs-lookup"><span data-stu-id="27b35-122">columnCount</span></span>|<span data-ttu-id="27b35-123">Int32</span><span class="sxs-lookup"><span data-stu-id="27b35-123">Int32</span></span>|<span data-ttu-id="27b35-p101">Возвращает количество видимых столбцов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27b35-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="27b35-126">formulas</span><span class="sxs-lookup"><span data-stu-id="27b35-126">formulas</span></span>|<span data-ttu-id="27b35-127">Json</span><span class="sxs-lookup"><span data-stu-id="27b35-127">Json</span></span>|<span data-ttu-id="27b35-128">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="27b35-128">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="27b35-129">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="27b35-129">formulasLocal</span></span>|<span data-ttu-id="27b35-130">Json</span><span class="sxs-lookup"><span data-stu-id="27b35-130">Json</span></span>|<span data-ttu-id="27b35-p102">Представляет формулу в формате A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула "=SUM(A1, 1.5)" превратится в "=СУММ(A1;1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="27b35-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="27b35-133">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="27b35-133">formulasR1C1</span></span>|<span data-ttu-id="27b35-134">Json</span><span class="sxs-lookup"><span data-stu-id="27b35-134">Json</span></span>|<span data-ttu-id="27b35-135">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="27b35-135">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="27b35-136">index</span><span class="sxs-lookup"><span data-stu-id="27b35-136">index</span></span>|<span data-ttu-id="27b35-137">Int32</span><span class="sxs-lookup"><span data-stu-id="27b35-137">Int32</span></span>|<span data-ttu-id="27b35-138">Индекс диапазона.</span><span class="sxs-lookup"><span data-stu-id="27b35-138">Index of the range.</span></span>|
|<span data-ttu-id="27b35-139">numberFormat</span><span class="sxs-lookup"><span data-stu-id="27b35-139">numberFormat</span></span>|<span data-ttu-id="27b35-140">Json</span><span class="sxs-lookup"><span data-stu-id="27b35-140">Json</span></span>|<span data-ttu-id="27b35-p103">Представляет код в числовом формате Excel для заданной ячейки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27b35-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="27b35-143">rowCount</span><span class="sxs-lookup"><span data-stu-id="27b35-143">rowCount</span></span>|<span data-ttu-id="27b35-144">Int32</span><span class="sxs-lookup"><span data-stu-id="27b35-144">Int32</span></span>|<span data-ttu-id="27b35-p104">Возвращает количество видимых строк. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27b35-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="27b35-147">text</span><span class="sxs-lookup"><span data-stu-id="27b35-147">text</span></span>|<span data-ttu-id="27b35-148">Json</span><span class="sxs-lookup"><span data-stu-id="27b35-148">Json</span></span>|<span data-ttu-id="27b35-p105">Текстовые значения указанного диапазона. Текстовое значение не зависит от ширины ячейки. Замена знака #, которая происходит в пользовательском интерфейсе Excel, не повлияет на текстовое значение, возвращаемое API. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27b35-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="27b35-153">valueTypes</span><span class="sxs-lookup"><span data-stu-id="27b35-153">valueTypes</span></span>|<span data-ttu-id="27b35-154">Json</span><span class="sxs-lookup"><span data-stu-id="27b35-154">Json</span></span>|<span data-ttu-id="27b35-p106">Представляет тип данных каждой ячейки. Только для чтения. Возможные значения: Unknown, Empty, String, Integer, Double, Boolean, Error.</span><span class="sxs-lookup"><span data-stu-id="27b35-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="27b35-158">values</span><span class="sxs-lookup"><span data-stu-id="27b35-158">values</span></span>|<span data-ttu-id="27b35-159">Json</span><span class="sxs-lookup"><span data-stu-id="27b35-159">Json</span></span>|<span data-ttu-id="27b35-p107">Представляет необработанные значения указанного объекта rangeView. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="27b35-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="27b35-163">Связи</span><span class="sxs-lookup"><span data-stu-id="27b35-163">Relationships</span></span>
| <span data-ttu-id="27b35-164">Связь</span><span class="sxs-lookup"><span data-stu-id="27b35-164">Relationship</span></span> | <span data-ttu-id="27b35-165">Тип</span><span class="sxs-lookup"><span data-stu-id="27b35-165">Type</span></span>   |<span data-ttu-id="27b35-166">Описание</span><span class="sxs-lookup"><span data-stu-id="27b35-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27b35-167">rows</span><span class="sxs-lookup"><span data-stu-id="27b35-167">rows</span></span>|<span data-ttu-id="27b35-168">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="27b35-168">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="27b35-p108">Представляет коллекцию видимых ячеек в диапазоне, сопоставленных с указанным диапазоном. Только для чтения.    Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27b35-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27b35-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27b35-172">JSON representation</span></span>
<span data-ttu-id="27b35-173">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27b35-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookrangeview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
