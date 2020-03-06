---
title: Тип ресурсов pivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b3ec3c9237e246b2af10a867155bc7b6d360a67f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533379"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="0595d-103">Тип ресурсов pivotTable</span><span class="sxs-lookup"><span data-stu-id="0595d-103">pivotTable resource type</span></span>

<span data-ttu-id="0595d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0595d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0595d-105">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="0595d-105">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="0595d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0595d-106">Methods</span></span>

| <span data-ttu-id="0595d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0595d-107">Method</span></span>           | <span data-ttu-id="0595d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0595d-108">Return Type</span></span>    |<span data-ttu-id="0595d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0595d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0595d-110">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="0595d-110">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="0595d-111">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="0595d-111">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="0595d-112">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="0595d-112">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="0595d-113">Refresh</span><span class="sxs-lookup"><span data-stu-id="0595d-113">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="0595d-114">Нет</span><span class="sxs-lookup"><span data-stu-id="0595d-114">None</span></span>|<span data-ttu-id="0595d-115">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="0595d-115">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="0595d-116">Refreshall</span><span class="sxs-lookup"><span data-stu-id="0595d-116">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="0595d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="0595d-117">None</span></span>|<span data-ttu-id="0595d-p101">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="0595d-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="0595d-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="0595d-120">Properties</span></span>
| <span data-ttu-id="0595d-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="0595d-121">Property</span></span>     | <span data-ttu-id="0595d-122">Тип</span><span class="sxs-lookup"><span data-stu-id="0595d-122">Type</span></span>   |<span data-ttu-id="0595d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0595d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0595d-124">id</span><span class="sxs-lookup"><span data-stu-id="0595d-124">id</span></span>|<span data-ttu-id="0595d-125">Строка</span><span class="sxs-lookup"><span data-stu-id="0595d-125">String</span></span>| <span data-ttu-id="0595d-126">Идентификатор сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="0595d-126">Id of the PivotTable.</span></span>   <span data-ttu-id="0595d-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0595d-127">Read-only.</span></span>|
|<span data-ttu-id="0595d-128">name</span><span class="sxs-lookup"><span data-stu-id="0595d-128">name</span></span>|<span data-ttu-id="0595d-129">String</span><span class="sxs-lookup"><span data-stu-id="0595d-129">String</span></span>|<span data-ttu-id="0595d-130">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="0595d-130">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="0595d-131">Связи</span><span class="sxs-lookup"><span data-stu-id="0595d-131">Relationships</span></span>
| <span data-ttu-id="0595d-132">Связь</span><span class="sxs-lookup"><span data-stu-id="0595d-132">Relationship</span></span> | <span data-ttu-id="0595d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0595d-133">Type</span></span>   |<span data-ttu-id="0595d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0595d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0595d-135">worksheet</span><span class="sxs-lookup"><span data-stu-id="0595d-135">worksheet</span></span>|[<span data-ttu-id="0595d-136">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="0595d-136">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="0595d-137">Лист, содержащий текущую сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="0595d-137">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="0595d-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0595d-138">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="0595d-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0595d-139">JSON representation</span></span>
<span data-ttu-id="0595d-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0595d-140">Here is a JSON representation of the resource.</span></span>

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
