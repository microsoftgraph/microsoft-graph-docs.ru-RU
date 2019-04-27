---
title: Тип ресурса Воркбуктаблесорт
description: Управляет операциями сортировки для объектов Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6ba1e7cdcf48a3ac5cf8262be2174481016aad2e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348960"
---
# <a name="workbooktablesort-resource-type"></a><span data-ttu-id="fe109-103">Тип ресурса Воркбуктаблесорт</span><span class="sxs-lookup"><span data-stu-id="fe109-103">workbookTableSort resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe109-104">Управляет операциями сортировки для объектов Table.</span><span class="sxs-lookup"><span data-stu-id="fe109-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="fe109-105">Методы</span><span class="sxs-lookup"><span data-stu-id="fe109-105">Methods</span></span>

| <span data-ttu-id="fe109-106">Метод</span><span class="sxs-lookup"><span data-stu-id="fe109-106">Method</span></span>           | <span data-ttu-id="fe109-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fe109-107">Return Type</span></span>    |<span data-ttu-id="fe109-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fe109-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe109-109">Получение объекта TableSort</span><span class="sxs-lookup"><span data-stu-id="fe109-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="fe109-110">Воркбуктаблесорт</span><span class="sxs-lookup"><span data-stu-id="fe109-110">workbookTableSort</span></span>](workbooktablesort.md) |<span data-ttu-id="fe109-111">Чтение свойств и связей объекта tableSort.</span><span class="sxs-lookup"><span data-stu-id="fe109-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="fe109-112">Apply</span><span class="sxs-lookup"><span data-stu-id="fe109-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="fe109-113">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="fe109-113">None</span></span>|<span data-ttu-id="fe109-114">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="fe109-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="fe109-115">Clear</span><span class="sxs-lookup"><span data-stu-id="fe109-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="fe109-116">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="fe109-116">None</span></span>|<span data-ttu-id="fe109-p101">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="fe109-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="fe109-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="fe109-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="fe109-120">Нет</span><span class="sxs-lookup"><span data-stu-id="fe109-120">None</span></span>|<span data-ttu-id="fe109-121">Повторно применяет текущие параметры сортировки к таблице.</span><span class="sxs-lookup"><span data-stu-id="fe109-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="fe109-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe109-122">Properties</span></span>
| <span data-ttu-id="fe109-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe109-123">Property</span></span>     | <span data-ttu-id="fe109-124">Тип</span><span class="sxs-lookup"><span data-stu-id="fe109-124">Type</span></span>   |<span data-ttu-id="fe109-125">Описание</span><span class="sxs-lookup"><span data-stu-id="fe109-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe109-126">matchCase</span><span class="sxs-lookup"><span data-stu-id="fe109-126">matchCase</span></span>|<span data-ttu-id="fe109-127">boolean</span><span class="sxs-lookup"><span data-stu-id="fe109-127">boolean</span></span>|<span data-ttu-id="fe109-p102">Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe109-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="fe109-130">method</span><span class="sxs-lookup"><span data-stu-id="fe109-130">method</span></span>|<span data-ttu-id="fe109-131">string</span><span class="sxs-lookup"><span data-stu-id="fe109-131">string</span></span>|<span data-ttu-id="fe109-p103">Указывает метод сортировки китайских символов, который использовался при последней сортировке таблицы. Возможные значения: `PinYin`, `StrokeCount`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe109-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe109-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="fe109-135">Relationships</span></span>
| <span data-ttu-id="fe109-136">Отношение</span><span class="sxs-lookup"><span data-stu-id="fe109-136">Relationship</span></span> | <span data-ttu-id="fe109-137">Тип</span><span class="sxs-lookup"><span data-stu-id="fe109-137">Type</span></span>   |<span data-ttu-id="fe109-138">Описание</span><span class="sxs-lookup"><span data-stu-id="fe109-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe109-139">fields</span><span class="sxs-lookup"><span data-stu-id="fe109-139">fields</span></span>|[<span data-ttu-id="fe109-140">Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="fe109-140">workbookSortField</span></span>](workbooksortfield.md)|<span data-ttu-id="fe109-141">Указывает текущие условия, которые использовались при последней сортировке таблицы.</span><span class="sxs-lookup"><span data-stu-id="fe109-141">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="fe109-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe109-142">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe109-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe109-143">JSON representation</span></span>

<span data-ttu-id="fe109-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe109-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
 
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "id": "string",
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
