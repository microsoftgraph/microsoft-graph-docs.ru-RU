---
title: Тип ресурса Принтоператионстатус
description: Представляет текущее состояние длительной универсальной операции печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 14c66cf59dc1715a16bd786657202a554d7c1753
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052553"
---
# <a name="printoperationstatus-complex-type"></a><span data-ttu-id="f2de4-103">сложный тип Принтоператионстатус</span><span class="sxs-lookup"><span data-stu-id="f2de4-103">printOperationStatus complex type</span></span>

<span data-ttu-id="f2de4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2de4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2de4-105">Представляет текущее состояние длительной универсальной операции печати.</span><span class="sxs-lookup"><span data-stu-id="f2de4-105">Represents the current status of a long-running Universal Print operation.</span></span>

## <a name="properties"></a><span data-ttu-id="f2de4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2de4-106">Properties</span></span>
| <span data-ttu-id="f2de4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2de4-107">Property</span></span>     | <span data-ttu-id="f2de4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f2de4-108">Type</span></span>        | <span data-ttu-id="f2de4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f2de4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f2de4-110">state</span><span class="sxs-lookup"><span data-stu-id="f2de4-110">state</span></span>|<span data-ttu-id="f2de4-111">принтоператионпроцессингстате</span><span class="sxs-lookup"><span data-stu-id="f2de4-111">printOperationProcessingState</span></span>|<span data-ttu-id="f2de4-112">Текущее состояние обработки Принтоператион.</span><span class="sxs-lookup"><span data-stu-id="f2de4-112">The printOperation's current processing state.</span></span> <span data-ttu-id="f2de4-113">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="f2de4-113">Valid values are described in the following table.</span></span> <span data-ttu-id="f2de4-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2de4-114">Read-only.</span></span>|
|<span data-ttu-id="f2de4-115">description</span><span class="sxs-lookup"><span data-stu-id="f2de4-115">description</span></span>|<span data-ttu-id="f2de4-116">String</span><span class="sxs-lookup"><span data-stu-id="f2de4-116">String</span></span>|<span data-ttu-id="f2de4-117">Удобное для человека описание текущего состояния обработки Принтоператион.</span><span class="sxs-lookup"><span data-stu-id="f2de4-117">A human-readable description of the printOperation's current processing state.</span></span> <span data-ttu-id="f2de4-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2de4-118">Read-only.</span></span>|

### <a name="printoperationprocessingstate-values"></a><span data-ttu-id="f2de4-119">значения Принтоператионпроцессингстате</span><span class="sxs-lookup"><span data-stu-id="f2de4-119">printOperationProcessingState values</span></span>

|<span data-ttu-id="f2de4-120">Элемент</span><span class="sxs-lookup"><span data-stu-id="f2de4-120">Member</span></span>|<span data-ttu-id="f2de4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f2de4-121">Value</span></span>|<span data-ttu-id="f2de4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f2de4-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2de4-123">notStarted</span><span class="sxs-lookup"><span data-stu-id="f2de4-123">notStarted</span></span>|<span data-ttu-id="f2de4-124">нуль</span><span class="sxs-lookup"><span data-stu-id="f2de4-124">0</span></span>|<span data-ttu-id="f2de4-125">Операция еще не запущена.</span><span class="sxs-lookup"><span data-stu-id="f2de4-125">The operation has not yet started.</span></span>|
|<span data-ttu-id="f2de4-126">запускается</span><span class="sxs-lookup"><span data-stu-id="f2de4-126">running</span></span>|<span data-ttu-id="f2de4-127">1 </span><span class="sxs-lookup"><span data-stu-id="f2de4-127">1</span></span>|<span data-ttu-id="f2de4-128">Выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="f2de4-128">The operation is running.</span></span>|
|<span data-ttu-id="f2de4-129">закончил</span><span class="sxs-lookup"><span data-stu-id="f2de4-129">succeeded</span></span>|<span data-ttu-id="f2de4-130">2 </span><span class="sxs-lookup"><span data-stu-id="f2de4-130">2</span></span>|<span data-ttu-id="f2de4-131">Операция успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="f2de4-131">The operation completed successfully.</span></span>|
|<span data-ttu-id="f2de4-132">сбоев</span><span class="sxs-lookup"><span data-stu-id="f2de4-132">failed</span></span>|<span data-ttu-id="f2de4-133">4</span><span class="sxs-lookup"><span data-stu-id="f2de4-133">3</span></span>|<span data-ttu-id="f2de4-134">Сбой операции.</span><span class="sxs-lookup"><span data-stu-id="f2de4-134">The operation failed.</span></span>|
|<span data-ttu-id="f2de4-135">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="f2de4-135">unknownFutureValue</span></span>|<span data-ttu-id="f2de4-136">4 </span><span class="sxs-lookup"><span data-stu-id="f2de4-136">4</span></span>|<span data-ttu-id="f2de4-137">Значение Sentinel для перечисления расширяемые.</span><span class="sxs-lookup"><span data-stu-id="f2de4-137">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="f2de4-138">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="f2de4-138">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2de4-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f2de4-139">JSON representation</span></span>

<span data-ttu-id="f2de4-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2de4-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperationStatus"
}-->

```json
{
    "state": "String",
    "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

