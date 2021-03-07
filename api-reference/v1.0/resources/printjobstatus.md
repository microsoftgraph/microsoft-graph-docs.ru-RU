---
title: тип ресурса printJobStatus
description: Представляет текущее состояние задания печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7a6f5e0c728c1de122f9b642b9de2f1db050cf09
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518061"
---
# <a name="printjobstatus-resource-type"></a><span data-ttu-id="772f7-103">тип ресурса printJobStatus</span><span class="sxs-lookup"><span data-stu-id="772f7-103">printJobStatus resource type</span></span>

<span data-ttu-id="772f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="772f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="772f7-105">Представляет текущее состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="772f7-105">Represents the current status of a print job.</span></span>

## <a name="properties"></a><span data-ttu-id="772f7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="772f7-106">Properties</span></span>
|<span data-ttu-id="772f7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="772f7-107">Property</span></span>|<span data-ttu-id="772f7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="772f7-108">Type</span></span>|<span data-ttu-id="772f7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="772f7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="772f7-110">state</span><span class="sxs-lookup"><span data-stu-id="772f7-110">state</span></span>|<span data-ttu-id="772f7-111">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="772f7-111">printJobProcessingState</span></span>|<span data-ttu-id="772f7-112">Текущее состояние обработки задания печати.</span><span class="sxs-lookup"><span data-stu-id="772f7-112">The print job's current processing state.</span></span> <span data-ttu-id="772f7-113">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="772f7-113">Valid values are described in the following table.</span></span> <span data-ttu-id="772f7-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="772f7-114">Read-only.</span></span>|
|<span data-ttu-id="772f7-115">details</span><span class="sxs-lookup"><span data-stu-id="772f7-115">details</span></span>|<span data-ttu-id="772f7-116">printJobProcessingDetail collection</span><span class="sxs-lookup"><span data-stu-id="772f7-116">printJobProcessingDetail collection</span></span>|<span data-ttu-id="772f7-117">Дополнительные сведения для состояния задания печати.</span><span class="sxs-lookup"><span data-stu-id="772f7-117">Additional details for print job state.</span></span> <span data-ttu-id="772f7-118">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="772f7-118">Valid values are described in the following table.</span></span> <span data-ttu-id="772f7-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="772f7-119">Read-only.</span></span>|
|<span data-ttu-id="772f7-120">description</span><span class="sxs-lookup"><span data-stu-id="772f7-120">description</span></span>|<span data-ttu-id="772f7-121">Строка</span><span class="sxs-lookup"><span data-stu-id="772f7-121">String</span></span>|<span data-ttu-id="772f7-122">Описание текущего состояния обработки задания печати, считываемым человеком.</span><span class="sxs-lookup"><span data-stu-id="772f7-122">A human-readable description of the print job's current processing state.</span></span> <span data-ttu-id="772f7-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="772f7-123">Read-only.</span></span>|
|<span data-ttu-id="772f7-124">isAcquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="772f7-124">isAcquiredByPrinter</span></span>|<span data-ttu-id="772f7-125">Логический</span><span class="sxs-lookup"><span data-stu-id="772f7-125">Boolean</span></span>|<span data-ttu-id="772f7-126">True, если задание было признано принтером; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="772f7-126">True if the job was acknowledged by a printer; false otherwise.</span></span> <span data-ttu-id="772f7-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="772f7-127">Read-only.</span></span>|

### <a name="printjobprocessingstate-values"></a><span data-ttu-id="772f7-128">printJobProcessingState values</span><span class="sxs-lookup"><span data-stu-id="772f7-128">printJobProcessingState values</span></span>

