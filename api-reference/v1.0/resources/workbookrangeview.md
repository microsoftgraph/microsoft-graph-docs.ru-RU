---
title: Тип ресурсов rangeView
description: Объект rangeView представляет набор видимых ячеек в родительском диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a216de96ba97e079efc1cfc034b00ddd027c9b1d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446718"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="fd69a-103">Тип ресурсов rangeView</span><span class="sxs-lookup"><span data-stu-id="fd69a-103">rangeView resource type</span></span>

<span data-ttu-id="fd69a-104">Пространство имен: Microsoft. Graph RangeView представляет набор видимых ячеек родительского диапазона.</span><span class="sxs-lookup"><span data-stu-id="fd69a-104">Namespace: microsoft.graph RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="fd69a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="fd69a-105">Methods</span></span>

| <span data-ttu-id="fd69a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="fd69a-106">Method</span></span>           | <span data-ttu-id="fd69a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fd69a-107">Return Type</span></span>    |<span data-ttu-id="fd69a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fd69a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd69a-109">Получение списка строк</span><span class="sxs-lookup"><span data-stu-id="fd69a-109">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="fd69a-110">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="fd69a-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="fd69a-111">Получение коллекции объектов workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="fd69a-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="fd69a-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="fd69a-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="fd69a-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="fd69a-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="fd69a-114">Получение видимой ячейки из диапазона с учетом индекса.</span><span class="sxs-lookup"><span data-stu-id="fd69a-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="fd69a-115">Диапазон</span><span class="sxs-lookup"><span data-stu-id="fd69a-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="fd69a-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="fd69a-116">workbookRange</span></span>](range.md)|<span data-ttu-id="fd69a-117">Возвращение экземпляра range, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="fd69a-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="fd69a-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd69a-118">Properties</span></span>
| <span data-ttu-id="fd69a-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd69a-119">Property</span></span>     | <span data-ttu-id="fd69a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fd69a-120">Type</span></span>   |<span data-ttu-id="fd69a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fd69a-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd69a-122">cellAddresses</span><span class="sxs-lookup"><span data-stu-id="fd69a-122">cellAddresses</span></span>|<span data-ttu-id="fd69a-123">Json</span><span class="sxs-lookup"><span data-stu-id="fd69a-123">Json</span></span>|<span data-ttu-id="fd69a-124">Представляет адреса ячеек</span><span class="sxs-lookup"><span data-stu-id="fd69a-124">Represents the cell addresses</span></span>
|<span data-ttu-id="fd69a-125">columnCount</span><span class="sxs-lookup"><span data-stu-id="fd69a-125">columnCount</span></span>|<span data-ttu-id="fd69a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="fd69a-126">Int32</span></span>|<span data-ttu-id="fd69a-p101">Возвращает количество видимых столбцов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd69a-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="fd69a-129">formulas</span><span class="sxs-lookup"><span data-stu-id="fd69a-129">formulas</span></span>|<span data-ttu-id="fd69a-130">Json</span><span class="sxs-lookup"><span data-stu-id="fd69a-130">Json</span></span>|<span data-ttu-id="fd69a-131">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="fd69a-131">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="fd69a-132">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="fd69a-132">formulasLocal</span></span>|<span data-ttu-id="fd69a-133">Json</span><span class="sxs-lookup"><span data-stu-id="fd69a-133">Json</span></span>|<span data-ttu-id="fd69a-p102">Представляет формулу в формате A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула "=SUM(A1, 1.5)" превратится в "=СУММ(A1;1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="fd69a-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="fd69a-136">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="fd69a-136">formulasR1C1</span></span>|<span data-ttu-id="fd69a-137">Json</span><span class="sxs-lookup"><span data-stu-id="fd69a-137">Json</span></span>|<span data-ttu-id="fd69a-138">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="fd69a-138">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="fd69a-139">index</span><span class="sxs-lookup"><span data-stu-id="fd69a-139">index</span></span>|<span data-ttu-id="fd69a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fd69a-140">Int32</span></span>|<span data-ttu-id="fd69a-141">Индекс диапазона.</span><span class="sxs-lookup"><span data-stu-id="fd69a-141">Index of the range.</span></span>|
|<span data-ttu-id="fd69a-142">numberFormat</span><span class="sxs-lookup"><span data-stu-id="fd69a-142">numberFormat</span></span>|<span data-ttu-id="fd69a-143">Json</span><span class="sxs-lookup"><span data-stu-id="fd69a-143">Json</span></span>|<span data-ttu-id="fd69a-p103">Представляет код в числовом формате Excel для заданной ячейки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd69a-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="fd69a-146">rowCount</span><span class="sxs-lookup"><span data-stu-id="fd69a-146">rowCount</span></span>|<span data-ttu-id="fd69a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="fd69a-147">Int32</span></span>|<span data-ttu-id="fd69a-p104">Возвращает количество видимых строк. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd69a-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="fd69a-150">текст</span><span class="sxs-lookup"><span data-stu-id="fd69a-150">text</span></span>|<span data-ttu-id="fd69a-151">Json</span><span class="sxs-lookup"><span data-stu-id="fd69a-151">Json</span></span>|<span data-ttu-id="fd69a-p105">Текстовые значения указанного диапазона. Текстовое значение не зависит от ширины ячейки. Замена знака #, которая происходит в пользовательском интерфейсе Excel, не повлияет на текстовое значение, возвращаемое API. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd69a-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="fd69a-156">valueTypes</span><span class="sxs-lookup"><span data-stu-id="fd69a-156">valueTypes</span></span>|<span data-ttu-id="fd69a-157">Json</span><span class="sxs-lookup"><span data-stu-id="fd69a-157">Json</span></span>|<span data-ttu-id="fd69a-158">Представляет тип данных каждой ячейки.</span><span class="sxs-lookup"><span data-stu-id="fd69a-158">Represents the type of data of each cell.</span></span> <span data-ttu-id="fd69a-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd69a-159">Read-only.</span></span> <span data-ttu-id="fd69a-160">Возможные значения: Unknown, Empty, String, Integer, Double, Boolean, Error.</span><span class="sxs-lookup"><span data-stu-id="fd69a-160">The possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="fd69a-161">values</span><span class="sxs-lookup"><span data-stu-id="fd69a-161">values</span></span>|<span data-ttu-id="fd69a-162">Json</span><span class="sxs-lookup"><span data-stu-id="fd69a-162">Json</span></span>|<span data-ttu-id="fd69a-p107">Представляет необработанные значения указанного объекта rangeView. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="fd69a-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="fd69a-166">Связи</span><span class="sxs-lookup"><span data-stu-id="fd69a-166">Relationships</span></span>
| <span data-ttu-id="fd69a-167">Связь</span><span class="sxs-lookup"><span data-stu-id="fd69a-167">Relationship</span></span> | <span data-ttu-id="fd69a-168">Тип</span><span class="sxs-lookup"><span data-stu-id="fd69a-168">Type</span></span>   |<span data-ttu-id="fd69a-169">Описание</span><span class="sxs-lookup"><span data-stu-id="fd69a-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd69a-170">rows</span><span class="sxs-lookup"><span data-stu-id="fd69a-170">rows</span></span>|<span data-ttu-id="fd69a-171">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="fd69a-171">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="fd69a-p108">Представляет коллекцию видимых ячеек в диапазоне, сопоставленных с указанным диапазоном. Только для чтения.    Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd69a-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd69a-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd69a-175">JSON representation</span></span>
<span data-ttu-id="fd69a-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd69a-176">Here is a JSON representation of the resource.</span></span>
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
