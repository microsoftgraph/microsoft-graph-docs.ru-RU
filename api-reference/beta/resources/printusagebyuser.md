---
title: тип ресурса printUsageByUser
description: Описывает действия печати для пользователя в течение определенного периода времени (useDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4b4809f77e7ceeba79ea5b7e75737fb0750cc4dc
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781298"
---
# <a name="printusagebyuser-resource-type"></a><span data-ttu-id="f8eb6-103">тип ресурса printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="f8eb6-103">printUsageByUser resource type</span></span>

<span data-ttu-id="f8eb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8eb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8eb6-105">Описывает действия печати для пользователя в течение определенного периода времени (useDate).</span><span class="sxs-lookup"><span data-stu-id="f8eb6-105">Describes print activity for a user during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="f8eb6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f8eb6-106">Methods</span></span>

| <span data-ttu-id="f8eb6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f8eb6-107">Method</span></span>       | <span data-ttu-id="f8eb6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f8eb6-108">Return Type</span></span> | <span data-ttu-id="f8eb6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f8eb6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f8eb6-110">Список (ежедневно)</span><span class="sxs-lookup"><span data-stu-id="f8eb6-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagebyuser.md) | [<span data-ttu-id="f8eb6-111">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="f8eb6-111">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="f8eb6-112">Получите список сводок ежедневного использования печати, сгруппив их по пользователю.</span><span class="sxs-lookup"><span data-stu-id="f8eb6-112">Get a list of daily print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="f8eb6-113">Список (ежемесячно)</span><span class="sxs-lookup"><span data-stu-id="f8eb6-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagebyuser.md) | [<span data-ttu-id="f8eb6-114">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="f8eb6-114">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="f8eb6-115">Получите список ежемесячных сводок использования печати, сгруппив их по пользователю.</span><span class="sxs-lookup"><span data-stu-id="f8eb6-115">Get a list of monthly print usage summaries, grouped by user.</span></span> |
| <span data-ttu-id="f8eb6-116">[получение](../api/printusagebyuser-get.md);</span><span class="sxs-lookup"><span data-stu-id="f8eb6-116">[Get](../api/printusagebyuser-get.md)</span></span> | [<span data-ttu-id="f8eb6-117">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="f8eb6-117">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="f8eb6-118">Чтение свойств и связей объекта printUsageByUser.</span><span class="sxs-lookup"><span data-stu-id="f8eb6-118">Read properties and relationships of a printUsageByUser object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f8eb6-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8eb6-119">Properties</span></span>
| <span data-ttu-id="f8eb6-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8eb6-120">Property</span></span>     | <span data-ttu-id="f8eb6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f8eb6-121">Type</span></span>        | <span data-ttu-id="f8eb6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f8eb6-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f8eb6-123">id</span><span class="sxs-lookup"><span data-stu-id="f8eb6-123">id</span></span>|<span data-ttu-id="f8eb6-124">String</span><span class="sxs-lookup"><span data-stu-id="f8eb6-124">String</span></span>|<span data-ttu-id="f8eb6-125">ID этого сводки использования.</span><span class="sxs-lookup"><span data-stu-id="f8eb6-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="f8eb6-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8eb6-126">userPrincipalName</span></span>|<span data-ttu-id="f8eb6-127">String</span><span class="sxs-lookup"><span data-stu-id="f8eb6-127">String</span></span>|<span data-ttu-id="f8eb6-128">UpN пользователя, представленного этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="f8eb6-128">The UPN of the user represented by these statistics.</span></span>|
|<span data-ttu-id="f8eb6-129">useDate</span><span class="sxs-lookup"><span data-stu-id="f8eb6-129">usageDate</span></span>|<span data-ttu-id="f8eb6-130">Дата</span><span class="sxs-lookup"><span data-stu-id="f8eb6-130">Date</span></span>|<span data-ttu-id="f8eb6-131">Дата, связанная с этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="f8eb6-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="f8eb6-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="f8eb6-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="f8eb6-133">Int64</span><span class="sxs-lookup"><span data-stu-id="f8eb6-133">Int64</span></span>|<span data-ttu-id="f8eb6-134">Количество заданий черной и белой печати, завершенных от имени пользователя в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="f8eb6-134">The number of black and white print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="f8eb6-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="f8eb6-135">completedColorJobCount</span></span>|<span data-ttu-id="f8eb6-136">Int64</span><span class="sxs-lookup"><span data-stu-id="f8eb6-136">Int64</span></span>|<span data-ttu-id="f8eb6-137">Количество заданий цветной печати, завершенных от имени пользователя в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="f8eb6-137">The number of color print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="f8eb6-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="f8eb6-138">incompleteJobCount</span></span>|<span data-ttu-id="f8eb6-139">Int64</span><span class="sxs-lookup"><span data-stu-id="f8eb6-139">Int64</span></span>|<span data-ttu-id="f8eb6-140">Количество заданий печати, которые были в очереди от имени пользователя, но не завершены, в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="f8eb6-140">The number of print jobs that were queued on behalf of the user, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8eb6-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8eb6-141">JSON representation</span></span>

<span data-ttu-id="f8eb6-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8eb6-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageByUser"
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
  "description": "printUsageByUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

