---
title: Тип ресурса TableSort
description: Управляет операциями сортировки для объектов Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3772d0063fc19eb3a3c46953d5c85d8085f0a72a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533567"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="221ba-103">Тип ресурса TableSort</span><span class="sxs-lookup"><span data-stu-id="221ba-103">TableSort resource type</span></span>

<span data-ttu-id="221ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="221ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="221ba-105">Управляет операциями сортировки для объектов Table.</span><span class="sxs-lookup"><span data-stu-id="221ba-105">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="221ba-106">Методы</span><span class="sxs-lookup"><span data-stu-id="221ba-106">Methods</span></span>

| <span data-ttu-id="221ba-107">Метод</span><span class="sxs-lookup"><span data-stu-id="221ba-107">Method</span></span>           | <span data-ttu-id="221ba-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="221ba-108">Return Type</span></span>    |<span data-ttu-id="221ba-109">Описание</span><span class="sxs-lookup"><span data-stu-id="221ba-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="221ba-110">Получение объекта TableSort</span><span class="sxs-lookup"><span data-stu-id="221ba-110">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="221ba-111">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="221ba-111">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="221ba-112">Чтение свойств и связей объекта tableSort.</span><span class="sxs-lookup"><span data-stu-id="221ba-112">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="221ba-113">Apply</span><span class="sxs-lookup"><span data-stu-id="221ba-113">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="221ba-114">Нет</span><span class="sxs-lookup"><span data-stu-id="221ba-114">None</span></span>|<span data-ttu-id="221ba-115">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="221ba-115">Perform a sort operation.</span></span>|
|[<span data-ttu-id="221ba-116">Clear</span><span class="sxs-lookup"><span data-stu-id="221ba-116">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="221ba-117">Нет</span><span class="sxs-lookup"><span data-stu-id="221ba-117">None</span></span>|<span data-ttu-id="221ba-p101">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="221ba-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="221ba-120">Reapply</span><span class="sxs-lookup"><span data-stu-id="221ba-120">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="221ba-121">Нет</span><span class="sxs-lookup"><span data-stu-id="221ba-121">None</span></span>|<span data-ttu-id="221ba-122">Повторно применяет текущие параметры сортировки к таблице.</span><span class="sxs-lookup"><span data-stu-id="221ba-122">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="221ba-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="221ba-123">Properties</span></span>
| <span data-ttu-id="221ba-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="221ba-124">Property</span></span>     | <span data-ttu-id="221ba-125">Тип</span><span class="sxs-lookup"><span data-stu-id="221ba-125">Type</span></span>   |<span data-ttu-id="221ba-126">Описание</span><span class="sxs-lookup"><span data-stu-id="221ba-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="221ba-127">fields</span><span class="sxs-lookup"><span data-stu-id="221ba-127">fields</span></span>|<span data-ttu-id="221ba-128">Коллекция [воркбуксортфиелд](sortfield.md)</span><span class="sxs-lookup"><span data-stu-id="221ba-128">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="221ba-129">Указывает текущие условия, которые использовались при последней сортировке таблицы.</span><span class="sxs-lookup"><span data-stu-id="221ba-129">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="221ba-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="221ba-130">Read-only.</span></span>|
|<span data-ttu-id="221ba-131">matchCase</span><span class="sxs-lookup"><span data-stu-id="221ba-131">matchCase</span></span>|<span data-ttu-id="221ba-132">boolean</span><span class="sxs-lookup"><span data-stu-id="221ba-132">boolean</span></span>|<span data-ttu-id="221ba-p103">Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="221ba-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="221ba-135">method</span><span class="sxs-lookup"><span data-stu-id="221ba-135">method</span></span>|<span data-ttu-id="221ba-136">string</span><span class="sxs-lookup"><span data-stu-id="221ba-136">string</span></span>|<span data-ttu-id="221ba-137">Указывает метод сортировки китайских символов, который использовался при последней сортировке таблицы.</span><span class="sxs-lookup"><span data-stu-id="221ba-137">Represents Chinese character ordering method last used to sort the table.</span></span> <span data-ttu-id="221ba-138">Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="221ba-138">The possible values are: `PinYin`, `StrokeCount`.</span></span> <span data-ttu-id="221ba-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="221ba-139">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="221ba-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="221ba-140">JSON representation</span></span>

<span data-ttu-id="221ba-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="221ba-141">Here is a JSON representation of the resource.</span></span>

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
