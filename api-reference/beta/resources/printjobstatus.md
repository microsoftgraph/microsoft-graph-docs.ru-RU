---
title: Тип ресурса Принтжобстатус
description: Представляет текущее состояние задания печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 1973d00ff8ca544f0acd1992626de9a3eaf59700
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895999"
---
# <a name="printjobstatus-resource-type"></a><span data-ttu-id="87b78-103">Тип ресурса Принтжобстатус</span><span class="sxs-lookup"><span data-stu-id="87b78-103">printJobStatus resource type</span></span>

<span data-ttu-id="87b78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87b78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87b78-105">Представляет текущее состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="87b78-105">Represents the current status of a print job.</span></span>

## <a name="properties"></a><span data-ttu-id="87b78-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="87b78-106">Properties</span></span>
| <span data-ttu-id="87b78-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="87b78-107">Property</span></span>     | <span data-ttu-id="87b78-108">Тип</span><span class="sxs-lookup"><span data-stu-id="87b78-108">Type</span></span>        | <span data-ttu-id="87b78-109">Описание</span><span class="sxs-lookup"><span data-stu-id="87b78-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87b78-110">процессингстате</span><span class="sxs-lookup"><span data-stu-id="87b78-110">processingState</span></span>|<span data-ttu-id="87b78-111">принтжобпроцессингстате</span><span class="sxs-lookup"><span data-stu-id="87b78-111">printJobProcessingState</span></span>|<span data-ttu-id="87b78-112">Текущее состояние обработки задания печати.</span><span class="sxs-lookup"><span data-stu-id="87b78-112">The print job's current processing state.</span></span> <span data-ttu-id="87b78-113">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="87b78-113">Valid values are described in the following table.</span></span> <span data-ttu-id="87b78-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87b78-114">Read-only.</span></span>|
|<span data-ttu-id="87b78-115">процессингстатедескриптион</span><span class="sxs-lookup"><span data-stu-id="87b78-115">processingStateDescription</span></span>|<span data-ttu-id="87b78-116">String</span><span class="sxs-lookup"><span data-stu-id="87b78-116">String</span></span>|<span data-ttu-id="87b78-117">Удобное для человека описание текущего состояния обработки задания печати.</span><span class="sxs-lookup"><span data-stu-id="87b78-117">A human-readable description of the print job's current processing state.</span></span> <span data-ttu-id="87b78-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87b78-118">Read-only.</span></span>|
|<span data-ttu-id="87b78-119">аккуиредбипринтер</span><span class="sxs-lookup"><span data-stu-id="87b78-119">acquiredByPrinter</span></span>|<span data-ttu-id="87b78-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="87b78-120">Boolean</span></span>|<span data-ttu-id="87b78-121">Значение true, если задание было подтверждено принтером; в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="87b78-121">True if the job was acknowledged by a printer; false otherwise.</span></span> <span data-ttu-id="87b78-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87b78-122">Read-only.</span></span>|

### <a name="printjobprocessingstate-values"></a><span data-ttu-id="87b78-123">значения Принтжобпроцессингстате</span><span class="sxs-lookup"><span data-stu-id="87b78-123">printJobProcessingState values</span></span>

