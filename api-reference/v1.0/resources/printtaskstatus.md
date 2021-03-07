---
title: тип ресурса printTaskStatus
description: Представляет текущее состояние выполнения printTask.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ef5587050926fef5fa924f6d541de63d5b1d33aa
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518017"
---
# <a name="printtaskstatus-resource-type"></a><span data-ttu-id="2b027-103">тип ресурса printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="2b027-103">printTaskStatus resource type</span></span>

<span data-ttu-id="2b027-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b027-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2b027-105">Представляет текущее состояние выполнения [printTask](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="2b027-105">Represents the current execution status of a [printTask](printtask.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="2b027-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b027-106">Properties</span></span>
|<span data-ttu-id="2b027-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b027-107">Property</span></span>|<span data-ttu-id="2b027-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2b027-108">Type</span></span>|<span data-ttu-id="2b027-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2b027-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b027-110">state</span><span class="sxs-lookup"><span data-stu-id="2b027-110">state</span></span>|<span data-ttu-id="2b027-111">printTaskProcessingState</span><span class="sxs-lookup"><span data-stu-id="2b027-111">printTaskProcessingState</span></span>|<span data-ttu-id="2b027-112">Текущее состояние обработки [printTask](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="2b027-112">The current processing state of the [printTask](printtask.md).</span></span> <span data-ttu-id="2b027-113">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="2b027-113">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="2b027-114">description</span><span class="sxs-lookup"><span data-stu-id="2b027-114">description</span></span>|<span data-ttu-id="2b027-115">Строка</span><span class="sxs-lookup"><span data-stu-id="2b027-115">String</span></span>|<span data-ttu-id="2b027-116">Понятное для человека описание текущего состояния обработки [printTask](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="2b027-116">A human-readable description of the current processing state of the [printTask](printtask.md).</span></span>|

### <a name="printtaskprocessingstate-values"></a><span data-ttu-id="2b027-117">printTaskProcessingState values</span><span class="sxs-lookup"><span data-stu-id="2b027-117">printTaskProcessingState values</span></span>

|<span data-ttu-id="2b027-118">Элемент</span><span class="sxs-lookup"><span data-stu-id="2b027-118">Member</span></span>|<span data-ttu-id="2b027-119">Значение</span><span class="sxs-lookup"><span data-stu-id="2b027-119">Value</span></span>|<span data-ttu-id="2b027-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2b027-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b027-121">ожидание</span><span class="sxs-lookup"><span data-stu-id="2b027-121">pending</span></span>|<span data-ttu-id="2b027-122">0</span><span class="sxs-lookup"><span data-stu-id="2b027-122">0</span></span>|<span data-ttu-id="2b027-123">Выполнение задач находится в стадии ожидания.</span><span class="sxs-lookup"><span data-stu-id="2b027-123">Task execution is pending.</span></span>|
|<span data-ttu-id="2b027-124">обработка</span><span class="sxs-lookup"><span data-stu-id="2b027-124">processing</span></span>|<span data-ttu-id="2b027-125">1 </span><span class="sxs-lookup"><span data-stu-id="2b027-125">1</span></span>|<span data-ttu-id="2b027-126">Выполнение задач продолжается.</span><span class="sxs-lookup"><span data-stu-id="2b027-126">Task execution is in progress.</span></span>|
|<span data-ttu-id="2b027-127">завершено</span><span class="sxs-lookup"><span data-stu-id="2b027-127">completed</span></span>|<span data-ttu-id="2b027-128">2 </span><span class="sxs-lookup"><span data-stu-id="2b027-128">2</span></span>|<span data-ttu-id="2b027-129">Выполнение задач завершено.</span><span class="sxs-lookup"><span data-stu-id="2b027-129">Task execution has completed.</span></span>|
|<span data-ttu-id="2b027-130">прервано</span><span class="sxs-lookup"><span data-stu-id="2b027-130">aborted</span></span>|<span data-ttu-id="2b027-131">3 </span><span class="sxs-lookup"><span data-stu-id="2b027-131">3</span></span>|<span data-ttu-id="2b027-132">Выполнение задач было прервано.</span><span class="sxs-lookup"><span data-stu-id="2b027-132">Task execution was aborted.</span></span>|
|<span data-ttu-id="2b027-133">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="2b027-133">unknownFutureValue</span></span>|<span data-ttu-id="2b027-134">4 </span><span class="sxs-lookup"><span data-stu-id="2b027-134">4</span></span>|<span data-ttu-id="2b027-135">Эволюционирующее значение sentinel.</span><span class="sxs-lookup"><span data-stu-id="2b027-135">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="2b027-136">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="2b027-136">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b027-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b027-137">JSON representation</span></span>
<span data-ttu-id="2b027-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b027-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printTaskStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskStatus",
  "state": "String",
  "description": "String"
}
```

