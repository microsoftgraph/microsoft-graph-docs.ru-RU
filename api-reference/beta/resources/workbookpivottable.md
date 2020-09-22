---
title: Тип ресурса workbookPivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 98db064c101d60c9db25eb0a9515da74e25e96ad
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023823"
---
# <a name="workbookpivottable-resource-type"></a><span data-ttu-id="36879-103">Тип ресурса workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="36879-103">workbookPivotTable resource type</span></span>

<span data-ttu-id="36879-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36879-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36879-105">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="36879-105">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="36879-106">Методы</span><span class="sxs-lookup"><span data-stu-id="36879-106">Methods</span></span>

| <span data-ttu-id="36879-107">Метод</span><span class="sxs-lookup"><span data-stu-id="36879-107">Method</span></span>           | <span data-ttu-id="36879-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="36879-108">Return Type</span></span>    |<span data-ttu-id="36879-109">Описание</span><span class="sxs-lookup"><span data-stu-id="36879-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="36879-110">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="36879-110">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="36879-111">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="36879-111">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="36879-112">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="36879-112">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="36879-113">Refresh</span><span class="sxs-lookup"><span data-stu-id="36879-113">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="36879-114">Нет</span><span class="sxs-lookup"><span data-stu-id="36879-114">None</span></span>|<span data-ttu-id="36879-115">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="36879-115">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="36879-116">Refreshall</span><span class="sxs-lookup"><span data-stu-id="36879-116">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="36879-117">Нет</span><span class="sxs-lookup"><span data-stu-id="36879-117">None</span></span>|<span data-ttu-id="36879-p101">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="36879-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="36879-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="36879-120">Properties</span></span>
| <span data-ttu-id="36879-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="36879-121">Property</span></span>     | <span data-ttu-id="36879-122">Тип</span><span class="sxs-lookup"><span data-stu-id="36879-122">Type</span></span>   |<span data-ttu-id="36879-123">Описание</span><span class="sxs-lookup"><span data-stu-id="36879-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36879-124">id</span><span class="sxs-lookup"><span data-stu-id="36879-124">id</span></span>|<span data-ttu-id="36879-125">String</span><span class="sxs-lookup"><span data-stu-id="36879-125">String</span></span>| <span data-ttu-id="36879-126">Идентификатор сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="36879-126">Id of the PivotTable.</span></span>   <span data-ttu-id="36879-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="36879-127">Read-only.</span></span>|
|<span data-ttu-id="36879-128">name</span><span class="sxs-lookup"><span data-stu-id="36879-128">name</span></span>|<span data-ttu-id="36879-129">String</span><span class="sxs-lookup"><span data-stu-id="36879-129">String</span></span>|<span data-ttu-id="36879-130">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="36879-130">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="36879-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="36879-131">Relationships</span></span>
| <span data-ttu-id="36879-132">Связь</span><span class="sxs-lookup"><span data-stu-id="36879-132">Relationship</span></span> | <span data-ttu-id="36879-133">Тип</span><span class="sxs-lookup"><span data-stu-id="36879-133">Type</span></span>   |<span data-ttu-id="36879-134">Описание</span><span class="sxs-lookup"><span data-stu-id="36879-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36879-135">worksheet</span><span class="sxs-lookup"><span data-stu-id="36879-135">worksheet</span></span>|[<span data-ttu-id="36879-136">воркбукворкшит</span><span class="sxs-lookup"><span data-stu-id="36879-136">workbookWorksheet</span></span>](workbookworksheet.md)| <span data-ttu-id="36879-137">Лист, содержащий текущую сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="36879-137">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="36879-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="36879-138">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="36879-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36879-139">JSON representation</span></span>
<span data-ttu-id="36879-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36879-140">Here is a JSON representation of the resource.</span></span>

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


