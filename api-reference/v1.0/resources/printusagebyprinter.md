---
title: тип ресурса printUsageByPrinter
description: Описывает активность печати для принтера в течение указанного периода времени (useDate).
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 8c5a69d01f0b8da05a5f72f5c2c7d9bacf10ff1a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518013"
---
# <a name="printusagebyprinter-resource-type"></a><span data-ttu-id="45b61-103">тип ресурса printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="45b61-103">printUsageByPrinter resource type</span></span>

<span data-ttu-id="45b61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45b61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="45b61-105">Описывает активность печати для принтера в течение указанного периода времени (useDate).</span><span class="sxs-lookup"><span data-stu-id="45b61-105">Describes print activity for a printer during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="45b61-106">Методы</span><span class="sxs-lookup"><span data-stu-id="45b61-106">Methods</span></span>
|<span data-ttu-id="45b61-107">Метод</span><span class="sxs-lookup"><span data-stu-id="45b61-107">Method</span></span>|<span data-ttu-id="45b61-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="45b61-108">Return type</span></span>|<span data-ttu-id="45b61-109">Описание</span><span class="sxs-lookup"><span data-stu-id="45b61-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="45b61-110">Список (ежедневно)</span><span class="sxs-lookup"><span data-stu-id="45b61-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagebyprinter.md) | [<span data-ttu-id="45b61-111">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="45b61-111">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="45b61-112">Получите список сводок об использовании ежедневной печати, сгруппив их по принтеру.</span><span class="sxs-lookup"><span data-stu-id="45b61-112">Get a list of daily print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="45b61-113">Список (ежемесячно)</span><span class="sxs-lookup"><span data-stu-id="45b61-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagebyprinter.md) | [<span data-ttu-id="45b61-114">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="45b61-114">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="45b61-115">Получите список ежемесячных сводок использования печати, сгруппив их по принтеру.</span><span class="sxs-lookup"><span data-stu-id="45b61-115">Get a list of monthly print usage summaries, grouped by printer.</span></span> |
| <span data-ttu-id="45b61-116">[получение](../api/printUsageByPrinter-get.md);</span><span class="sxs-lookup"><span data-stu-id="45b61-116">[Get](../api/printUsageByPrinter-get.md)</span></span> | [<span data-ttu-id="45b61-117">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="45b61-117">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="45b61-118">Ознакомьтесь с свойствами и отношениями объекта **printUsageByPrinter.**</span><span class="sxs-lookup"><span data-stu-id="45b61-118">Read the properties and relationships of a **printUsageByPrinter** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="45b61-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="45b61-119">Properties</span></span>
|<span data-ttu-id="45b61-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="45b61-120">Property</span></span>|<span data-ttu-id="45b61-121">Тип</span><span class="sxs-lookup"><span data-stu-id="45b61-121">Type</span></span>|<span data-ttu-id="45b61-122">Описание</span><span class="sxs-lookup"><span data-stu-id="45b61-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45b61-123">id</span><span class="sxs-lookup"><span data-stu-id="45b61-123">id</span></span>|<span data-ttu-id="45b61-124">Строка</span><span class="sxs-lookup"><span data-stu-id="45b61-124">String</span></span>|<span data-ttu-id="45b61-125">ID этого сводки использования.</span><span class="sxs-lookup"><span data-stu-id="45b61-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="45b61-126">printerID</span><span class="sxs-lookup"><span data-stu-id="45b61-126">printerID</span></span>|<span data-ttu-id="45b61-127">Строка</span><span class="sxs-lookup"><span data-stu-id="45b61-127">String</span></span>|<span data-ttu-id="45b61-128">ID принтера, представленный этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="45b61-128">The ID of the printer represented by these statistics.</span></span>|
|<span data-ttu-id="45b61-129">useDate</span><span class="sxs-lookup"><span data-stu-id="45b61-129">usageDate</span></span>|<span data-ttu-id="45b61-130">Дата</span><span class="sxs-lookup"><span data-stu-id="45b61-130">Date</span></span>|<span data-ttu-id="45b61-131">Дата, связанная с этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="45b61-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="45b61-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="45b61-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="45b61-133">Int64</span><span class="sxs-lookup"><span data-stu-id="45b61-133">Int64</span></span>|<span data-ttu-id="45b61-134">Количество заданий черной и белой печати, завершенных принтером в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="45b61-134">The number of black and white print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="45b61-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="45b61-135">completedColorJobCount</span></span>|<span data-ttu-id="45b61-136">Int64</span><span class="sxs-lookup"><span data-stu-id="45b61-136">Int64</span></span>|<span data-ttu-id="45b61-137">Количество заданий цветного печати, завершенных принтером в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="45b61-137">The number of color print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="45b61-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="45b61-138">incompleteJobCount</span></span>|<span data-ttu-id="45b61-139">Int64</span><span class="sxs-lookup"><span data-stu-id="45b61-139">Int64</span></span>|<span data-ttu-id="45b61-140">Количество заданий печати, которые были в очереди для принтера, но не завершены, в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="45b61-140">The number of print jobs that were queued for the printer, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45b61-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45b61-141">JSON representation</span></span>
<span data-ttu-id="45b61-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45b61-142">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByPrinter",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByPrinter",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "printerId": "String"
}
```

