---
title: Тип ресурсов rangeView
description: Объект rangeView представляет набор видимых ячеек в родительском диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 745ed45b4e5b79c8d1764a86fac04cf7fcfdcc26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957804"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="26197-103">Тип ресурсов rangeView</span><span class="sxs-lookup"><span data-stu-id="26197-103">rangeView resource type</span></span>
<span data-ttu-id="26197-104">Объект rangeView представляет набор видимых ячеек в родительском диапазоне.</span><span class="sxs-lookup"><span data-stu-id="26197-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="26197-105">Методы</span><span class="sxs-lookup"><span data-stu-id="26197-105">Methods</span></span>

| <span data-ttu-id="26197-106">Метод</span><span class="sxs-lookup"><span data-stu-id="26197-106">Method</span></span>           | <span data-ttu-id="26197-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="26197-107">Return Type</span></span>    |<span data-ttu-id="26197-108">Описание</span><span class="sxs-lookup"><span data-stu-id="26197-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26197-109">[Получение списка строк](../api/workbookrangeview-list-rows.md) </span><span class="sxs-lookup"><span data-stu-id="26197-109">[List rows](../api/workbookrangeview-list-rows.md)</span></span> |<span data-ttu-id="26197-110">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="26197-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="26197-111">Получение коллекции объектов workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="26197-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="26197-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="26197-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="26197-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="26197-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="26197-114">Получение видимой ячейки из диапазона с учетом индекса.</span><span class="sxs-lookup"><span data-stu-id="26197-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="26197-115">Диапазон</span><span class="sxs-lookup"><span data-stu-id="26197-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="26197-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="26197-116">workbookRange</span></span>](range.md)|<span data-ttu-id="26197-117">Возвращение экземпляра range, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="26197-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="26197-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="26197-118">Properties</span></span>
| <span data-ttu-id="26197-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="26197-119">Property</span></span>     | <span data-ttu-id="26197-120">Тип</span><span class="sxs-lookup"><span data-stu-id="26197-120">Type</span></span>   |<span data-ttu-id="26197-121">Описание</span><span class="sxs-lookup"><span data-stu-id="26197-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26197-122">cellAddresses</span><span class="sxs-lookup"><span data-stu-id="26197-122">cellAddresses</span></span>|<span data-ttu-id="26197-123">Json</span><span class="sxs-lookup"><span data-stu-id="26197-123">Json</span></span>|<span data-ttu-id="26197-124">Представляет адреса ячеек</span><span class="sxs-lookup"><span data-stu-id="26197-124">Represents the cell addresses</span></span>
|<span data-ttu-id="26197-125">columnCount</span><span class="sxs-lookup"><span data-stu-id="26197-125">columnCount</span></span>|<span data-ttu-id="26197-126">Int32</span><span class="sxs-lookup"><span data-stu-id="26197-126">Int32</span></span>|<span data-ttu-id="26197-p101">Возвращает количество видимых столбцов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26197-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="26197-129">formulas</span><span class="sxs-lookup"><span data-stu-id="26197-129">formulas</span></span>|<span data-ttu-id="26197-130">Json</span><span class="sxs-lookup"><span data-stu-id="26197-130">Json</span></span>|<span data-ttu-id="26197-131">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="26197-131">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="26197-132">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="26197-132">formulasLocal</span></span>|<span data-ttu-id="26197-133">Json</span><span class="sxs-lookup"><span data-stu-id="26197-133">Json</span></span>|<span data-ttu-id="26197-p102">Представляет формулу в формате A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула "=SUM(A1, 1.5)" превратится в "=СУММ(A1;1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="26197-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="26197-136">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="26197-136">formulasR1C1</span></span>|<span data-ttu-id="26197-137">Json</span><span class="sxs-lookup"><span data-stu-id="26197-137">Json</span></span>|<span data-ttu-id="26197-138">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="26197-138">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="26197-139">index</span><span class="sxs-lookup"><span data-stu-id="26197-139">index</span></span>|<span data-ttu-id="26197-140">Int32</span><span class="sxs-lookup"><span data-stu-id="26197-140">Int32</span></span>|<span data-ttu-id="26197-141">Индекс диапазона.</span><span class="sxs-lookup"><span data-stu-id="26197-141">Index of the range.</span></span>|
|<span data-ttu-id="26197-142">numberFormat</span><span class="sxs-lookup"><span data-stu-id="26197-142">numberFormat</span></span>|<span data-ttu-id="26197-143">Json</span><span class="sxs-lookup"><span data-stu-id="26197-143">Json</span></span>|<span data-ttu-id="26197-p103">Представляет код в числовом формате Excel для заданной ячейки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26197-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="26197-146">rowCount</span><span class="sxs-lookup"><span data-stu-id="26197-146">rowCount</span></span>|<span data-ttu-id="26197-147">Int32</span><span class="sxs-lookup"><span data-stu-id="26197-147">Int32</span></span>|<span data-ttu-id="26197-p104">Возвращает количество видимых строк. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26197-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="26197-150">text</span><span class="sxs-lookup"><span data-stu-id="26197-150">text</span></span>|<span data-ttu-id="26197-151">Json</span><span class="sxs-lookup"><span data-stu-id="26197-151">Json</span></span>|<span data-ttu-id="26197-p105">Текстовые значения указанного диапазона. Текстовое значение не зависит от ширины ячейки. Замена знака #, которая происходит в пользовательском интерфейсе Excel, не повлияет на текстовое значение, возвращаемое API. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26197-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="26197-156">valueTypes</span><span class="sxs-lookup"><span data-stu-id="26197-156">valueTypes</span></span>|<span data-ttu-id="26197-157">Json</span><span class="sxs-lookup"><span data-stu-id="26197-157">Json</span></span>|<span data-ttu-id="26197-158">Представляет тип данных для каждой ячейки.</span><span class="sxs-lookup"><span data-stu-id="26197-158">Represents the type of data of each cell.</span></span> <span data-ttu-id="26197-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26197-159">Read-only.</span></span> <span data-ttu-id="26197-160">Возможные значения: неизвестно, пустой, строка, целое число, двойное, Boolean, ошибка.</span><span class="sxs-lookup"><span data-stu-id="26197-160">The possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="26197-161">values</span><span class="sxs-lookup"><span data-stu-id="26197-161">values</span></span>|<span data-ttu-id="26197-162">Json</span><span class="sxs-lookup"><span data-stu-id="26197-162">Json</span></span>|<span data-ttu-id="26197-p107">Представляет необработанные значения указанного объекта rangeView. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="26197-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="26197-166">Связи</span><span class="sxs-lookup"><span data-stu-id="26197-166">Relationships</span></span>
| <span data-ttu-id="26197-167">Связь</span><span class="sxs-lookup"><span data-stu-id="26197-167">Relationship</span></span> | <span data-ttu-id="26197-168">Тип</span><span class="sxs-lookup"><span data-stu-id="26197-168">Type</span></span>   |<span data-ttu-id="26197-169">Описание</span><span class="sxs-lookup"><span data-stu-id="26197-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26197-170">rows</span><span class="sxs-lookup"><span data-stu-id="26197-170">rows</span></span>|<span data-ttu-id="26197-171">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="26197-171">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="26197-p108">Представляет коллекцию видимых ячеек в диапазоне, сопоставленных с указанным диапазоном. Только для чтения.    Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26197-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26197-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26197-175">JSON representation</span></span>
<span data-ttu-id="26197-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26197-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
