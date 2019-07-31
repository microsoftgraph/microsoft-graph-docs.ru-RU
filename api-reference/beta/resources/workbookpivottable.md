---
title: Тип ресурса workbookPivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d8df88699fde1e4d5562db6299cd12665512c03b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963997"
---
# <a name="workbookpivottable-resource-type"></a><span data-ttu-id="a10f0-103">Тип ресурса workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="a10f0-103">workbookPivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a10f0-104">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="a10f0-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="a10f0-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a10f0-105">Methods</span></span>

| <span data-ttu-id="a10f0-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a10f0-106">Method</span></span>           | <span data-ttu-id="a10f0-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a10f0-107">Return Type</span></span>    |<span data-ttu-id="a10f0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a10f0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a10f0-109">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="a10f0-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="a10f0-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="a10f0-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="a10f0-111">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="a10f0-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="a10f0-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="a10f0-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="a10f0-113">Нет</span><span class="sxs-lookup"><span data-stu-id="a10f0-113">None</span></span>|<span data-ttu-id="a10f0-114">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="a10f0-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="a10f0-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="a10f0-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="a10f0-116">Нет</span><span class="sxs-lookup"><span data-stu-id="a10f0-116">None</span></span>|<span data-ttu-id="a10f0-p101">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="a10f0-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="a10f0-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="a10f0-119">Properties</span></span>
| <span data-ttu-id="a10f0-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="a10f0-120">Property</span></span>     | <span data-ttu-id="a10f0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a10f0-121">Type</span></span>   |<span data-ttu-id="a10f0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a10f0-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a10f0-123">id</span><span class="sxs-lookup"><span data-stu-id="a10f0-123">id</span></span>|<span data-ttu-id="a10f0-124">Строка</span><span class="sxs-lookup"><span data-stu-id="a10f0-124">String</span></span>| <span data-ttu-id="a10f0-125">Идентификатор сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="a10f0-125">Id of the PivotTable.</span></span>   <span data-ttu-id="a10f0-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a10f0-126">Read-only.</span></span>|
|<span data-ttu-id="a10f0-127">name</span><span class="sxs-lookup"><span data-stu-id="a10f0-127">name</span></span>|<span data-ttu-id="a10f0-128">String</span><span class="sxs-lookup"><span data-stu-id="a10f0-128">String</span></span>|<span data-ttu-id="a10f0-129">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="a10f0-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="a10f0-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="a10f0-130">Relationships</span></span>
| <span data-ttu-id="a10f0-131">Отношение</span><span class="sxs-lookup"><span data-stu-id="a10f0-131">Relationship</span></span> | <span data-ttu-id="a10f0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a10f0-132">Type</span></span>   |<span data-ttu-id="a10f0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a10f0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a10f0-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="a10f0-134">worksheet</span></span>|[<span data-ttu-id="a10f0-135">Воркбукворкшит</span><span class="sxs-lookup"><span data-stu-id="a10f0-135">workbookWorksheet</span></span>](workbookworksheet.md)| <span data-ttu-id="a10f0-136">Лист, содержащий текущую сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="a10f0-136">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="a10f0-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a10f0-137">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="a10f0-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a10f0-138">JSON representation</span></span>
<span data-ttu-id="a10f0-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a10f0-139">Here is a JSON representation of the resource.</span></span>

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
