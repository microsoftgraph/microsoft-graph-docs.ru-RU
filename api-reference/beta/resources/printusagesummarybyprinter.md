---
title: Тип ресурса Принтусажесуммарибипринтер
description: Описывает действия печати для принтера в указанный период времени (Усажедате).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4d33ab99780f980dcc24e267ba1ac6603f602aa2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070658"
---
# <a name="printusagesummarybyprinter-resource-type"></a><span data-ttu-id="8bbb6-103">Тип ресурса Принтусажесуммарибипринтер</span><span class="sxs-lookup"><span data-stu-id="8bbb6-103">printUsageSummaryByPrinter resource type</span></span>

<span data-ttu-id="8bbb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bbb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bbb6-105">Описывает действия печати для принтера в указанный период времени (Усажедате).</span><span class="sxs-lookup"><span data-stu-id="8bbb6-105">Describes print activity for a printer during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="8bbb6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8bbb6-106">Methods</span></span>

| <span data-ttu-id="8bbb6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8bbb6-107">Method</span></span>       | <span data-ttu-id="8bbb6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8bbb6-108">Return Type</span></span> | <span data-ttu-id="8bbb6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8bbb6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8bbb6-110">Список (ежедневно)</span><span class="sxs-lookup"><span data-stu-id="8bbb6-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagesummariesbyprinter.md) | [<span data-ttu-id="8bbb6-111">принтусажесуммарибипринтер</span><span class="sxs-lookup"><span data-stu-id="8bbb6-111">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="8bbb6-112">Получите список ежедневных сводок использования, сгруппированных по принтерам.</span><span class="sxs-lookup"><span data-stu-id="8bbb6-112">Get a list of daily print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="8bbb6-113">Список (ежемесячно)</span><span class="sxs-lookup"><span data-stu-id="8bbb6-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagesummariesbyprinter.md) | [<span data-ttu-id="8bbb6-114">принтусажесуммарибипринтер</span><span class="sxs-lookup"><span data-stu-id="8bbb6-114">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="8bbb6-115">Получение списка ежемесячных сводок использования печати с группировкой по принтерам.</span><span class="sxs-lookup"><span data-stu-id="8bbb6-115">Get a list of monthly print usage summaries, grouped by printer.</span></span> |
| <span data-ttu-id="8bbb6-116">[получение](../api/printusagesummarybyprinter-get.md);</span><span class="sxs-lookup"><span data-stu-id="8bbb6-116">[Get](../api/printusagesummarybyprinter-get.md)</span></span> | [<span data-ttu-id="8bbb6-117">принтусажесуммарибипринтер</span><span class="sxs-lookup"><span data-stu-id="8bbb6-117">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="8bbb6-118">Чтение свойств и связей объекта **принтусажесуммарибипринтер** .</span><span class="sxs-lookup"><span data-stu-id="8bbb6-118">Read the properties and relationships of a **printUsageSummaryByPrinter** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8bbb6-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bbb6-119">Properties</span></span>
| <span data-ttu-id="8bbb6-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bbb6-120">Property</span></span>     | <span data-ttu-id="8bbb6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8bbb6-121">Type</span></span>        | <span data-ttu-id="8bbb6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8bbb6-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8bbb6-123">id</span><span class="sxs-lookup"><span data-stu-id="8bbb6-123">id</span></span>|<span data-ttu-id="8bbb6-124">String</span><span class="sxs-lookup"><span data-stu-id="8bbb6-124">String</span></span>|<span data-ttu-id="8bbb6-125">Идентификатор этой сводки использования.</span><span class="sxs-lookup"><span data-stu-id="8bbb6-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="8bbb6-126">принтерид</span><span class="sxs-lookup"><span data-stu-id="8bbb6-126">printerID</span></span>|<span data-ttu-id="8bbb6-127">String</span><span class="sxs-lookup"><span data-stu-id="8bbb6-127">String</span></span>|<span data-ttu-id="8bbb6-128">ИДЕНТИФИКАТОР принтера, представленный данными статистикой.</span><span class="sxs-lookup"><span data-stu-id="8bbb6-128">The ID of the printer represented by these statistics.</span></span>|
|<span data-ttu-id="8bbb6-129">усажедате</span><span class="sxs-lookup"><span data-stu-id="8bbb6-129">usageDate</span></span>|<span data-ttu-id="8bbb6-130">Дата</span><span class="sxs-lookup"><span data-stu-id="8bbb6-130">Date</span></span>|<span data-ttu-id="8bbb6-131">Дата, связанная с этими статистикой.</span><span class="sxs-lookup"><span data-stu-id="8bbb6-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="8bbb6-132">комплетедблаккандвхитежобкаунт</span><span class="sxs-lookup"><span data-stu-id="8bbb6-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="8bbb6-133">Int64</span><span class="sxs-lookup"><span data-stu-id="8bbb6-133">Int64</span></span>|<span data-ttu-id="8bbb6-134">Количество черно-белых заданий печати, выполненных принтером на связанную дату.</span><span class="sxs-lookup"><span data-stu-id="8bbb6-134">The number of black and white print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="8bbb6-135">комплетедколоржобкаунт</span><span class="sxs-lookup"><span data-stu-id="8bbb6-135">completedColorJobCount</span></span>|<span data-ttu-id="8bbb6-136">Int64</span><span class="sxs-lookup"><span data-stu-id="8bbb6-136">Int64</span></span>|<span data-ttu-id="8bbb6-137">Число заданий цветной печати, выполненных принтером на связанную дату.</span><span class="sxs-lookup"><span data-stu-id="8bbb6-137">The number of color print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="8bbb6-138">инкомплетежобкаунт</span><span class="sxs-lookup"><span data-stu-id="8bbb6-138">incompleteJobCount</span></span>|<span data-ttu-id="8bbb6-139">Int64</span><span class="sxs-lookup"><span data-stu-id="8bbb6-139">Int64</span></span>|<span data-ttu-id="8bbb6-140">Количество заданий печати, которые были поставлены в очередь для принтера, но не завершены, на соответствующую дату.</span><span class="sxs-lookup"><span data-stu-id="8bbb6-140">The number of print jobs that were queued for the printer, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bbb6-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bbb6-141">JSON representation</span></span>

<span data-ttu-id="8bbb6-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bbb6-142">The following is a JSON representation of the resource.</span></span>

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