|<span data-ttu-id="87b78-124">Элемент</span><span class="sxs-lookup"><span data-stu-id="87b78-124">Member</span></span>|<span data-ttu-id="87b78-125">Значение</span><span class="sxs-lookup"><span data-stu-id="87b78-125">Value</span></span>|<span data-ttu-id="87b78-126">Описание</span><span class="sxs-lookup"><span data-stu-id="87b78-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87b78-127">unknown</span><span class="sxs-lookup"><span data-stu-id="87b78-127">unknown</span></span>|<span data-ttu-id="87b78-128">нуль</span><span class="sxs-lookup"><span data-stu-id="87b78-128">0</span></span>|<span data-ttu-id="87b78-129">Состояние обработки, сообщаемое принтером, не распознано.</span><span class="sxs-lookup"><span data-stu-id="87b78-129">The processing state reported by the printer is not recognized.</span></span>|
|<span data-ttu-id="87b78-130">закончен</span><span class="sxs-lookup"><span data-stu-id="87b78-130">pending</span></span>|<span data-ttu-id="87b78-131">1,1</span><span class="sxs-lookup"><span data-stu-id="87b78-131">1</span></span>|<span data-ttu-id="87b78-132">Задание печати ожидает обработки принтером.</span><span class="sxs-lookup"><span data-stu-id="87b78-132">The print job is pending processing by the printer.</span></span>|
|<span data-ttu-id="87b78-133">пендингхелд</span><span class="sxs-lookup"><span data-stu-id="87b78-133">pendingHeld</span></span>|<span data-ttu-id="87b78-134">2</span><span class="sxs-lookup"><span data-stu-id="87b78-134">2</span></span>|<span data-ttu-id="87b78-135">Задание еще не является кандидатом на обработку.</span><span class="sxs-lookup"><span data-stu-id="87b78-135">The job is not a candidate for processing yet.</span></span> <span data-ttu-id="87b78-136">Убедитесь в отсутствии ошибок или ограничений ресурсов, препятствующих запуску задания.</span><span class="sxs-lookup"><span data-stu-id="87b78-136">Ensure that there are no errors or resource limitations preventing the job from starting.</span></span>|
|<span data-ttu-id="87b78-137">двухпроцессорной</span><span class="sxs-lookup"><span data-stu-id="87b78-137">processing</span></span>|<span data-ttu-id="87b78-138">4</span><span class="sxs-lookup"><span data-stu-id="87b78-138">3</span></span>|<span data-ttu-id="87b78-139">Задание печати в настоящее время обрабатывается принтером.</span><span class="sxs-lookup"><span data-stu-id="87b78-139">The print job is currently being processed by the printer.</span></span>|
|<span data-ttu-id="87b78-140">приостановлено</span><span class="sxs-lookup"><span data-stu-id="87b78-140">paused</span></span>|<span data-ttu-id="87b78-141">4 </span><span class="sxs-lookup"><span data-stu-id="87b78-141">4</span></span>|<span data-ttu-id="87b78-142">Задание печати приостановлено пользователем.</span><span class="sxs-lookup"><span data-stu-id="87b78-142">The print job has been paused by a user.</span></span>|
|<span data-ttu-id="87b78-143">отключен</span><span class="sxs-lookup"><span data-stu-id="87b78-143">stopped</span></span>|<span data-ttu-id="87b78-144">5 </span><span class="sxs-lookup"><span data-stu-id="87b78-144">5</span></span>|<span data-ttu-id="87b78-145">Задание печати остановлено, так как перед продолжением выполнения задания необходимо устранить проблемы с принтером.</span><span class="sxs-lookup"><span data-stu-id="87b78-145">The print job has been stopped because an issue with the printer needs to be addressed before the job can continue.</span></span> <span data-ttu-id="87b78-146">Дополнительные сведения можно найти в ресурсе "состояние принтера".</span><span class="sxs-lookup"><span data-stu-id="87b78-146">More information can be found in the printer state resource.</span></span>|
|<span data-ttu-id="87b78-147">готовы</span><span class="sxs-lookup"><span data-stu-id="87b78-147">completed</span></span>|<span data-ttu-id="87b78-148">6 </span><span class="sxs-lookup"><span data-stu-id="87b78-148">6</span></span>|<span data-ttu-id="87b78-149">Задание печати успешно завершено, дальнейшая обработка выполняться не будет.</span><span class="sxs-lookup"><span data-stu-id="87b78-149">The print job has completed successfully and no further processing will take place.</span></span>|
|<span data-ttu-id="87b78-150">закрыт</span><span class="sxs-lookup"><span data-stu-id="87b78-150">canceled</span></span>|<span data-ttu-id="87b78-151">7 </span><span class="sxs-lookup"><span data-stu-id="87b78-151">7</span></span>|<span data-ttu-id="87b78-152">Задание печати отменено пользователем, дальнейшая обработка не будет выполнена.</span><span class="sxs-lookup"><span data-stu-id="87b78-152">The print job has been canceled by a user and no further processing will take place.</span></span>|
|<span data-ttu-id="87b78-153">прерван</span><span class="sxs-lookup"><span data-stu-id="87b78-153">aborted</span></span>|<span data-ttu-id="87b78-154">8 </span><span class="sxs-lookup"><span data-stu-id="87b78-154">8</span></span>|<span data-ttu-id="87b78-155">Задание печати было прервано пользователем или принтером, и дальнейшая обработка не будет выполнена.</span><span class="sxs-lookup"><span data-stu-id="87b78-155">The print job has been aborted by a user or the printer and no further processing will take place.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87b78-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87b78-156">JSON representation</span></span>

<span data-ttu-id="87b78-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87b78-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobStatus"
}-->

```json
{
    "processingState": "String",
    "processingStateDescription": "String",
    "acquiredByPrinter": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJobStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->