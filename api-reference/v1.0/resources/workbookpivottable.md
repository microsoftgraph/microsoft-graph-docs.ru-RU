---
title: Тип ресурсов pivotTable
description: Представляет сводную таблицу Excel.
ms.openlocfilehash: b4ddd0c1bb9e4ee13aaf3d1b4472c4e750e3a755
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025064"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="677d5-103">Тип ресурсов pivotTable</span><span class="sxs-lookup"><span data-stu-id="677d5-103">pivotTable resource type</span></span>

<span data-ttu-id="677d5-104">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="677d5-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="677d5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="677d5-105">Methods</span></span>

| <span data-ttu-id="677d5-106">Метод</span><span class="sxs-lookup"><span data-stu-id="677d5-106">Method</span></span>           | <span data-ttu-id="677d5-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="677d5-107">Return Type</span></span>    |<span data-ttu-id="677d5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="677d5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="677d5-109">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="677d5-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="677d5-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="677d5-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="677d5-111">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="677d5-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="677d5-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="677d5-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="677d5-113">Нет</span><span class="sxs-lookup"><span data-stu-id="677d5-113">None</span></span>|<span data-ttu-id="677d5-114">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="677d5-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="677d5-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="677d5-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="677d5-116">Нет</span><span class="sxs-lookup"><span data-stu-id="677d5-116">None</span></span>|<span data-ttu-id="677d5-p101">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="677d5-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="677d5-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="677d5-119">Properties</span></span>
| <span data-ttu-id="677d5-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="677d5-120">Property</span></span>     | <span data-ttu-id="677d5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="677d5-121">Type</span></span>   |<span data-ttu-id="677d5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="677d5-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="677d5-123">id</span><span class="sxs-lookup"><span data-stu-id="677d5-123">id</span></span>|<span data-ttu-id="677d5-124">String</span><span class="sxs-lookup"><span data-stu-id="677d5-124">String</span></span>| <span data-ttu-id="677d5-p102">Идентификатор сводной таблицы.   Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="677d5-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="677d5-127">name</span><span class="sxs-lookup"><span data-stu-id="677d5-127">name</span></span>|<span data-ttu-id="677d5-128">String</span><span class="sxs-lookup"><span data-stu-id="677d5-128">String</span></span>|<span data-ttu-id="677d5-129">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="677d5-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="677d5-130">Связи</span><span class="sxs-lookup"><span data-stu-id="677d5-130">Relationships</span></span>
| <span data-ttu-id="677d5-131">Связь</span><span class="sxs-lookup"><span data-stu-id="677d5-131">Relationship</span></span> | <span data-ttu-id="677d5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="677d5-132">Type</span></span>   |<span data-ttu-id="677d5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="677d5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="677d5-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="677d5-134">worksheet</span></span>|[<span data-ttu-id="677d5-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="677d5-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="677d5-p103">Лист, содержащий текущую сводную таблицу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="677d5-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="677d5-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="677d5-138">JSON representation</span></span>
<span data-ttu-id="677d5-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="677d5-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
