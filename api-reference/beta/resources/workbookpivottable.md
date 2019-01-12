---
title: Тип ресурсов pivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 91035b607d8c44f2d1515e9c004abd4c2235c0ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950860"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="b1c3f-103">Тип ресурсов pivotTable</span><span class="sxs-lookup"><span data-stu-id="b1c3f-103">pivotTable resource type</span></span>

> <span data-ttu-id="b1c3f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b1c3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1c3f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c3f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1c3f-106">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="b1c3f-106">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="b1c3f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b1c3f-107">Methods</span></span>

| <span data-ttu-id="b1c3f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b1c3f-108">Method</span></span>           | <span data-ttu-id="b1c3f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b1c3f-109">Return Type</span></span>    |<span data-ttu-id="b1c3f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b1c3f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1c3f-111">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="b1c3f-111">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="b1c3f-112">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="b1c3f-112">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="b1c3f-113">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="b1c3f-113">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="b1c3f-114">Refresh</span><span class="sxs-lookup"><span data-stu-id="b1c3f-114">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="b1c3f-115">Нет</span><span class="sxs-lookup"><span data-stu-id="b1c3f-115">None</span></span>|<span data-ttu-id="b1c3f-116">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="b1c3f-116">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="b1c3f-117">Refreshall</span><span class="sxs-lookup"><span data-stu-id="b1c3f-117">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="b1c3f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b1c3f-118">None</span></span>|<span data-ttu-id="b1c3f-p102">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="b1c3f-p102">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1c3f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1c3f-121">Properties</span></span>
| <span data-ttu-id="b1c3f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1c3f-122">Property</span></span>     | <span data-ttu-id="b1c3f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b1c3f-123">Type</span></span>   |<span data-ttu-id="b1c3f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b1c3f-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1c3f-125">id</span><span class="sxs-lookup"><span data-stu-id="b1c3f-125">id</span></span>|<span data-ttu-id="b1c3f-126">String</span><span class="sxs-lookup"><span data-stu-id="b1c3f-126">String</span></span>| <span data-ttu-id="b1c3f-p103">Идентификатор сводной таблицы.   Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1c3f-p103">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="b1c3f-129">name</span><span class="sxs-lookup"><span data-stu-id="b1c3f-129">name</span></span>|<span data-ttu-id="b1c3f-130">String</span><span class="sxs-lookup"><span data-stu-id="b1c3f-130">String</span></span>|<span data-ttu-id="b1c3f-131">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="b1c3f-131">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="b1c3f-132">Связи</span><span class="sxs-lookup"><span data-stu-id="b1c3f-132">Relationships</span></span>
| <span data-ttu-id="b1c3f-133">Связь</span><span class="sxs-lookup"><span data-stu-id="b1c3f-133">Relationship</span></span> | <span data-ttu-id="b1c3f-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b1c3f-134">Type</span></span>   |<span data-ttu-id="b1c3f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b1c3f-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1c3f-136">worksheet</span><span class="sxs-lookup"><span data-stu-id="b1c3f-136">worksheet</span></span>|[<span data-ttu-id="b1c3f-137">worksheet</span><span class="sxs-lookup"><span data-stu-id="b1c3f-137">worksheet</span></span>](worksheet.md)| <span data-ttu-id="b1c3f-p104">Лист, содержащий текущую сводную таблицу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1c3f-p104">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="b1c3f-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1c3f-140">JSON representation</span></span>
<span data-ttu-id="b1c3f-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1c3f-141">Here is a JSON representation of the resource.</span></span>

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
