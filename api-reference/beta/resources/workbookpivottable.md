---
title: Тип ресурсов pivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: aead84b21117b896f620a0722cf42c2e6c5d1293
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831544"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="7660d-103">Тип ресурсов pivotTable</span><span class="sxs-lookup"><span data-stu-id="7660d-103">pivotTable resource type</span></span>

> <span data-ttu-id="7660d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7660d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7660d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7660d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7660d-106">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="7660d-106">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="7660d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7660d-107">Methods</span></span>

| <span data-ttu-id="7660d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7660d-108">Method</span></span>           | <span data-ttu-id="7660d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7660d-109">Return Type</span></span>    |<span data-ttu-id="7660d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7660d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7660d-111">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="7660d-111">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="7660d-112">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="7660d-112">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="7660d-113">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="7660d-113">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="7660d-114">Refresh</span><span class="sxs-lookup"><span data-stu-id="7660d-114">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="7660d-115">Нет</span><span class="sxs-lookup"><span data-stu-id="7660d-115">None</span></span>|<span data-ttu-id="7660d-116">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="7660d-116">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="7660d-117">Refreshall</span><span class="sxs-lookup"><span data-stu-id="7660d-117">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="7660d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="7660d-118">None</span></span>|<span data-ttu-id="7660d-p102">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="7660d-p102">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="7660d-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="7660d-121">Properties</span></span>
| <span data-ttu-id="7660d-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="7660d-122">Property</span></span>     | <span data-ttu-id="7660d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7660d-123">Type</span></span>   |<span data-ttu-id="7660d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7660d-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7660d-125">id</span><span class="sxs-lookup"><span data-stu-id="7660d-125">id</span></span>|<span data-ttu-id="7660d-126">String</span><span class="sxs-lookup"><span data-stu-id="7660d-126">String</span></span>| <span data-ttu-id="7660d-p103">Идентификатор сводной таблицы.   Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7660d-p103">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="7660d-129">name</span><span class="sxs-lookup"><span data-stu-id="7660d-129">name</span></span>|<span data-ttu-id="7660d-130">String</span><span class="sxs-lookup"><span data-stu-id="7660d-130">String</span></span>|<span data-ttu-id="7660d-131">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="7660d-131">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="7660d-132">Связи</span><span class="sxs-lookup"><span data-stu-id="7660d-132">Relationships</span></span>
| <span data-ttu-id="7660d-133">Связь</span><span class="sxs-lookup"><span data-stu-id="7660d-133">Relationship</span></span> | <span data-ttu-id="7660d-134">Тип</span><span class="sxs-lookup"><span data-stu-id="7660d-134">Type</span></span>   |<span data-ttu-id="7660d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="7660d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7660d-136">worksheet</span><span class="sxs-lookup"><span data-stu-id="7660d-136">worksheet</span></span>|[<span data-ttu-id="7660d-137">worksheet</span><span class="sxs-lookup"><span data-stu-id="7660d-137">worksheet</span></span>](worksheet.md)| <span data-ttu-id="7660d-p104">Лист, содержащий текущую сводную таблицу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7660d-p104">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="7660d-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7660d-140">JSON representation</span></span>
<span data-ttu-id="7660d-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7660d-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