|<span data-ttu-id="772f7-129">Элемент</span><span class="sxs-lookup"><span data-stu-id="772f7-129">Member</span></span>|<span data-ttu-id="772f7-130">Значение</span><span class="sxs-lookup"><span data-stu-id="772f7-130">Value</span></span>|<span data-ttu-id="772f7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="772f7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="772f7-132">unknown</span><span class="sxs-lookup"><span data-stu-id="772f7-132">unknown</span></span>|<span data-ttu-id="772f7-133">0</span><span class="sxs-lookup"><span data-stu-id="772f7-133">0</span></span>|<span data-ttu-id="772f7-134">Состояние обработки, о чем сообщает принтер, не распознается.</span><span class="sxs-lookup"><span data-stu-id="772f7-134">The processing state reported by the printer is not recognized.</span></span>|
|<span data-ttu-id="772f7-135">ожидание</span><span class="sxs-lookup"><span data-stu-id="772f7-135">pending</span></span>|<span data-ttu-id="772f7-136">1 </span><span class="sxs-lookup"><span data-stu-id="772f7-136">1</span></span>|<span data-ttu-id="772f7-137">Задание печати находится в ожидании обработки принтером.</span><span class="sxs-lookup"><span data-stu-id="772f7-137">The print job is pending processing by the printer.</span></span>|
|<span data-ttu-id="772f7-138">обработка</span><span class="sxs-lookup"><span data-stu-id="772f7-138">processing</span></span>|<span data-ttu-id="772f7-139">2 </span><span class="sxs-lookup"><span data-stu-id="772f7-139">2</span></span>|<span data-ttu-id="772f7-140">Задание печати в настоящее время обрабатывается принтером.</span><span class="sxs-lookup"><span data-stu-id="772f7-140">The print job is currently being processed by the printer.</span></span>|
|<span data-ttu-id="772f7-141">приостановлено</span><span class="sxs-lookup"><span data-stu-id="772f7-141">paused</span></span>|<span data-ttu-id="772f7-142">3 </span><span class="sxs-lookup"><span data-stu-id="772f7-142">3</span></span>|<span data-ttu-id="772f7-143">Задание печати приостановлено.</span><span class="sxs-lookup"><span data-stu-id="772f7-143">The print job has been paused.</span></span>|
|<span data-ttu-id="772f7-144">остановлено</span><span class="sxs-lookup"><span data-stu-id="772f7-144">stopped</span></span>|<span data-ttu-id="772f7-145">4 </span><span class="sxs-lookup"><span data-stu-id="772f7-145">4</span></span>|<span data-ttu-id="772f7-146">Задание печати было остановлено, так как перед продолжением работы необходимо устранить проблему с принтером.</span><span class="sxs-lookup"><span data-stu-id="772f7-146">The print job has been stopped because an issue with the printer needs to be addressed before the job can continue.</span></span> <span data-ttu-id="772f7-147">Дополнительные сведения можно найти на ресурсе состояния принтера.</span><span class="sxs-lookup"><span data-stu-id="772f7-147">More information can be found in the printer state resource.</span></span>|
|<span data-ttu-id="772f7-148">завершено</span><span class="sxs-lookup"><span data-stu-id="772f7-148">completed</span></span>|<span data-ttu-id="772f7-149">5 </span><span class="sxs-lookup"><span data-stu-id="772f7-149">5</span></span>|<span data-ttu-id="772f7-150">Задание печати выполнено успешно, и дальнейшая обработка не будет выполнена.</span><span class="sxs-lookup"><span data-stu-id="772f7-150">The print job has completed successfully and no further processing will take place.</span></span>|
|<span data-ttu-id="772f7-151">отменено</span><span class="sxs-lookup"><span data-stu-id="772f7-151">canceled</span></span>|<span data-ttu-id="772f7-152">6 </span><span class="sxs-lookup"><span data-stu-id="772f7-152">6</span></span>|<span data-ttu-id="772f7-153">Задание печати было отменено пользователем, и дальнейшая обработка не будет происходить.</span><span class="sxs-lookup"><span data-stu-id="772f7-153">The print job has been canceled by a user and no further processing will take place.</span></span>|
|<span data-ttu-id="772f7-154">прервано</span><span class="sxs-lookup"><span data-stu-id="772f7-154">aborted</span></span>|<span data-ttu-id="772f7-155">7 </span><span class="sxs-lookup"><span data-stu-id="772f7-155">7</span></span>|<span data-ttu-id="772f7-156">Задание печати было прервано пользователем или принтером, и дальнейшая обработка не будет происходить.</span><span class="sxs-lookup"><span data-stu-id="772f7-156">The print job has been aborted by a user or the printer and no further processing will take place.</span></span>|

### <a name="printjobprocessingdetail-values"></a><span data-ttu-id="772f7-157">printJobProcessingDetail values</span><span class="sxs-lookup"><span data-stu-id="772f7-157">printJobProcessingDetail values</span></span>

