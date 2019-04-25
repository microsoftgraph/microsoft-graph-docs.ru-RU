---
title: Тип ресурса TableSort
description: Управляет операциями сортировки для объектов Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: be607832be82b99853b4cd44cfa5b60449a2c432
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534516"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="e5390-103">Тип ресурса TableSort</span><span class="sxs-lookup"><span data-stu-id="e5390-103">TableSort resource type</span></span>

<span data-ttu-id="e5390-104">Управляет операциями сортировки для объектов Table.</span><span class="sxs-lookup"><span data-stu-id="e5390-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="e5390-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e5390-105">Methods</span></span>

| <span data-ttu-id="e5390-106">Метод</span><span class="sxs-lookup"><span data-stu-id="e5390-106">Method</span></span>           | <span data-ttu-id="e5390-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e5390-107">Return Type</span></span>    |<span data-ttu-id="e5390-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e5390-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5390-109">Получение объекта TableSort</span><span class="sxs-lookup"><span data-stu-id="e5390-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="e5390-110">Воркбуктаблесорт</span><span class="sxs-lookup"><span data-stu-id="e5390-110">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="e5390-111">Чтение свойств и связей объекта tableSort.</span><span class="sxs-lookup"><span data-stu-id="e5390-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="e5390-112">Apply</span><span class="sxs-lookup"><span data-stu-id="e5390-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="e5390-113">Нет</span><span class="sxs-lookup"><span data-stu-id="e5390-113">None</span></span>|<span data-ttu-id="e5390-114">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="e5390-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="e5390-115">Clear</span><span class="sxs-lookup"><span data-stu-id="e5390-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="e5390-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e5390-116">None</span></span>|<span data-ttu-id="e5390-p101">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="e5390-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="e5390-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="e5390-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="e5390-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e5390-120">None</span></span>|<span data-ttu-id="e5390-121">Повторно применяет текущие параметры сортировки к таблице.</span><span class="sxs-lookup"><span data-stu-id="e5390-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5390-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5390-122">Properties</span></span>
| <span data-ttu-id="e5390-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5390-123">Property</span></span>     | <span data-ttu-id="e5390-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e5390-124">Type</span></span>   |<span data-ttu-id="e5390-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e5390-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5390-126">fields</span><span class="sxs-lookup"><span data-stu-id="e5390-126">fields</span></span>|<span data-ttu-id="e5390-127">Коллекция [воркбуксортфиелд](sortfield.md)</span><span class="sxs-lookup"><span data-stu-id="e5390-127">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="e5390-128">Указывает текущие условия, которые использовались при последней сортировке таблицы.</span><span class="sxs-lookup"><span data-stu-id="e5390-128">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="e5390-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5390-129">Read-only.</span></span>|
|<span data-ttu-id="e5390-130">matchCase</span><span class="sxs-lookup"><span data-stu-id="e5390-130">matchCase</span></span>|<span data-ttu-id="e5390-131">boolean</span><span class="sxs-lookup"><span data-stu-id="e5390-131">boolean</span></span>|<span data-ttu-id="e5390-p103">Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5390-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="e5390-134">method</span><span class="sxs-lookup"><span data-stu-id="e5390-134">method</span></span>|<span data-ttu-id="e5390-135">string</span><span class="sxs-lookup"><span data-stu-id="e5390-135">string</span></span>|<span data-ttu-id="e5390-136">Указывает метод сортировки китайских символов, который использовался при последней сортировке таблицы.</span><span class="sxs-lookup"><span data-stu-id="e5390-136">Represents Chinese character ordering method last used to sort the table.</span></span> <span data-ttu-id="e5390-137">Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="e5390-137">The possible values are: `PinYin`, `StrokeCount`.</span></span> <span data-ttu-id="e5390-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5390-138">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5390-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e5390-139">JSON representation</span></span>

<span data-ttu-id="e5390-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5390-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
