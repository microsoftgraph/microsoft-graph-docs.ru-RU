---
title: Тип ресурса Воркбуктаблесорт
description: Управляет операциями сортировки для объектов Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ea0332f1ad00029cf511f2bc55aca80836e5ef2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007034"
---
# <a name="workbooktablesort-resource-type"></a><span data-ttu-id="97987-103">Тип ресурса Воркбуктаблесорт</span><span class="sxs-lookup"><span data-stu-id="97987-103">workbookTableSort resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97987-104">Управляет операциями сортировки для объектов Table.</span><span class="sxs-lookup"><span data-stu-id="97987-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="97987-105">Методы</span><span class="sxs-lookup"><span data-stu-id="97987-105">Methods</span></span>

| <span data-ttu-id="97987-106">Метод</span><span class="sxs-lookup"><span data-stu-id="97987-106">Method</span></span>           | <span data-ttu-id="97987-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="97987-107">Return Type</span></span>    |<span data-ttu-id="97987-108">Описание</span><span class="sxs-lookup"><span data-stu-id="97987-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="97987-109">Получение объекта TableSort</span><span class="sxs-lookup"><span data-stu-id="97987-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="97987-110">Воркбуктаблесорт</span><span class="sxs-lookup"><span data-stu-id="97987-110">workbookTableSort</span></span>](workbooktablesort.md) |<span data-ttu-id="97987-111">Чтение свойств и связей объекта tableSort.</span><span class="sxs-lookup"><span data-stu-id="97987-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="97987-112">Apply</span><span class="sxs-lookup"><span data-stu-id="97987-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="97987-113">Нет</span><span class="sxs-lookup"><span data-stu-id="97987-113">None</span></span>|<span data-ttu-id="97987-114">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="97987-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="97987-115">Clear</span><span class="sxs-lookup"><span data-stu-id="97987-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="97987-116">Нет</span><span class="sxs-lookup"><span data-stu-id="97987-116">None</span></span>|<span data-ttu-id="97987-p101">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="97987-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="97987-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="97987-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="97987-120">Нет</span><span class="sxs-lookup"><span data-stu-id="97987-120">None</span></span>|<span data-ttu-id="97987-121">Повторно применяет текущие параметры сортировки к таблице.</span><span class="sxs-lookup"><span data-stu-id="97987-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="97987-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="97987-122">Properties</span></span>
| <span data-ttu-id="97987-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="97987-123">Property</span></span>     | <span data-ttu-id="97987-124">Тип</span><span class="sxs-lookup"><span data-stu-id="97987-124">Type</span></span>   |<span data-ttu-id="97987-125">Описание</span><span class="sxs-lookup"><span data-stu-id="97987-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97987-126">matchCase</span><span class="sxs-lookup"><span data-stu-id="97987-126">matchCase</span></span>|<span data-ttu-id="97987-127">boolean</span><span class="sxs-lookup"><span data-stu-id="97987-127">boolean</span></span>|<span data-ttu-id="97987-p102">Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97987-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="97987-130">method</span><span class="sxs-lookup"><span data-stu-id="97987-130">method</span></span>|<span data-ttu-id="97987-131">string</span><span class="sxs-lookup"><span data-stu-id="97987-131">string</span></span>|<span data-ttu-id="97987-p103">Указывает метод сортировки китайских символов, который использовался при последней сортировке таблицы. Возможные значения: `PinYin`, `StrokeCount`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97987-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97987-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="97987-135">Relationships</span></span>
| <span data-ttu-id="97987-136">Отношение</span><span class="sxs-lookup"><span data-stu-id="97987-136">Relationship</span></span> | <span data-ttu-id="97987-137">Тип</span><span class="sxs-lookup"><span data-stu-id="97987-137">Type</span></span>   |<span data-ttu-id="97987-138">Описание</span><span class="sxs-lookup"><span data-stu-id="97987-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97987-139">fields</span><span class="sxs-lookup"><span data-stu-id="97987-139">fields</span></span>|[<span data-ttu-id="97987-140">Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="97987-140">workbookSortField</span></span>](workbooksortfield.md)|<span data-ttu-id="97987-141">Указывает текущие условия, которые использовались при последней сортировке таблицы.</span><span class="sxs-lookup"><span data-stu-id="97987-141">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="97987-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97987-142">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97987-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97987-143">JSON representation</span></span>

<span data-ttu-id="97987-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97987-144">Here is a JSON representation of the resource.</span></span>

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
