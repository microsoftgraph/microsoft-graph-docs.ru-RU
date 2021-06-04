---
title: тип ресурса printUsageSummaryByPrinter
description: Описывает активность печати для принтера в течение указанного периода времени (useDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4d33ab99780f980dcc24e267ba1ac6603f602aa2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753613"
---
# <a name="printusagesummarybyprinter-resource-type"></a><span data-ttu-id="24b3f-103">тип ресурса printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="24b3f-103">printUsageSummaryByPrinter resource type</span></span>

<span data-ttu-id="24b3f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24b3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24b3f-105">Описывает активность печати для принтера в течение указанного периода времени (useDate).</span><span class="sxs-lookup"><span data-stu-id="24b3f-105">Describes print activity for a printer during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="24b3f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="24b3f-106">Methods</span></span>

| <span data-ttu-id="24b3f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="24b3f-107">Method</span></span>       | <span data-ttu-id="24b3f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="24b3f-108">Return Type</span></span> | <span data-ttu-id="24b3f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="24b3f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="24b3f-110">Список (ежедневно)</span><span class="sxs-lookup"><span data-stu-id="24b3f-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagesummariesbyprinter.md) | [<span data-ttu-id="24b3f-111">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="24b3f-111">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="24b3f-112">Получите список сводок об использовании ежедневной печати, сгруппив их по принтеру.</span><span class="sxs-lookup"><span data-stu-id="24b3f-112">Get a list of daily print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="24b3f-113">Список (ежемесячно)</span><span class="sxs-lookup"><span data-stu-id="24b3f-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagesummariesbyprinter.md) | [<span data-ttu-id="24b3f-114">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="24b3f-114">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="24b3f-115">Получите список ежемесячных сводок использования печати, сгруппив их по принтеру.</span><span class="sxs-lookup"><span data-stu-id="24b3f-115">Get a list of monthly print usage summaries, grouped by printer.</span></span> |
| <span data-ttu-id="24b3f-116">[получение](../api/printusagesummarybyprinter-get.md);</span><span class="sxs-lookup"><span data-stu-id="24b3f-116">[Get](../api/printusagesummarybyprinter-get.md)</span></span> | [<span data-ttu-id="24b3f-117">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="24b3f-117">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="24b3f-118">Ознакомьтесь с свойствами и отношениями объекта **printUsageSummaryByPrinter.**</span><span class="sxs-lookup"><span data-stu-id="24b3f-118">Read the properties and relationships of a **printUsageSummaryByPrinter** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="24b3f-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="24b3f-119">Properties</span></span>
| <span data-ttu-id="24b3f-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="24b3f-120">Property</span></span>     | <span data-ttu-id="24b3f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="24b3f-121">Type</span></span>        | <span data-ttu-id="24b3f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="24b3f-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="24b3f-123">id</span><span class="sxs-lookup"><span data-stu-id="24b3f-123">id</span></span>|<span data-ttu-id="24b3f-124">String</span><span class="sxs-lookup"><span data-stu-id="24b3f-124">String</span></span>|<span data-ttu-id="24b3f-125">ID этого сводки использования.</span><span class="sxs-lookup"><span data-stu-id="24b3f-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="24b3f-126">printerID</span><span class="sxs-lookup"><span data-stu-id="24b3f-126">printerID</span></span>|<span data-ttu-id="24b3f-127">String</span><span class="sxs-lookup"><span data-stu-id="24b3f-127">String</span></span>|<span data-ttu-id="24b3f-128">ID принтера, представленный этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="24b3f-128">The ID of the printer represented by these statistics.</span></span>|
|<span data-ttu-id="24b3f-129">useDate</span><span class="sxs-lookup"><span data-stu-id="24b3f-129">usageDate</span></span>|<span data-ttu-id="24b3f-130">Дата</span><span class="sxs-lookup"><span data-stu-id="24b3f-130">Date</span></span>|<span data-ttu-id="24b3f-131">Дата, связанная с этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="24b3f-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="24b3f-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="24b3f-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="24b3f-133">Int64</span><span class="sxs-lookup"><span data-stu-id="24b3f-133">Int64</span></span>|<span data-ttu-id="24b3f-134">Количество заданий черной и белой печати, завершенных принтером в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="24b3f-134">The number of black and white print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="24b3f-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="24b3f-135">completedColorJobCount</span></span>|<span data-ttu-id="24b3f-136">Int64</span><span class="sxs-lookup"><span data-stu-id="24b3f-136">Int64</span></span>|<span data-ttu-id="24b3f-137">Количество заданий цветного печати, завершенных принтером в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="24b3f-137">The number of color print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="24b3f-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="24b3f-138">incompleteJobCount</span></span>|<span data-ttu-id="24b3f-139">Int64</span><span class="sxs-lookup"><span data-stu-id="24b3f-139">Int64</span></span>|<span data-ttu-id="24b3f-140">Количество заданий печати, которые были в очереди для принтера, но не завершены, в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="24b3f-140">The number of print jobs that were queued for the printer, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24b3f-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="24b3f-141">JSON representation</span></span>

<span data-ttu-id="24b3f-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24b3f-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter"
}-->

```json
{
    "id": "String (identifier)",
    "printerId": "String (identifier)",
    "usageDate": "String (timestamp)",
    "completedBlackAndWhiteJobCount": 123456,
    "completedColorJobCount": 123456,
    "incompleteJobCount": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUsageSummaryByPrinter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

