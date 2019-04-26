---
title: Тип ресурса workbookPivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 99ad62474ef0c8e56ec5a699edac742ee28ae446
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345791"
---
# <a name="workbookpivottable-resource-type"></a><span data-ttu-id="a0ae6-103">Тип ресурса workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="a0ae6-103">workbookPivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0ae6-104">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="a0ae6-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="a0ae6-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a0ae6-105">Methods</span></span>

| <span data-ttu-id="a0ae6-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a0ae6-106">Method</span></span>           | <span data-ttu-id="a0ae6-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a0ae6-107">Return Type</span></span>    |<span data-ttu-id="a0ae6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a0ae6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a0ae6-109">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="a0ae6-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="a0ae6-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="a0ae6-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="a0ae6-111">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="a0ae6-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="a0ae6-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="a0ae6-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="a0ae6-113">Нет</span><span class="sxs-lookup"><span data-stu-id="a0ae6-113">None</span></span>|<span data-ttu-id="a0ae6-114">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="a0ae6-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="a0ae6-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="a0ae6-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="a0ae6-116">Нет</span><span class="sxs-lookup"><span data-stu-id="a0ae6-116">None</span></span>|<span data-ttu-id="a0ae6-p101">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="a0ae6-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="a0ae6-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0ae6-119">Properties</span></span>
| <span data-ttu-id="a0ae6-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0ae6-120">Property</span></span>     | <span data-ttu-id="a0ae6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a0ae6-121">Type</span></span>   |<span data-ttu-id="a0ae6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a0ae6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0ae6-123">id</span><span class="sxs-lookup"><span data-stu-id="a0ae6-123">id</span></span>|<span data-ttu-id="a0ae6-124">Строка</span><span class="sxs-lookup"><span data-stu-id="a0ae6-124">String</span></span>| <span data-ttu-id="a0ae6-125">Идентификатор сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="a0ae6-125">Id of the PivotTable.</span></span>   <span data-ttu-id="a0ae6-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0ae6-126">Read-only.</span></span>|
|<span data-ttu-id="a0ae6-127">name</span><span class="sxs-lookup"><span data-stu-id="a0ae6-127">name</span></span>|<span data-ttu-id="a0ae6-128">String</span><span class="sxs-lookup"><span data-stu-id="a0ae6-128">String</span></span>|<span data-ttu-id="a0ae6-129">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="a0ae6-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="a0ae6-130">Связи</span><span class="sxs-lookup"><span data-stu-id="a0ae6-130">Relationships</span></span>
| <span data-ttu-id="a0ae6-131">Отношение</span><span class="sxs-lookup"><span data-stu-id="a0ae6-131">Relationship</span></span> | <span data-ttu-id="a0ae6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a0ae6-132">Type</span></span>   |<span data-ttu-id="a0ae6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a0ae6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0ae6-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="a0ae6-134">worksheet</span></span>|[<span data-ttu-id="a0ae6-135">Воркбукворкшит</span><span class="sxs-lookup"><span data-stu-id="a0ae6-135">workbookWorksheet</span></span>](workbookworksheet.md)| <span data-ttu-id="a0ae6-136">Лист, содержащий текущую сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="a0ae6-136">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="a0ae6-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0ae6-137">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="a0ae6-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a0ae6-138">JSON representation</span></span>
<span data-ttu-id="a0ae6-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0ae6-139">Here is a JSON representation of the resource.</span></span>

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
