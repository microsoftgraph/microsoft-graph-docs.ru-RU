---
title: Тип ресурсов pivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 774c407022d700bc5856dc780eff3a6dafa6bc4e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577461"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="877a5-103">Тип ресурсов pivotTable</span><span class="sxs-lookup"><span data-stu-id="877a5-103">pivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="877a5-104">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="877a5-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="877a5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="877a5-105">Methods</span></span>

| <span data-ttu-id="877a5-106">Метод</span><span class="sxs-lookup"><span data-stu-id="877a5-106">Method</span></span>           | <span data-ttu-id="877a5-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="877a5-107">Return Type</span></span>    |<span data-ttu-id="877a5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="877a5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="877a5-109">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="877a5-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="877a5-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="877a5-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="877a5-111">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="877a5-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="877a5-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="877a5-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="877a5-113">Нет</span><span class="sxs-lookup"><span data-stu-id="877a5-113">None</span></span>|<span data-ttu-id="877a5-114">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="877a5-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="877a5-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="877a5-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="877a5-116">Нет</span><span class="sxs-lookup"><span data-stu-id="877a5-116">None</span></span>|<span data-ttu-id="877a5-p101">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="877a5-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="877a5-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="877a5-119">Properties</span></span>
| <span data-ttu-id="877a5-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="877a5-120">Property</span></span>     | <span data-ttu-id="877a5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="877a5-121">Type</span></span>   |<span data-ttu-id="877a5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="877a5-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="877a5-123">id</span><span class="sxs-lookup"><span data-stu-id="877a5-123">id</span></span>|<span data-ttu-id="877a5-124">String</span><span class="sxs-lookup"><span data-stu-id="877a5-124">String</span></span>| <span data-ttu-id="877a5-p102">Идентификатор сводной таблицы.   Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="877a5-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="877a5-127">name</span><span class="sxs-lookup"><span data-stu-id="877a5-127">name</span></span>|<span data-ttu-id="877a5-128">String</span><span class="sxs-lookup"><span data-stu-id="877a5-128">String</span></span>|<span data-ttu-id="877a5-129">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="877a5-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="877a5-130">Связи</span><span class="sxs-lookup"><span data-stu-id="877a5-130">Relationships</span></span>
| <span data-ttu-id="877a5-131">Связь</span><span class="sxs-lookup"><span data-stu-id="877a5-131">Relationship</span></span> | <span data-ttu-id="877a5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="877a5-132">Type</span></span>   |<span data-ttu-id="877a5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="877a5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="877a5-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="877a5-134">worksheet</span></span>|[<span data-ttu-id="877a5-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="877a5-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="877a5-p103">Лист, содержащий текущую сводную таблицу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="877a5-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="877a5-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="877a5-138">JSON representation</span></span>
<span data-ttu-id="877a5-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="877a5-139">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookpivottable.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
