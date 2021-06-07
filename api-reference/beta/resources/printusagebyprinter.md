---
title: тип ресурса printUsageByPrinter
description: Описывает активность печати для принтера в течение указанного периода времени (useDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2826e73ef68d9ee2162c6a2de0bbaba351fd87bd
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781307"
---
# <a name="printusagebyprinter-resource-type"></a><span data-ttu-id="3695a-103">тип ресурса printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="3695a-103">printUsageByPrinter resource type</span></span>

<span data-ttu-id="3695a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3695a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3695a-105">Описывает активность печати для принтера в течение указанного периода времени (useDate).</span><span class="sxs-lookup"><span data-stu-id="3695a-105">Describes print activity for a printer during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="3695a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3695a-106">Methods</span></span>

| <span data-ttu-id="3695a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3695a-107">Method</span></span>       | <span data-ttu-id="3695a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3695a-108">Return Type</span></span> | <span data-ttu-id="3695a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3695a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3695a-110">Список (ежедневно)</span><span class="sxs-lookup"><span data-stu-id="3695a-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagebyprinter.md) | [<span data-ttu-id="3695a-111">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="3695a-111">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="3695a-112">Получите список сводок об использовании ежедневной печати, сгруппив их по принтеру.</span><span class="sxs-lookup"><span data-stu-id="3695a-112">Get a list of daily print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="3695a-113">Список (ежемесячно)</span><span class="sxs-lookup"><span data-stu-id="3695a-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagebyprinter.md) | [<span data-ttu-id="3695a-114">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="3695a-114">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="3695a-115">Получите список ежемесячных сводок использования печати, сгруппив их по принтеру.</span><span class="sxs-lookup"><span data-stu-id="3695a-115">Get a list of monthly print usage summaries, grouped by printer.</span></span> |
| <span data-ttu-id="3695a-116">[получение](../api/printUsageByPrinter-get.md);</span><span class="sxs-lookup"><span data-stu-id="3695a-116">[Get](../api/printUsageByPrinter-get.md)</span></span> | [<span data-ttu-id="3695a-117">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="3695a-117">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="3695a-118">Ознакомьтесь с свойствами и отношениями объекта **printUsageByPrinter.**</span><span class="sxs-lookup"><span data-stu-id="3695a-118">Read the properties and relationships of a **printUsageByPrinter** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3695a-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="3695a-119">Properties</span></span>
| <span data-ttu-id="3695a-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="3695a-120">Property</span></span>     | <span data-ttu-id="3695a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3695a-121">Type</span></span>        | <span data-ttu-id="3695a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3695a-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3695a-123">id</span><span class="sxs-lookup"><span data-stu-id="3695a-123">id</span></span>|<span data-ttu-id="3695a-124">String</span><span class="sxs-lookup"><span data-stu-id="3695a-124">String</span></span>|<span data-ttu-id="3695a-125">ID этого сводки использования.</span><span class="sxs-lookup"><span data-stu-id="3695a-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="3695a-126">printerID</span><span class="sxs-lookup"><span data-stu-id="3695a-126">printerID</span></span>|<span data-ttu-id="3695a-127">String</span><span class="sxs-lookup"><span data-stu-id="3695a-127">String</span></span>|<span data-ttu-id="3695a-128">ID принтера, представленный этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="3695a-128">The ID of the printer represented by these statistics.</span></span>|
|<span data-ttu-id="3695a-129">useDate</span><span class="sxs-lookup"><span data-stu-id="3695a-129">usageDate</span></span>|<span data-ttu-id="3695a-130">Дата</span><span class="sxs-lookup"><span data-stu-id="3695a-130">Date</span></span>|<span data-ttu-id="3695a-131">Дата, связанная с этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="3695a-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="3695a-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="3695a-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="3695a-133">Int64</span><span class="sxs-lookup"><span data-stu-id="3695a-133">Int64</span></span>|<span data-ttu-id="3695a-134">Количество заданий черной и белой печати, завершенных принтером в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="3695a-134">The number of black and white print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="3695a-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="3695a-135">completedColorJobCount</span></span>|<span data-ttu-id="3695a-136">Int64</span><span class="sxs-lookup"><span data-stu-id="3695a-136">Int64</span></span>|<span data-ttu-id="3695a-137">Количество заданий цветного печати, завершенных принтером в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="3695a-137">The number of color print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="3695a-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="3695a-138">incompleteJobCount</span></span>|<span data-ttu-id="3695a-139">Int64</span><span class="sxs-lookup"><span data-stu-id="3695a-139">Int64</span></span>|<span data-ttu-id="3695a-140">Количество заданий печати, которые были в очереди для принтера, но не завершены, в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="3695a-140">The number of print jobs that were queued for the printer, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3695a-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3695a-141">JSON representation</span></span>

<span data-ttu-id="3695a-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3695a-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageByPrinter"
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
  "description": "printUsageByPrinter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

