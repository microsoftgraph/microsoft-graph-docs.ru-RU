---
title: Тип ресурсов pivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fb67920598d883a126c18cdf8acdfb1b38d9014a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015136"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="f2a37-103">Тип ресурсов pivotTable</span><span class="sxs-lookup"><span data-stu-id="f2a37-103">pivotTable resource type</span></span>

<span data-ttu-id="f2a37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2a37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2a37-105">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="f2a37-105">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="f2a37-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f2a37-106">Methods</span></span>

| <span data-ttu-id="f2a37-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f2a37-107">Method</span></span>           | <span data-ttu-id="f2a37-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f2a37-108">Return Type</span></span>    |<span data-ttu-id="f2a37-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f2a37-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2a37-110">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="f2a37-110">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="f2a37-111">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="f2a37-111">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="f2a37-112">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="f2a37-112">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="f2a37-113">Refresh</span><span class="sxs-lookup"><span data-stu-id="f2a37-113">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="f2a37-114">Нет</span><span class="sxs-lookup"><span data-stu-id="f2a37-114">None</span></span>|<span data-ttu-id="f2a37-115">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="f2a37-115">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="f2a37-116">Refreshall</span><span class="sxs-lookup"><span data-stu-id="f2a37-116">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="f2a37-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f2a37-117">None</span></span>|<span data-ttu-id="f2a37-p101">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="f2a37-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2a37-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2a37-120">Properties</span></span>
| <span data-ttu-id="f2a37-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2a37-121">Property</span></span>     | <span data-ttu-id="f2a37-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f2a37-122">Type</span></span>   |<span data-ttu-id="f2a37-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f2a37-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2a37-124">id</span><span class="sxs-lookup"><span data-stu-id="f2a37-124">id</span></span>|<span data-ttu-id="f2a37-125">String</span><span class="sxs-lookup"><span data-stu-id="f2a37-125">String</span></span>| <span data-ttu-id="f2a37-126">Идентификатор сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="f2a37-126">Id of the PivotTable.</span></span>   <span data-ttu-id="f2a37-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2a37-127">Read-only.</span></span>|
|<span data-ttu-id="f2a37-128">name</span><span class="sxs-lookup"><span data-stu-id="f2a37-128">name</span></span>|<span data-ttu-id="f2a37-129">String</span><span class="sxs-lookup"><span data-stu-id="f2a37-129">String</span></span>|<span data-ttu-id="f2a37-130">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="f2a37-130">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="f2a37-131">Связи</span><span class="sxs-lookup"><span data-stu-id="f2a37-131">Relationships</span></span>
| <span data-ttu-id="f2a37-132">Связь</span><span class="sxs-lookup"><span data-stu-id="f2a37-132">Relationship</span></span> | <span data-ttu-id="f2a37-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f2a37-133">Type</span></span>   |<span data-ttu-id="f2a37-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f2a37-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2a37-135">worksheet</span><span class="sxs-lookup"><span data-stu-id="f2a37-135">worksheet</span></span>|[<span data-ttu-id="f2a37-136">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="f2a37-136">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="f2a37-137">Лист, содержащий текущую сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="f2a37-137">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="f2a37-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2a37-138">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="f2a37-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2a37-139">JSON representation</span></span>
<span data-ttu-id="f2a37-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2a37-140">Here is a JSON representation of the resource.</span></span>

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

