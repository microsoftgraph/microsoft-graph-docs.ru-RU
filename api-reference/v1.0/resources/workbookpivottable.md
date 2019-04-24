---
title: Тип ресурсов pivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5f6360ce1eacc313f1bcc8a9f59b44b216a87b84
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456866"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="c4535-103">Тип ресурсов pivotTable</span><span class="sxs-lookup"><span data-stu-id="c4535-103">pivotTable resource type</span></span>

<span data-ttu-id="c4535-104">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="c4535-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="c4535-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c4535-105">Methods</span></span>

| <span data-ttu-id="c4535-106">Метод</span><span class="sxs-lookup"><span data-stu-id="c4535-106">Method</span></span>           | <span data-ttu-id="c4535-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c4535-107">Return Type</span></span>    |<span data-ttu-id="c4535-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c4535-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4535-109">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="c4535-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="c4535-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="c4535-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="c4535-111">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="c4535-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="c4535-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="c4535-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="c4535-113">Нет</span><span class="sxs-lookup"><span data-stu-id="c4535-113">None</span></span>|<span data-ttu-id="c4535-114">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="c4535-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="c4535-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="c4535-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="c4535-116">Нет</span><span class="sxs-lookup"><span data-stu-id="c4535-116">None</span></span>|<span data-ttu-id="c4535-p101">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="c4535-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="c4535-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4535-119">Properties</span></span>
| <span data-ttu-id="c4535-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4535-120">Property</span></span>     | <span data-ttu-id="c4535-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c4535-121">Type</span></span>   |<span data-ttu-id="c4535-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c4535-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4535-123">id</span><span class="sxs-lookup"><span data-stu-id="c4535-123">id</span></span>|<span data-ttu-id="c4535-124">Строка</span><span class="sxs-lookup"><span data-stu-id="c4535-124">String</span></span>| <span data-ttu-id="c4535-125">Идентификатор сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="c4535-125">Id of the PivotTable.</span></span>   <span data-ttu-id="c4535-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4535-126">Read-only.</span></span>|
|<span data-ttu-id="c4535-127">name</span><span class="sxs-lookup"><span data-stu-id="c4535-127">name</span></span>|<span data-ttu-id="c4535-128">String</span><span class="sxs-lookup"><span data-stu-id="c4535-128">String</span></span>|<span data-ttu-id="c4535-129">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="c4535-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="c4535-130">Связи</span><span class="sxs-lookup"><span data-stu-id="c4535-130">Relationships</span></span>
| <span data-ttu-id="c4535-131">Отношение</span><span class="sxs-lookup"><span data-stu-id="c4535-131">Relationship</span></span> | <span data-ttu-id="c4535-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c4535-132">Type</span></span>   |<span data-ttu-id="c4535-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c4535-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4535-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="c4535-134">worksheet</span></span>|[<span data-ttu-id="c4535-135">Воркбукворкшит</span><span class="sxs-lookup"><span data-stu-id="c4535-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="c4535-136">Лист, содержащий текущую сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="c4535-136">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="c4535-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4535-137">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="c4535-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4535-138">JSON representation</span></span>
<span data-ttu-id="c4535-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4535-139">Here is a JSON representation of the resource.</span></span>

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
