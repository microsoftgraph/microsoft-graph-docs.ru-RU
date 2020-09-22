---
title: Тип ресурса Воркбуктаблесорт
description: Управляет операциями сортировки для объектов Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 77f4fb1dcaed54c2b4cd992b7d6105e194812149
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023746"
---
# <a name="workbooktablesort-resource-type"></a><span data-ttu-id="ac3c1-103">Тип ресурса Воркбуктаблесорт</span><span class="sxs-lookup"><span data-stu-id="ac3c1-103">workbookTableSort resource type</span></span>

<span data-ttu-id="ac3c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac3c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac3c1-105">Управляет операциями сортировки для объектов Table.</span><span class="sxs-lookup"><span data-stu-id="ac3c1-105">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="ac3c1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ac3c1-106">Methods</span></span>

| <span data-ttu-id="ac3c1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ac3c1-107">Method</span></span>           | <span data-ttu-id="ac3c1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ac3c1-108">Return Type</span></span>    |<span data-ttu-id="ac3c1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ac3c1-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac3c1-110">Получение объекта TableSort</span><span class="sxs-lookup"><span data-stu-id="ac3c1-110">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="ac3c1-111">воркбуктаблесорт</span><span class="sxs-lookup"><span data-stu-id="ac3c1-111">workbookTableSort</span></span>](workbooktablesort.md) |<span data-ttu-id="ac3c1-112">Чтение свойств и связей объекта tableSort.</span><span class="sxs-lookup"><span data-stu-id="ac3c1-112">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="ac3c1-113">Apply</span><span class="sxs-lookup"><span data-stu-id="ac3c1-113">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="ac3c1-114">Нет</span><span class="sxs-lookup"><span data-stu-id="ac3c1-114">None</span></span>|<span data-ttu-id="ac3c1-115">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="ac3c1-115">Perform a sort operation.</span></span>|
|[<span data-ttu-id="ac3c1-116">Clear</span><span class="sxs-lookup"><span data-stu-id="ac3c1-116">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="ac3c1-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ac3c1-117">None</span></span>|<span data-ttu-id="ac3c1-p101">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="ac3c1-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="ac3c1-120">Reapply</span><span class="sxs-lookup"><span data-stu-id="ac3c1-120">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="ac3c1-121">Нет</span><span class="sxs-lookup"><span data-stu-id="ac3c1-121">None</span></span>|<span data-ttu-id="ac3c1-122">Повторно применяет текущие параметры сортировки к таблице.</span><span class="sxs-lookup"><span data-stu-id="ac3c1-122">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac3c1-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac3c1-123">Properties</span></span>
| <span data-ttu-id="ac3c1-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac3c1-124">Property</span></span>     | <span data-ttu-id="ac3c1-125">Тип</span><span class="sxs-lookup"><span data-stu-id="ac3c1-125">Type</span></span>   |<span data-ttu-id="ac3c1-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ac3c1-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac3c1-127">matchCase</span><span class="sxs-lookup"><span data-stu-id="ac3c1-127">matchCase</span></span>|<span data-ttu-id="ac3c1-128">boolean</span><span class="sxs-lookup"><span data-stu-id="ac3c1-128">boolean</span></span>|<span data-ttu-id="ac3c1-p102">Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac3c1-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="ac3c1-131">method</span><span class="sxs-lookup"><span data-stu-id="ac3c1-131">method</span></span>|<span data-ttu-id="ac3c1-132">string</span><span class="sxs-lookup"><span data-stu-id="ac3c1-132">string</span></span>|<span data-ttu-id="ac3c1-p103">Указывает метод сортировки китайских символов, который использовался при последней сортировке таблицы. Возможные значения: `PinYin`, `StrokeCount`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac3c1-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac3c1-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="ac3c1-136">Relationships</span></span>
| <span data-ttu-id="ac3c1-137">Связь</span><span class="sxs-lookup"><span data-stu-id="ac3c1-137">Relationship</span></span> | <span data-ttu-id="ac3c1-138">Тип</span><span class="sxs-lookup"><span data-stu-id="ac3c1-138">Type</span></span>   |<span data-ttu-id="ac3c1-139">Описание</span><span class="sxs-lookup"><span data-stu-id="ac3c1-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac3c1-140">fields</span><span class="sxs-lookup"><span data-stu-id="ac3c1-140">fields</span></span>|[<span data-ttu-id="ac3c1-141">воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="ac3c1-141">workbookSortField</span></span>](workbooksortfield.md)|<span data-ttu-id="ac3c1-142">Указывает текущие условия, которые использовались при последней сортировке таблицы.</span><span class="sxs-lookup"><span data-stu-id="ac3c1-142">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="ac3c1-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac3c1-143">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac3c1-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac3c1-144">JSON representation</span></span>

<span data-ttu-id="ac3c1-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac3c1-145">Here is a JSON representation of the resource.</span></span>

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