|<span data-ttu-id="772f7-158">Элемент</span><span class="sxs-lookup"><span data-stu-id="772f7-158">Member</span></span>|<span data-ttu-id="772f7-159">Значение</span><span class="sxs-lookup"><span data-stu-id="772f7-159">Value</span></span>|<span data-ttu-id="772f7-160">Описание</span><span class="sxs-lookup"><span data-stu-id="772f7-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="772f7-161">uploadPending</span><span class="sxs-lookup"><span data-stu-id="772f7-161">uploadPending</span></span>|<span data-ttu-id="772f7-162">0</span><span class="sxs-lookup"><span data-stu-id="772f7-162">0</span></span>|<span data-ttu-id="772f7-163">Загрузка полезной нагрузки документа не была.</span><span class="sxs-lookup"><span data-stu-id="772f7-163">Document payload has not been uploaded.</span></span>|
|<span data-ttu-id="772f7-164">преобразование</span><span class="sxs-lookup"><span data-stu-id="772f7-164">transforming</span></span>|<span data-ttu-id="772f7-165">1 </span><span class="sxs-lookup"><span data-stu-id="772f7-165">1</span></span>|<span data-ttu-id="772f7-166">Преобразование полезной нагрузки документа.</span><span class="sxs-lookup"><span data-stu-id="772f7-166">Document payload is being transformed.</span></span>|
|<span data-ttu-id="772f7-167">completedSuccessfully</span><span class="sxs-lookup"><span data-stu-id="772f7-167">completedSuccessfully</span></span>|<span data-ttu-id="772f7-168">2 </span><span class="sxs-lookup"><span data-stu-id="772f7-168">2</span></span>|<span data-ttu-id="772f7-169">Задание выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="772f7-169">Job has been completed successfully.</span></span>|
|<span data-ttu-id="772f7-170">completedWithWarnings</span><span class="sxs-lookup"><span data-stu-id="772f7-170">completedWithWarnings</span></span>|<span data-ttu-id="772f7-171">3 </span><span class="sxs-lookup"><span data-stu-id="772f7-171">3</span></span>|<span data-ttu-id="772f7-172">Задание выполнено с помощью предупреждений.</span><span class="sxs-lookup"><span data-stu-id="772f7-172">Job has been completed with warnings.</span></span>|
|<span data-ttu-id="772f7-173">completedWithErrors</span><span class="sxs-lookup"><span data-stu-id="772f7-173">completedWithErrors</span></span>|<span data-ttu-id="772f7-174">4 </span><span class="sxs-lookup"><span data-stu-id="772f7-174">4</span></span>|<span data-ttu-id="772f7-175">Задание выполнено с ошибками.</span><span class="sxs-lookup"><span data-stu-id="772f7-175">Job has been completed with errors.</span></span>|
|<span data-ttu-id="772f7-176">releaseWait</span><span class="sxs-lookup"><span data-stu-id="772f7-176">releaseWait</span></span>|<span data-ttu-id="772f7-177">5 </span><span class="sxs-lookup"><span data-stu-id="772f7-177">5</span></span>|<span data-ttu-id="772f7-178">Ожидается, что задание будет выпущено.</span><span class="sxs-lookup"><span data-stu-id="772f7-178">Job is pending to be released.</span></span>|
|<span data-ttu-id="772f7-179">интерпретация</span><span class="sxs-lookup"><span data-stu-id="772f7-179">interpreting</span></span>|<span data-ttu-id="772f7-180">6 </span><span class="sxs-lookup"><span data-stu-id="772f7-180">6</span></span>|<span data-ttu-id="772f7-181">Задание находится в состоянии "обработка", но, более конкретно, документ полезной нагрузки в настоящее время интерпретируется.</span><span class="sxs-lookup"><span data-stu-id="772f7-181">Job is in 'processing' state, but more specifically, document payload is being interpreted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="772f7-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="772f7-182">JSON representation</span></span>
<span data-ttu-id="772f7-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="772f7-183">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobStatus",
  "state": "String",
  "description": "String",
  "isAcquiredByPrinter": "Boolean",
  "details": [
    "String"
  ]
}
```

