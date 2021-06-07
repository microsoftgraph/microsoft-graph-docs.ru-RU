---
title: тип ресурса printUsageSummaryByUser
description: Описывает действия печати для пользователя в течение определенного периода времени (useDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bba9f57799a36bef4a90b7c514a5be4b4846565e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753610"
---
# <a name="printusagesummarybyuser-resource-type"></a><span data-ttu-id="e3936-103">тип ресурса printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="e3936-103">printUsageSummaryByUser resource type</span></span>

<span data-ttu-id="e3936-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3936-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3936-105">Описывает действия печати для пользователя в течение определенного периода времени (useDate).</span><span class="sxs-lookup"><span data-stu-id="e3936-105">Describes print activity for a user during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="e3936-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e3936-106">Methods</span></span>

| <span data-ttu-id="e3936-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e3936-107">Method</span></span>       | <span data-ttu-id="e3936-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e3936-108">Return Type</span></span> | <span data-ttu-id="e3936-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e3936-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e3936-110">Список (ежедневно)</span><span class="sxs-lookup"><span data-stu-id="e3936-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagesummariesbyuser.md) | [<span data-ttu-id="e3936-111">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="e3936-111">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="e3936-112">Получите список сводок ежедневного использования печати, сгруппив их по пользователю.</span><span class="sxs-lookup"><span data-stu-id="e3936-112">Get a list of daily print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="e3936-113">Список (ежемесячно)</span><span class="sxs-lookup"><span data-stu-id="e3936-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagesummariesbyuser.md) | [<span data-ttu-id="e3936-114">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="e3936-114">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="e3936-115">Получите список ежемесячных сводок использования печати, сгруппив их по пользователю.</span><span class="sxs-lookup"><span data-stu-id="e3936-115">Get a list of monthly print usage summaries, grouped by user.</span></span> |
| <span data-ttu-id="e3936-116">[получение](../api/printusagesummarybyuser-get.md);</span><span class="sxs-lookup"><span data-stu-id="e3936-116">[Get](../api/printusagesummarybyuser-get.md)</span></span> | [<span data-ttu-id="e3936-117">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="e3936-117">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="e3936-118">Чтение свойств и связей объекта printUsageSummaryByUser.</span><span class="sxs-lookup"><span data-stu-id="e3936-118">Read properties and relationships of a printUsageSummaryByUser object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e3936-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3936-119">Properties</span></span>
| <span data-ttu-id="e3936-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3936-120">Property</span></span>     | <span data-ttu-id="e3936-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e3936-121">Type</span></span>        | <span data-ttu-id="e3936-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e3936-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e3936-123">id</span><span class="sxs-lookup"><span data-stu-id="e3936-123">id</span></span>|<span data-ttu-id="e3936-124">String</span><span class="sxs-lookup"><span data-stu-id="e3936-124">String</span></span>|<span data-ttu-id="e3936-125">ID этого сводки использования.</span><span class="sxs-lookup"><span data-stu-id="e3936-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="e3936-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e3936-126">userPrincipalName</span></span>|<span data-ttu-id="e3936-127">String</span><span class="sxs-lookup"><span data-stu-id="e3936-127">String</span></span>|<span data-ttu-id="e3936-128">UpN пользователя, представленного этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="e3936-128">The UPN of the user represented by these statistics.</span></span>|
|<span data-ttu-id="e3936-129">useDate</span><span class="sxs-lookup"><span data-stu-id="e3936-129">usageDate</span></span>|<span data-ttu-id="e3936-130">Дата</span><span class="sxs-lookup"><span data-stu-id="e3936-130">Date</span></span>|<span data-ttu-id="e3936-131">Дата, связанная с этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="e3936-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="e3936-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="e3936-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="e3936-133">Int64</span><span class="sxs-lookup"><span data-stu-id="e3936-133">Int64</span></span>|<span data-ttu-id="e3936-134">Количество заданий черной и белой печати, завершенных от имени пользователя в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="e3936-134">The number of black and white print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="e3936-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="e3936-135">completedColorJobCount</span></span>|<span data-ttu-id="e3936-136">Int64</span><span class="sxs-lookup"><span data-stu-id="e3936-136">Int64</span></span>|<span data-ttu-id="e3936-137">Количество заданий цветной печати, завершенных от имени пользователя в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="e3936-137">The number of color print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="e3936-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="e3936-138">incompleteJobCount</span></span>|<span data-ttu-id="e3936-139">Int64</span><span class="sxs-lookup"><span data-stu-id="e3936-139">Int64</span></span>|<span data-ttu-id="e3936-140">Количество заданий печати, которые были в очереди от имени пользователя, но не завершены, в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="e3936-140">The number of print jobs that were queued on behalf of the user, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3936-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3936-141">JSON representation</span></span>

<span data-ttu-id="e3936-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3936-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByUser"
}-->

```json
{
    "id": "String (identifier)",
    "userPrincipalName": "String (identifier)",
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
  "description": "printUsageSummaryByUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

