---
title: Тип ресурсов pivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5f6360ce1eacc313f1bcc8a9f59b44b216a87b84
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958742"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="604ad-103">Тип ресурсов pivotTable</span><span class="sxs-lookup"><span data-stu-id="604ad-103">pivotTable resource type</span></span>

<span data-ttu-id="604ad-104">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="604ad-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="604ad-105">Методы</span><span class="sxs-lookup"><span data-stu-id="604ad-105">Methods</span></span>

| <span data-ttu-id="604ad-106">Метод</span><span class="sxs-lookup"><span data-stu-id="604ad-106">Method</span></span>           | <span data-ttu-id="604ad-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="604ad-107">Return Type</span></span>    |<span data-ttu-id="604ad-108">Описание</span><span class="sxs-lookup"><span data-stu-id="604ad-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="604ad-109">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="604ad-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="604ad-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="604ad-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="604ad-111">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="604ad-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="604ad-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="604ad-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="604ad-113">Нет</span><span class="sxs-lookup"><span data-stu-id="604ad-113">None</span></span>|<span data-ttu-id="604ad-114">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="604ad-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="604ad-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="604ad-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="604ad-116">Нет</span><span class="sxs-lookup"><span data-stu-id="604ad-116">None</span></span>|<span data-ttu-id="604ad-p101">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="604ad-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="604ad-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="604ad-119">Properties</span></span>
| <span data-ttu-id="604ad-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="604ad-120">Property</span></span>     | <span data-ttu-id="604ad-121">Тип</span><span class="sxs-lookup"><span data-stu-id="604ad-121">Type</span></span>   |<span data-ttu-id="604ad-122">Описание</span><span class="sxs-lookup"><span data-stu-id="604ad-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="604ad-123">id</span><span class="sxs-lookup"><span data-stu-id="604ad-123">id</span></span>|<span data-ttu-id="604ad-124">String</span><span class="sxs-lookup"><span data-stu-id="604ad-124">String</span></span>| <span data-ttu-id="604ad-p102">Идентификатор сводной таблицы.   Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="604ad-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="604ad-127">name</span><span class="sxs-lookup"><span data-stu-id="604ad-127">name</span></span>|<span data-ttu-id="604ad-128">String</span><span class="sxs-lookup"><span data-stu-id="604ad-128">String</span></span>|<span data-ttu-id="604ad-129">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="604ad-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="604ad-130">Связи</span><span class="sxs-lookup"><span data-stu-id="604ad-130">Relationships</span></span>
| <span data-ttu-id="604ad-131">Связь</span><span class="sxs-lookup"><span data-stu-id="604ad-131">Relationship</span></span> | <span data-ttu-id="604ad-132">Тип</span><span class="sxs-lookup"><span data-stu-id="604ad-132">Type</span></span>   |<span data-ttu-id="604ad-133">Описание</span><span class="sxs-lookup"><span data-stu-id="604ad-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="604ad-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="604ad-134">worksheet</span></span>|[<span data-ttu-id="604ad-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="604ad-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="604ad-p103">Лист, содержащий текущую сводную таблицу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="604ad-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="604ad-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="604ad-138">JSON representation</span></span>
<span data-ttu-id="604ad-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="604ad-139">Here is a JSON representation of the resource.</span></span>

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
