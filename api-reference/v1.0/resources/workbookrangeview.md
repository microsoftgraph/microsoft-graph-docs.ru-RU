---
title: Тип ресурсов rangeView
description: Объект rangeView представляет набор видимых ячеек в родительском диапазоне.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 0fae95999de35b5bac42716a4c9ec8b16a5b1158
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810082"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="00add-103">Тип ресурсов rangeView</span><span class="sxs-lookup"><span data-stu-id="00add-103">rangeView resource type</span></span>
<span data-ttu-id="00add-104">Объект rangeView представляет набор видимых ячеек в родительском диапазоне.</span><span class="sxs-lookup"><span data-stu-id="00add-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="00add-105">Методы</span><span class="sxs-lookup"><span data-stu-id="00add-105">Methods</span></span>

| <span data-ttu-id="00add-106">Метод</span><span class="sxs-lookup"><span data-stu-id="00add-106">Method</span></span>           | <span data-ttu-id="00add-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="00add-107">Return Type</span></span>    |<span data-ttu-id="00add-108">Описание</span><span class="sxs-lookup"><span data-stu-id="00add-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00add-109">[Получение списка строк](../api/workbookrangeview-list-rows.md) </span><span class="sxs-lookup"><span data-stu-id="00add-109">[List rows](../api/workbookrangeview-list-rows.md)</span></span> |<span data-ttu-id="00add-110">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="00add-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="00add-111">Получение коллекции объектов workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="00add-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="00add-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="00add-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="00add-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="00add-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="00add-114">Получение видимой ячейки из диапазона с учетом индекса.</span><span class="sxs-lookup"><span data-stu-id="00add-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="00add-115">Диапазон</span><span class="sxs-lookup"><span data-stu-id="00add-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="00add-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="00add-116">workbookRange</span></span>](range.md)|<span data-ttu-id="00add-117">Возвращение экземпляра range, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="00add-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="00add-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="00add-118">Properties</span></span>
| <span data-ttu-id="00add-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="00add-119">Property</span></span>     | <span data-ttu-id="00add-120">Тип</span><span class="sxs-lookup"><span data-stu-id="00add-120">Type</span></span>   |<span data-ttu-id="00add-121">Описание</span><span class="sxs-lookup"><span data-stu-id="00add-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00add-122">cellAddresses</span><span class="sxs-lookup"><span data-stu-id="00add-122">cellAddresses</span></span>|<span data-ttu-id="00add-123">Json</span><span class="sxs-lookup"><span data-stu-id="00add-123">Json</span></span>|<span data-ttu-id="00add-124">Представляет адреса ячеек</span><span class="sxs-lookup"><span data-stu-id="00add-124">Represents the cell addresses</span></span>
|<span data-ttu-id="00add-125">columnCount</span><span class="sxs-lookup"><span data-stu-id="00add-125">columnCount</span></span>|<span data-ttu-id="00add-126">Int32</span><span class="sxs-lookup"><span data-stu-id="00add-126">Int32</span></span>|<span data-ttu-id="00add-p101">Возвращает количество видимых столбцов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00add-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="00add-129">formulas</span><span class="sxs-lookup"><span data-stu-id="00add-129">formulas</span></span>|<span data-ttu-id="00add-130">Json</span><span class="sxs-lookup"><span data-stu-id="00add-130">Json</span></span>|<span data-ttu-id="00add-131">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="00add-131">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="00add-132">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="00add-132">formulasLocal</span></span>|<span data-ttu-id="00add-133">Json</span><span class="sxs-lookup"><span data-stu-id="00add-133">Json</span></span>|<span data-ttu-id="00add-p102">Представляет формулу в формате A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула "=SUM(A1, 1.5)" превратится в "=СУММ(A1;1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="00add-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="00add-136">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="00add-136">formulasR1C1</span></span>|<span data-ttu-id="00add-137">Json</span><span class="sxs-lookup"><span data-stu-id="00add-137">Json</span></span>|<span data-ttu-id="00add-138">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="00add-138">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="00add-139">index</span><span class="sxs-lookup"><span data-stu-id="00add-139">index</span></span>|<span data-ttu-id="00add-140">Int32</span><span class="sxs-lookup"><span data-stu-id="00add-140">Int32</span></span>|<span data-ttu-id="00add-141">Индекс диапазона.</span><span class="sxs-lookup"><span data-stu-id="00add-141">Index of the range.</span></span>|
|<span data-ttu-id="00add-142">numberFormat</span><span class="sxs-lookup"><span data-stu-id="00add-142">numberFormat</span></span>|<span data-ttu-id="00add-143">Json</span><span class="sxs-lookup"><span data-stu-id="00add-143">Json</span></span>|<span data-ttu-id="00add-p103">Представляет код в числовом формате Excel для заданной ячейки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00add-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="00add-146">rowCount</span><span class="sxs-lookup"><span data-stu-id="00add-146">rowCount</span></span>|<span data-ttu-id="00add-147">Int32</span><span class="sxs-lookup"><span data-stu-id="00add-147">Int32</span></span>|<span data-ttu-id="00add-p104">Возвращает количество видимых строк. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00add-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="00add-150">text</span><span class="sxs-lookup"><span data-stu-id="00add-150">text</span></span>|<span data-ttu-id="00add-151">Json</span><span class="sxs-lookup"><span data-stu-id="00add-151">Json</span></span>|<span data-ttu-id="00add-p105">Текстовые значения указанного диапазона. Текстовое значение не зависит от ширины ячейки. Замена знака #, которая происходит в пользовательском интерфейсе Excel, не повлияет на текстовое значение, возвращаемое API. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00add-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="00add-156">valueTypes</span><span class="sxs-lookup"><span data-stu-id="00add-156">valueTypes</span></span>|<span data-ttu-id="00add-157">Json</span><span class="sxs-lookup"><span data-stu-id="00add-157">Json</span></span>|<span data-ttu-id="00add-158">Представляет тип данных для каждой ячейки.</span><span class="sxs-lookup"><span data-stu-id="00add-158">Represents the type of data of each cell.</span></span> <span data-ttu-id="00add-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00add-159">Read-only.</span></span> <span data-ttu-id="00add-160">Возможные значения: неизвестно, пустой, строка, целое число, двойное, Boolean, ошибка.</span><span class="sxs-lookup"><span data-stu-id="00add-160">The possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="00add-161">values</span><span class="sxs-lookup"><span data-stu-id="00add-161">values</span></span>|<span data-ttu-id="00add-162">Json</span><span class="sxs-lookup"><span data-stu-id="00add-162">Json</span></span>|<span data-ttu-id="00add-p107">Представляет необработанные значения указанного объекта rangeView. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="00add-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="00add-166">Связи</span><span class="sxs-lookup"><span data-stu-id="00add-166">Relationships</span></span>
| <span data-ttu-id="00add-167">Связь</span><span class="sxs-lookup"><span data-stu-id="00add-167">Relationship</span></span> | <span data-ttu-id="00add-168">Тип</span><span class="sxs-lookup"><span data-stu-id="00add-168">Type</span></span>   |<span data-ttu-id="00add-169">Описание</span><span class="sxs-lookup"><span data-stu-id="00add-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00add-170">rows</span><span class="sxs-lookup"><span data-stu-id="00add-170">rows</span></span>|<span data-ttu-id="00add-171">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="00add-171">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="00add-p108">Представляет коллекцию видимых ячеек в диапазоне, сопоставленных с указанным диапазоном. Только для чтения.    Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00add-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00add-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00add-175">JSON representation</span></span>
<span data-ttu-id="00add-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00add-176">Here is a JSON representation of the resource.</span></span>
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
