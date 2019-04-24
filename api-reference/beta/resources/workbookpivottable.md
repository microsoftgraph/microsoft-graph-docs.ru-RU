---
title: Тип ресурсов pivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fc43bf160e93e354ff58b2f960e8ec38d252287f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453879"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="76e42-103">Тип ресурсов pivotTable</span><span class="sxs-lookup"><span data-stu-id="76e42-103">pivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76e42-104">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="76e42-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="76e42-105">Методы</span><span class="sxs-lookup"><span data-stu-id="76e42-105">Methods</span></span>

| <span data-ttu-id="76e42-106">Метод</span><span class="sxs-lookup"><span data-stu-id="76e42-106">Method</span></span>           | <span data-ttu-id="76e42-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="76e42-107">Return Type</span></span>    |<span data-ttu-id="76e42-108">Описание</span><span class="sxs-lookup"><span data-stu-id="76e42-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="76e42-109">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="76e42-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="76e42-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="76e42-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="76e42-111">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="76e42-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="76e42-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="76e42-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="76e42-113">Нет</span><span class="sxs-lookup"><span data-stu-id="76e42-113">None</span></span>|<span data-ttu-id="76e42-114">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="76e42-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="76e42-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="76e42-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="76e42-116">Нет</span><span class="sxs-lookup"><span data-stu-id="76e42-116">None</span></span>|<span data-ttu-id="76e42-p101">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="76e42-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="76e42-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="76e42-119">Properties</span></span>
| <span data-ttu-id="76e42-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="76e42-120">Property</span></span>     | <span data-ttu-id="76e42-121">Тип</span><span class="sxs-lookup"><span data-stu-id="76e42-121">Type</span></span>   |<span data-ttu-id="76e42-122">Описание</span><span class="sxs-lookup"><span data-stu-id="76e42-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76e42-123">id</span><span class="sxs-lookup"><span data-stu-id="76e42-123">id</span></span>|<span data-ttu-id="76e42-124">Строка</span><span class="sxs-lookup"><span data-stu-id="76e42-124">String</span></span>| <span data-ttu-id="76e42-125">Идентификатор сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="76e42-125">Id of the PivotTable.</span></span>   <span data-ttu-id="76e42-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76e42-126">Read-only.</span></span>|
|<span data-ttu-id="76e42-127">name</span><span class="sxs-lookup"><span data-stu-id="76e42-127">name</span></span>|<span data-ttu-id="76e42-128">String</span><span class="sxs-lookup"><span data-stu-id="76e42-128">String</span></span>|<span data-ttu-id="76e42-129">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="76e42-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="76e42-130">Связи</span><span class="sxs-lookup"><span data-stu-id="76e42-130">Relationships</span></span>
| <span data-ttu-id="76e42-131">Отношение</span><span class="sxs-lookup"><span data-stu-id="76e42-131">Relationship</span></span> | <span data-ttu-id="76e42-132">Тип</span><span class="sxs-lookup"><span data-stu-id="76e42-132">Type</span></span>   |<span data-ttu-id="76e42-133">Описание</span><span class="sxs-lookup"><span data-stu-id="76e42-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76e42-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="76e42-134">worksheet</span></span>|[<span data-ttu-id="76e42-135">worksheet</span><span class="sxs-lookup"><span data-stu-id="76e42-135">worksheet</span></span>](worksheet.md)| <span data-ttu-id="76e42-p103">Лист, содержащий текущую сводную таблицу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76e42-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="76e42-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76e42-138">JSON representation</span></span>
<span data-ttu-id="76e42-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76e42-139">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookpivottable.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
