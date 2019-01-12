---
title: Тип ресурсов rangeView
description: Объект rangeView представляет набор видимых ячеек в родительском диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9476b3f4a085f70be51d81a9da667c07db3b9232
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983718"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="c3101-103">Тип ресурсов rangeView</span><span class="sxs-lookup"><span data-stu-id="c3101-103">rangeView resource type</span></span>

> <span data-ttu-id="c3101-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c3101-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3101-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3101-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3101-106">Объект rangeView представляет набор видимых ячеек в родительском диапазоне.</span><span class="sxs-lookup"><span data-stu-id="c3101-106">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="c3101-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c3101-107">Methods</span></span>

| <span data-ttu-id="c3101-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c3101-108">Method</span></span>           | <span data-ttu-id="c3101-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c3101-109">Return Type</span></span>    |<span data-ttu-id="c3101-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c3101-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3101-111">[Получение списка строк](../api/workbookrangeview-list-rows.md) </span><span class="sxs-lookup"><span data-stu-id="c3101-111">[List rows](../api/workbookrangeview-list-rows.md)</span></span> |<span data-ttu-id="c3101-112">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="c3101-112">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="c3101-113">Получение коллекции объектов workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="c3101-113">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="c3101-114">Itemat</span><span class="sxs-lookup"><span data-stu-id="c3101-114">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="c3101-115">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="c3101-115">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="c3101-116">Получение видимой ячейки из диапазона с учетом индекса.</span><span class="sxs-lookup"><span data-stu-id="c3101-116">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="c3101-117">Диапазон</span><span class="sxs-lookup"><span data-stu-id="c3101-117">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="c3101-118">workbookRange</span><span class="sxs-lookup"><span data-stu-id="c3101-118">workbookRange</span></span>](range.md)|<span data-ttu-id="c3101-119">Возвращение экземпляра range, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="c3101-119">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="c3101-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3101-120">Properties</span></span>
| <span data-ttu-id="c3101-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3101-121">Property</span></span>     | <span data-ttu-id="c3101-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c3101-122">Type</span></span>   |<span data-ttu-id="c3101-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c3101-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3101-124">columnCount</span><span class="sxs-lookup"><span data-stu-id="c3101-124">columnCount</span></span>|<span data-ttu-id="c3101-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c3101-125">Int32</span></span>|<span data-ttu-id="c3101-p102">Возвращает количество видимых столбцов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3101-p102">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="c3101-128">formulas</span><span class="sxs-lookup"><span data-stu-id="c3101-128">formulas</span></span>|<span data-ttu-id="c3101-129">Json</span><span class="sxs-lookup"><span data-stu-id="c3101-129">Json</span></span>|<span data-ttu-id="c3101-130">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="c3101-130">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="c3101-131">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="c3101-131">formulasLocal</span></span>|<span data-ttu-id="c3101-132">Json</span><span class="sxs-lookup"><span data-stu-id="c3101-132">Json</span></span>|<span data-ttu-id="c3101-p103">Представляет формулу в формате A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула "=SUM(A1, 1.5)" превратится в "=СУММ(A1;1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="c3101-p103">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="c3101-135">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="c3101-135">formulasR1C1</span></span>|<span data-ttu-id="c3101-136">Json</span><span class="sxs-lookup"><span data-stu-id="c3101-136">Json</span></span>|<span data-ttu-id="c3101-137">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="c3101-137">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="c3101-138">index</span><span class="sxs-lookup"><span data-stu-id="c3101-138">index</span></span>|<span data-ttu-id="c3101-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c3101-139">Int32</span></span>|<span data-ttu-id="c3101-140">Индекс диапазона.</span><span class="sxs-lookup"><span data-stu-id="c3101-140">Index of the range.</span></span>|
|<span data-ttu-id="c3101-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="c3101-141">numberFormat</span></span>|<span data-ttu-id="c3101-142">Json</span><span class="sxs-lookup"><span data-stu-id="c3101-142">Json</span></span>|<span data-ttu-id="c3101-p104">Представляет код в числовом формате Excel для заданной ячейки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3101-p104">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="c3101-145">rowCount</span><span class="sxs-lookup"><span data-stu-id="c3101-145">rowCount</span></span>|<span data-ttu-id="c3101-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c3101-146">Int32</span></span>|<span data-ttu-id="c3101-p105">Возвращает количество видимых строк. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3101-p105">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="c3101-149">text</span><span class="sxs-lookup"><span data-stu-id="c3101-149">text</span></span>|<span data-ttu-id="c3101-150">Json</span><span class="sxs-lookup"><span data-stu-id="c3101-150">Json</span></span>|<span data-ttu-id="c3101-p106">Текстовые значения указанного диапазона. Текстовое значение не зависит от ширины ячейки. Замена знака #, которая происходит в пользовательском интерфейсе Excel, не повлияет на текстовое значение, возвращаемое API. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3101-p106">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="c3101-155">valueTypes</span><span class="sxs-lookup"><span data-stu-id="c3101-155">valueTypes</span></span>|<span data-ttu-id="c3101-156">Json</span><span class="sxs-lookup"><span data-stu-id="c3101-156">Json</span></span>|<span data-ttu-id="c3101-p107">Представляет тип данных каждой ячейки. Только для чтения. Возможные значения: Unknown, Empty, String, Integer, Double, Boolean, Error.</span><span class="sxs-lookup"><span data-stu-id="c3101-p107">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="c3101-160">values</span><span class="sxs-lookup"><span data-stu-id="c3101-160">values</span></span>|<span data-ttu-id="c3101-161">Json</span><span class="sxs-lookup"><span data-stu-id="c3101-161">Json</span></span>|<span data-ttu-id="c3101-p108">Представляет необработанные значения указанного объекта rangeView. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="c3101-p108">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="c3101-165">Связи</span><span class="sxs-lookup"><span data-stu-id="c3101-165">Relationships</span></span>
| <span data-ttu-id="c3101-166">Связь</span><span class="sxs-lookup"><span data-stu-id="c3101-166">Relationship</span></span> | <span data-ttu-id="c3101-167">Тип</span><span class="sxs-lookup"><span data-stu-id="c3101-167">Type</span></span>   |<span data-ttu-id="c3101-168">Описание</span><span class="sxs-lookup"><span data-stu-id="c3101-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3101-169">rows</span><span class="sxs-lookup"><span data-stu-id="c3101-169">rows</span></span>|<span data-ttu-id="c3101-170">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="c3101-170">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="c3101-p109">Представляет коллекцию видимых ячеек в диапазоне, сопоставленных с указанным диапазоном. Только для чтения.    Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3101-p109">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3101-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3101-174">JSON representation</span></span>
<span data-ttu-id="c3101-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3101-175">Here is a JSON representation of the resource.</span></span>
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
