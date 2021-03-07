---
title: тип ресурса printUsageByUser
description: Описывает действия печати для пользователя в течение определенного периода времени (useDate).
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c478a4f9827de96d4db0da5d8533628bd8468d98
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518012"
---
# <a name="printusagebyuser-resource-type"></a><span data-ttu-id="eaeff-103">тип ресурса printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="eaeff-103">printUsageByUser resource type</span></span>

<span data-ttu-id="eaeff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaeff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="eaeff-105">Описывает действия печати для пользователя в течение определенного периода времени (useDate).</span><span class="sxs-lookup"><span data-stu-id="eaeff-105">Describes print activity for a user during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="eaeff-106">Методы</span><span class="sxs-lookup"><span data-stu-id="eaeff-106">Methods</span></span>
|<span data-ttu-id="eaeff-107">Метод</span><span class="sxs-lookup"><span data-stu-id="eaeff-107">Method</span></span>|<span data-ttu-id="eaeff-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="eaeff-108">Return type</span></span>|<span data-ttu-id="eaeff-109">Описание</span><span class="sxs-lookup"><span data-stu-id="eaeff-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="eaeff-110">Список (ежедневно)</span><span class="sxs-lookup"><span data-stu-id="eaeff-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagebyuser.md) | [<span data-ttu-id="eaeff-111">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="eaeff-111">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="eaeff-112">Получите список сводок ежедневного использования печати, сгруппив их по пользователю.</span><span class="sxs-lookup"><span data-stu-id="eaeff-112">Get a list of daily print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="eaeff-113">Список (ежемесячно)</span><span class="sxs-lookup"><span data-stu-id="eaeff-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagebyuser.md) | [<span data-ttu-id="eaeff-114">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="eaeff-114">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="eaeff-115">Получите список ежемесячных сводок использования печати, сгруппив их по пользователю.</span><span class="sxs-lookup"><span data-stu-id="eaeff-115">Get a list of monthly print usage summaries, grouped by user.</span></span> |
| <span data-ttu-id="eaeff-116">[получение](../api/printusagebyuser-get.md);</span><span class="sxs-lookup"><span data-stu-id="eaeff-116">[Get](../api/printusagebyuser-get.md)</span></span> | [<span data-ttu-id="eaeff-117">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="eaeff-117">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="eaeff-118">Чтение свойств и связей объекта printUsageByUser.</span><span class="sxs-lookup"><span data-stu-id="eaeff-118">Read properties and relationships of a printUsageByUser object.</span></span> |

## <a name="properties"></a><span data-ttu-id="eaeff-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="eaeff-119">Properties</span></span>
|<span data-ttu-id="eaeff-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="eaeff-120">Property</span></span>|<span data-ttu-id="eaeff-121">Тип</span><span class="sxs-lookup"><span data-stu-id="eaeff-121">Type</span></span>|<span data-ttu-id="eaeff-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eaeff-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaeff-123">id</span><span class="sxs-lookup"><span data-stu-id="eaeff-123">id</span></span>|<span data-ttu-id="eaeff-124">Строка</span><span class="sxs-lookup"><span data-stu-id="eaeff-124">String</span></span>|<span data-ttu-id="eaeff-125">ID этого сводки использования.</span><span class="sxs-lookup"><span data-stu-id="eaeff-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="eaeff-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eaeff-126">userPrincipalName</span></span>|<span data-ttu-id="eaeff-127">String</span><span class="sxs-lookup"><span data-stu-id="eaeff-127">String</span></span>|<span data-ttu-id="eaeff-128">UpN пользователя, представленного этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="eaeff-128">The UPN of the user represented by these statistics.</span></span>|
|<span data-ttu-id="eaeff-129">useDate</span><span class="sxs-lookup"><span data-stu-id="eaeff-129">usageDate</span></span>|<span data-ttu-id="eaeff-130">Дата</span><span class="sxs-lookup"><span data-stu-id="eaeff-130">Date</span></span>|<span data-ttu-id="eaeff-131">Дата, связанная с этими статистическими данными.</span><span class="sxs-lookup"><span data-stu-id="eaeff-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="eaeff-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="eaeff-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="eaeff-133">Int64</span><span class="sxs-lookup"><span data-stu-id="eaeff-133">Int64</span></span>|<span data-ttu-id="eaeff-134">Количество заданий черной и белой печати, завершенных от имени пользователя в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="eaeff-134">The number of black and white print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="eaeff-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="eaeff-135">completedColorJobCount</span></span>|<span data-ttu-id="eaeff-136">Int64</span><span class="sxs-lookup"><span data-stu-id="eaeff-136">Int64</span></span>|<span data-ttu-id="eaeff-137">Количество заданий цветной печати, завершенных от имени пользователя в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="eaeff-137">The number of color print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="eaeff-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="eaeff-138">incompleteJobCount</span></span>|<span data-ttu-id="eaeff-139">Int64</span><span class="sxs-lookup"><span data-stu-id="eaeff-139">Int64</span></span>|<span data-ttu-id="eaeff-140">Количество заданий печати, которые были в очереди от имени пользователя, но не завершены, в связанную дату.</span><span class="sxs-lookup"><span data-stu-id="eaeff-140">The number of print jobs that were queued on behalf of the user, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eaeff-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eaeff-141">JSON representation</span></span>
<span data-ttu-id="eaeff-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eaeff-142">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByUser",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "userPrincipalName": "String"
}
```

