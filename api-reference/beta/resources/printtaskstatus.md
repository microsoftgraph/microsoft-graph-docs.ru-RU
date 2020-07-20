---
title: Тип ресурса Принттаскстатус
description: Представляет текущее состояние выполнения Принттаск.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c5d46cd0c8d14b6dc07873bc503d024928e2b2e3
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091702"
---
# <a name="printtaskstatus-resource-type"></a><span data-ttu-id="1cbb2-103">Тип ресурса Принттаскстатус</span><span class="sxs-lookup"><span data-stu-id="1cbb2-103">printTaskStatus resource type</span></span>

<span data-ttu-id="1cbb2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cbb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cbb2-105">Представляет текущее состояние выполнения [принттаск](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="1cbb2-105">Represents the current execution status of a [printTask](printtask.md).</span></span> 

><span data-ttu-id="1cbb2-106">**Примечание:** Приложения, которые регистрируют триггеры задач, несут ответственность за обновление состояния задач при завершении обработки, если соответствующее задание печати не было перенаправлено на другой принтер.</span><span class="sxs-lookup"><span data-stu-id="1cbb2-106">**Note:** Applications that register task triggers are responsible for updating task statuses when processing is finished, unless the related print job has been redirected to another printer.</span></span>

<span data-ttu-id="1cbb2-107">Дополнительные сведения о том, как использовать этот ресурс для поддержки печати по запросу в универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="1cbb2-107">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="properties"></a><span data-ttu-id="1cbb2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1cbb2-108">Properties</span></span>
| <span data-ttu-id="1cbb2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cbb2-109">Property</span></span>     | <span data-ttu-id="1cbb2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1cbb2-110">Type</span></span>        | <span data-ttu-id="1cbb2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1cbb2-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1cbb2-112">state</span><span class="sxs-lookup"><span data-stu-id="1cbb2-112">state</span></span>|<span data-ttu-id="1cbb2-113">принттаскпроцессингстате</span><span class="sxs-lookup"><span data-stu-id="1cbb2-113">printTaskProcessingState</span></span>|<span data-ttu-id="1cbb2-114">Текущее состояние обработки [принттаск](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="1cbb2-114">The current processing state of the [printTask](printtask.md).</span></span> <span data-ttu-id="1cbb2-115">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="1cbb2-115">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="1cbb2-116">description</span><span class="sxs-lookup"><span data-stu-id="1cbb2-116">description</span></span>|<span data-ttu-id="1cbb2-117">String</span><span class="sxs-lookup"><span data-stu-id="1cbb2-117">String</span></span>|<span data-ttu-id="1cbb2-118">Удобное для человека описание текущего состояния обработки [принттаск](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="1cbb2-118">A human-readable description of the current processing state of the [printTask](printtask.md).</span></span>|

### <a name="printtaskprocessingstate-values"></a><span data-ttu-id="1cbb2-119">значения Принттаскпроцессингстате</span><span class="sxs-lookup"><span data-stu-id="1cbb2-119">printTaskProcessingState values</span></span>

|<span data-ttu-id="1cbb2-120">Элемент</span><span class="sxs-lookup"><span data-stu-id="1cbb2-120">Member</span></span>|<span data-ttu-id="1cbb2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1cbb2-121">Value</span></span>|<span data-ttu-id="1cbb2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1cbb2-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cbb2-123">закончен</span><span class="sxs-lookup"><span data-stu-id="1cbb2-123">pending</span></span>|<span data-ttu-id="1cbb2-124">нуль</span><span class="sxs-lookup"><span data-stu-id="1cbb2-124">0</span></span>|<span data-ttu-id="1cbb2-125">Ожидание выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="1cbb2-125">Task execution is pending.</span></span>|
|<span data-ttu-id="1cbb2-126">двухпроцессорной</span><span class="sxs-lookup"><span data-stu-id="1cbb2-126">processing</span></span>|<span data-ttu-id="1cbb2-127">1 </span><span class="sxs-lookup"><span data-stu-id="1cbb2-127">1</span></span>|<span data-ttu-id="1cbb2-128">Выполняется выполнение задачи.</span><span class="sxs-lookup"><span data-stu-id="1cbb2-128">Task execution is in progress.</span></span>|
|<span data-ttu-id="1cbb2-129">готовы</span><span class="sxs-lookup"><span data-stu-id="1cbb2-129">completed</span></span>|<span data-ttu-id="1cbb2-130">2 </span><span class="sxs-lookup"><span data-stu-id="1cbb2-130">2</span></span>|<span data-ttu-id="1cbb2-131">Выполнение задачи завершено.</span><span class="sxs-lookup"><span data-stu-id="1cbb2-131">Task execution has completed.</span></span>|
|<span data-ttu-id="1cbb2-132">прерван</span><span class="sxs-lookup"><span data-stu-id="1cbb2-132">aborted</span></span>|<span data-ttu-id="1cbb2-133">3 </span><span class="sxs-lookup"><span data-stu-id="1cbb2-133">3</span></span>|<span data-ttu-id="1cbb2-134">Выполнение задачи было прервано.</span><span class="sxs-lookup"><span data-stu-id="1cbb2-134">Task execution was aborted.</span></span>|
|<span data-ttu-id="1cbb2-135">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="1cbb2-135">unknownFutureValue</span></span>|<span data-ttu-id="1cbb2-136">4 </span><span class="sxs-lookup"><span data-stu-id="1cbb2-136">4</span></span>|<span data-ttu-id="1cbb2-137">Значение Sentinel для перечисления расширяемые.</span><span class="sxs-lookup"><span data-stu-id="1cbb2-137">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="1cbb2-138">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="1cbb2-138">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1cbb2-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1cbb2-139">JSON representation</span></span>

<span data-ttu-id="1cbb2-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cbb2-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskStatus"
}-->

```json
{
  "state": {"@odata.type": "microsoft.graph.printTaskProcessingState"},
  "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
