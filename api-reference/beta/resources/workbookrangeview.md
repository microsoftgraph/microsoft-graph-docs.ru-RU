---
title: Тип ресурсов rangeView
description: Объект rangeView представляет набор видимых ячеек в родительском диапазоне.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c356c737946dc70c6718b71c1c9aa7081069fd96
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859005"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="8d698-103">Тип ресурсов rangeView</span><span class="sxs-lookup"><span data-stu-id="8d698-103">rangeView resource type</span></span>

> <span data-ttu-id="8d698-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8d698-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d698-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d698-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d698-106">Объект rangeView представляет набор видимых ячеек в родительском диапазоне.</span><span class="sxs-lookup"><span data-stu-id="8d698-106">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="8d698-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8d698-107">Methods</span></span>

| <span data-ttu-id="8d698-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8d698-108">Method</span></span>           | <span data-ttu-id="8d698-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8d698-109">Return Type</span></span>    |<span data-ttu-id="8d698-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8d698-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d698-111">[Получение списка строк](../api/workbookrangeview-list-rows.md) </span><span class="sxs-lookup"><span data-stu-id="8d698-111">[List rows](../api/workbookrangeview-list-rows.md)</span></span> |<span data-ttu-id="8d698-112">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="8d698-112">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="8d698-113">Получение коллекции объектов workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="8d698-113">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="8d698-114">Itemat</span><span class="sxs-lookup"><span data-stu-id="8d698-114">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="8d698-115">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="8d698-115">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="8d698-116">Получение видимой ячейки из диапазона с учетом индекса.</span><span class="sxs-lookup"><span data-stu-id="8d698-116">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="8d698-117">Диапазон</span><span class="sxs-lookup"><span data-stu-id="8d698-117">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="8d698-118">workbookRange</span><span class="sxs-lookup"><span data-stu-id="8d698-118">workbookRange</span></span>](range.md)|<span data-ttu-id="8d698-119">Возвращение экземпляра range, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="8d698-119">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="8d698-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d698-120">Properties</span></span>
| <span data-ttu-id="8d698-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d698-121">Property</span></span>     | <span data-ttu-id="8d698-122">Тип</span><span class="sxs-lookup"><span data-stu-id="8d698-122">Type</span></span>   |<span data-ttu-id="8d698-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8d698-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d698-124">columnCount</span><span class="sxs-lookup"><span data-stu-id="8d698-124">columnCount</span></span>|<span data-ttu-id="8d698-125">Int32</span><span class="sxs-lookup"><span data-stu-id="8d698-125">Int32</span></span>|<span data-ttu-id="8d698-p102">Возвращает количество видимых столбцов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d698-p102">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="8d698-128">formulas</span><span class="sxs-lookup"><span data-stu-id="8d698-128">formulas</span></span>|<span data-ttu-id="8d698-129">Json</span><span class="sxs-lookup"><span data-stu-id="8d698-129">Json</span></span>|<span data-ttu-id="8d698-130">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="8d698-130">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="8d698-131">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="8d698-131">formulasLocal</span></span>|<span data-ttu-id="8d698-132">Json</span><span class="sxs-lookup"><span data-stu-id="8d698-132">Json</span></span>|<span data-ttu-id="8d698-p103">Представляет формулу в формате A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула "=SUM(A1, 1.5)" превратится в "=СУММ(A1;1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="8d698-p103">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="8d698-135">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="8d698-135">formulasR1C1</span></span>|<span data-ttu-id="8d698-136">Json</span><span class="sxs-lookup"><span data-stu-id="8d698-136">Json</span></span>|<span data-ttu-id="8d698-137">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="8d698-137">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="8d698-138">index</span><span class="sxs-lookup"><span data-stu-id="8d698-138">index</span></span>|<span data-ttu-id="8d698-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8d698-139">Int32</span></span>|<span data-ttu-id="8d698-140">Индекс диапазона.</span><span class="sxs-lookup"><span data-stu-id="8d698-140">Index of the range.</span></span>|
|<span data-ttu-id="8d698-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="8d698-141">numberFormat</span></span>|<span data-ttu-id="8d698-142">Json</span><span class="sxs-lookup"><span data-stu-id="8d698-142">Json</span></span>|<span data-ttu-id="8d698-p104">Представляет код в числовом формате Excel для заданной ячейки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d698-p104">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="8d698-145">rowCount</span><span class="sxs-lookup"><span data-stu-id="8d698-145">rowCount</span></span>|<span data-ttu-id="8d698-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8d698-146">Int32</span></span>|<span data-ttu-id="8d698-p105">Возвращает количество видимых строк. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d698-p105">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="8d698-149">text</span><span class="sxs-lookup"><span data-stu-id="8d698-149">text</span></span>|<span data-ttu-id="8d698-150">Json</span><span class="sxs-lookup"><span data-stu-id="8d698-150">Json</span></span>|<span data-ttu-id="8d698-p106">Текстовые значения указанного диапазона. Текстовое значение не зависит от ширины ячейки. Замена знака #, которая происходит в пользовательском интерфейсе Excel, не повлияет на текстовое значение, возвращаемое API. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d698-p106">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="8d698-155">valueTypes</span><span class="sxs-lookup"><span data-stu-id="8d698-155">valueTypes</span></span>|<span data-ttu-id="8d698-156">Json</span><span class="sxs-lookup"><span data-stu-id="8d698-156">Json</span></span>|<span data-ttu-id="8d698-p107">Представляет тип данных каждой ячейки. Только для чтения. Возможные значения: Unknown, Empty, String, Integer, Double, Boolean, Error.</span><span class="sxs-lookup"><span data-stu-id="8d698-p107">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="8d698-160">values</span><span class="sxs-lookup"><span data-stu-id="8d698-160">values</span></span>|<span data-ttu-id="8d698-161">Json</span><span class="sxs-lookup"><span data-stu-id="8d698-161">Json</span></span>|<span data-ttu-id="8d698-p108">Представляет необработанные значения указанного объекта rangeView. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="8d698-p108">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="8d698-165">Связи</span><span class="sxs-lookup"><span data-stu-id="8d698-165">Relationships</span></span>
| <span data-ttu-id="8d698-166">Связь</span><span class="sxs-lookup"><span data-stu-id="8d698-166">Relationship</span></span> | <span data-ttu-id="8d698-167">Тип</span><span class="sxs-lookup"><span data-stu-id="8d698-167">Type</span></span>   |<span data-ttu-id="8d698-168">Описание</span><span class="sxs-lookup"><span data-stu-id="8d698-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d698-169">rows</span><span class="sxs-lookup"><span data-stu-id="8d698-169">rows</span></span>|<span data-ttu-id="8d698-170">Коллекция [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="8d698-170">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="8d698-p109">Представляет коллекцию видимых ячеек в диапазоне, сопоставленных с указанным диапазоном. Только для чтения.    Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d698-p109">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d698-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d698-174">JSON representation</span></span>
<span data-ttu-id="8d698-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d698-175">Here is a JSON representation of the resource.</span></span>
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
