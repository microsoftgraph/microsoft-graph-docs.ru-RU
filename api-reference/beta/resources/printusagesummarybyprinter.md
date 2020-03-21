---
title: Тип ресурса Принтусажесуммарибипринтер
description: Описывает действия печати для принтера в указанный период времени (Усажедате).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 86d7b4eb107ac6e2732e32bf55a65a7125edb529
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896053"
---
# <a name="printusagesummarybyprinter-resource-type"></a><span data-ttu-id="1777b-103">Тип ресурса Принтусажесуммарибипринтер</span><span class="sxs-lookup"><span data-stu-id="1777b-103">printUsageSummaryByPrinter resource type</span></span>

<span data-ttu-id="1777b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1777b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1777b-105">Описывает действия печати для принтера в указанный период времени (Усажедате).</span><span class="sxs-lookup"><span data-stu-id="1777b-105">Describes print activity for a printer during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="1777b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1777b-106">Methods</span></span>

| <span data-ttu-id="1777b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1777b-107">Method</span></span>       | <span data-ttu-id="1777b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1777b-108">Return Type</span></span> | <span data-ttu-id="1777b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1777b-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1777b-110">Список (ежедневно)</span><span class="sxs-lookup"><span data-stu-id="1777b-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagesummariesbyprinter.md) | [<span data-ttu-id="1777b-111">принтусажесуммарибипринтер</span><span class="sxs-lookup"><span data-stu-id="1777b-111">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="1777b-112">Получите список ежедневных сводок использования, сгруппированных по принтерам.</span><span class="sxs-lookup"><span data-stu-id="1777b-112">Get a list of daily print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="1777b-113">Список (ежемесячно)</span><span class="sxs-lookup"><span data-stu-id="1777b-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagesummariesbyprinter.md) | [<span data-ttu-id="1777b-114">принтусажесуммарибипринтер</span><span class="sxs-lookup"><span data-stu-id="1777b-114">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="1777b-115">Получение списка ежемесячных сводок использования печати с группировкой по принтерам.</span><span class="sxs-lookup"><span data-stu-id="1777b-115">Get a list of monthly print usage summaries, grouped by printer.</span></span> |
| <span data-ttu-id="1777b-116">[получение](../api/printusagesummarybyprinter-get.md);</span><span class="sxs-lookup"><span data-stu-id="1777b-116">[Get](../api/printusagesummarybyprinter-get.md)</span></span> | [<span data-ttu-id="1777b-117">принтусажесуммарибипринтер</span><span class="sxs-lookup"><span data-stu-id="1777b-117">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="1777b-118">Чтение свойств и связей объекта **принтусажесуммарибипринтер** .</span><span class="sxs-lookup"><span data-stu-id="1777b-118">Read the properties and relationships of a **printUsageSummaryByPrinter** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1777b-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="1777b-119">Properties</span></span>
| <span data-ttu-id="1777b-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="1777b-120">Property</span></span>     | <span data-ttu-id="1777b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1777b-121">Type</span></span>        | <span data-ttu-id="1777b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1777b-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1777b-123">id</span><span class="sxs-lookup"><span data-stu-id="1777b-123">id</span></span>|<span data-ttu-id="1777b-124">String</span><span class="sxs-lookup"><span data-stu-id="1777b-124">String</span></span>|<span data-ttu-id="1777b-125">Идентификатор этой сводки использования.</span><span class="sxs-lookup"><span data-stu-id="1777b-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="1777b-126">принтерид</span><span class="sxs-lookup"><span data-stu-id="1777b-126">printerID</span></span>|<span data-ttu-id="1777b-127">String</span><span class="sxs-lookup"><span data-stu-id="1777b-127">String</span></span>|<span data-ttu-id="1777b-128">ИДЕНТИФИКАТОР принтера, представленный данными статистикой.</span><span class="sxs-lookup"><span data-stu-id="1777b-128">The ID of the printer represented by these statistics.</span></span>|
|<span data-ttu-id="1777b-129">усажедате</span><span class="sxs-lookup"><span data-stu-id="1777b-129">usageDate</span></span>|<span data-ttu-id="1777b-130">Дата</span><span class="sxs-lookup"><span data-stu-id="1777b-130">Date</span></span>|<span data-ttu-id="1777b-131">Дата, связанная с этими статистикой.</span><span class="sxs-lookup"><span data-stu-id="1777b-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="1777b-132">комплетедблаккандвхитежобкаунт</span><span class="sxs-lookup"><span data-stu-id="1777b-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="1777b-133">Int64</span><span class="sxs-lookup"><span data-stu-id="1777b-133">Int64</span></span>|<span data-ttu-id="1777b-134">Количество черно-белых заданий печати, выполненных принтером на связанную дату.</span><span class="sxs-lookup"><span data-stu-id="1777b-134">The number of black and white print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="1777b-135">комплетедколоржобкаунт</span><span class="sxs-lookup"><span data-stu-id="1777b-135">completedColorJobCount</span></span>|<span data-ttu-id="1777b-136">Int64</span><span class="sxs-lookup"><span data-stu-id="1777b-136">Int64</span></span>|<span data-ttu-id="1777b-137">Число заданий цветной печати, выполненных принтером на связанную дату.</span><span class="sxs-lookup"><span data-stu-id="1777b-137">The number of color print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="1777b-138">инкомплетежобкаунт</span><span class="sxs-lookup"><span data-stu-id="1777b-138">incompleteJobCount</span></span>|<span data-ttu-id="1777b-139">Int64</span><span class="sxs-lookup"><span data-stu-id="1777b-139">Int64</span></span>|<span data-ttu-id="1777b-140">Количество заданий печати, которые были поставлены в очередь для принтера, но не завершены, на соответствующую дату.</span><span class="sxs-lookup"><span data-stu-id="1777b-140">The number of print jobs that were queued for the printer, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1777b-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1777b-141">JSON representation</span></span>

<span data-ttu-id="1777b-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1777b-142">The following is a JSON representation of the resource.</span></span>

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