---
title: тип ресурса printOperationStatus
description: Представляет текущее состояние длительной операции универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 787a584b32c6f34d78d14fa4d676b1be30a62c25
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517469"
---
# <a name="printoperationstatus-resource-type"></a><span data-ttu-id="0639c-103">тип ресурса printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="0639c-103">printOperationStatus resource type</span></span>

<span data-ttu-id="0639c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0639c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0639c-105">Представляет текущее состояние длительной операции универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="0639c-105">Represents the current status of a long-running Universal Print operation.</span></span>

## <a name="properties"></a><span data-ttu-id="0639c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0639c-106">Properties</span></span>
|<span data-ttu-id="0639c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0639c-107">Property</span></span>|<span data-ttu-id="0639c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0639c-108">Type</span></span>|<span data-ttu-id="0639c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0639c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0639c-110">state</span><span class="sxs-lookup"><span data-stu-id="0639c-110">state</span></span>|<span data-ttu-id="0639c-111">printOperationProcessingState</span><span class="sxs-lookup"><span data-stu-id="0639c-111">printOperationProcessingState</span></span>|<span data-ttu-id="0639c-112">Текущее состояние обработки printOperation.</span><span class="sxs-lookup"><span data-stu-id="0639c-112">The printOperation's current processing state.</span></span> <span data-ttu-id="0639c-113">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0639c-113">Valid values are described in the following table.</span></span> <span data-ttu-id="0639c-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0639c-114">Read-only.</span></span>|
|<span data-ttu-id="0639c-115">description</span><span class="sxs-lookup"><span data-stu-id="0639c-115">description</span></span>|<span data-ttu-id="0639c-116">Строка</span><span class="sxs-lookup"><span data-stu-id="0639c-116">String</span></span>|<span data-ttu-id="0639c-117">Описание текущего состояния обработки printOperation с читаемым человеком.</span><span class="sxs-lookup"><span data-stu-id="0639c-117">A human-readable description of the printOperation's current processing state.</span></span> <span data-ttu-id="0639c-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0639c-118">Read-only.</span></span>|

### <a name="printoperationprocessingstate-values"></a><span data-ttu-id="0639c-119">значения printOperationProcessingState</span><span class="sxs-lookup"><span data-stu-id="0639c-119">printOperationProcessingState values</span></span>

|<span data-ttu-id="0639c-120">Элемент</span><span class="sxs-lookup"><span data-stu-id="0639c-120">Member</span></span>|<span data-ttu-id="0639c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0639c-121">Value</span></span>|<span data-ttu-id="0639c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0639c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0639c-123">notStarted</span><span class="sxs-lookup"><span data-stu-id="0639c-123">notStarted</span></span>|<span data-ttu-id="0639c-124">0</span><span class="sxs-lookup"><span data-stu-id="0639c-124">0</span></span>|<span data-ttu-id="0639c-125">Операция еще не началась.</span><span class="sxs-lookup"><span data-stu-id="0639c-125">The operation has not yet started.</span></span>|
|<span data-ttu-id="0639c-126">запуск</span><span class="sxs-lookup"><span data-stu-id="0639c-126">running</span></span>|<span data-ttu-id="0639c-127">1 </span><span class="sxs-lookup"><span data-stu-id="0639c-127">1</span></span>|<span data-ttu-id="0639c-128">Операция запущена.</span><span class="sxs-lookup"><span data-stu-id="0639c-128">The operation is running.</span></span>|
|<span data-ttu-id="0639c-129">успешно</span><span class="sxs-lookup"><span data-stu-id="0639c-129">succeeded</span></span>|<span data-ttu-id="0639c-130">2 </span><span class="sxs-lookup"><span data-stu-id="0639c-130">2</span></span>|<span data-ttu-id="0639c-131">Операция выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="0639c-131">The operation completed successfully.</span></span>|
|<span data-ttu-id="0639c-132">не удалось</span><span class="sxs-lookup"><span data-stu-id="0639c-132">failed</span></span>|<span data-ttu-id="0639c-133">3 </span><span class="sxs-lookup"><span data-stu-id="0639c-133">3</span></span>|<span data-ttu-id="0639c-134">Сбой операции.</span><span class="sxs-lookup"><span data-stu-id="0639c-134">The operation failed.</span></span>|
|<span data-ttu-id="0639c-135">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="0639c-135">unknownFutureValue</span></span>|<span data-ttu-id="0639c-136">4 </span><span class="sxs-lookup"><span data-stu-id="0639c-136">4</span></span>|<span data-ttu-id="0639c-137">Эволюционирующее значение sentinel.</span><span class="sxs-lookup"><span data-stu-id="0639c-137">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="0639c-138">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="0639c-138">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0639c-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0639c-139">JSON representation</span></span>
<span data-ttu-id="0639c-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0639c-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printOperationStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperationStatus",
  "state": "String",
  "description": "String"
}
```

