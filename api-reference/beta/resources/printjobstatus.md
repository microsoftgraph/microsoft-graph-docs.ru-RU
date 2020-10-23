---
title: Тип ресурса Принтжобстатус
description: Представляет текущее состояние задания печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bb3221eb12946d58664211731a31993e540aaf00
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728946"
---
# <a name="printjobstatus-resource-type"></a><span data-ttu-id="b35ac-103">Тип ресурса Принтжобстатус</span><span class="sxs-lookup"><span data-stu-id="b35ac-103">printJobStatus resource type</span></span>

<span data-ttu-id="b35ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b35ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b35ac-105">Представляет текущее состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="b35ac-105">Represents the current status of a print job.</span></span>

## <a name="properties"></a><span data-ttu-id="b35ac-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b35ac-106">Properties</span></span>
| <span data-ttu-id="b35ac-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b35ac-107">Property</span></span>     | <span data-ttu-id="b35ac-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b35ac-108">Type</span></span>        | <span data-ttu-id="b35ac-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b35ac-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b35ac-110">state</span><span class="sxs-lookup"><span data-stu-id="b35ac-110">state</span></span>|<span data-ttu-id="b35ac-111">принтжобпроцессингстате</span><span class="sxs-lookup"><span data-stu-id="b35ac-111">printJobProcessingState</span></span>|<span data-ttu-id="b35ac-112">Текущее состояние обработки задания печати.</span><span class="sxs-lookup"><span data-stu-id="b35ac-112">The print job's current processing state.</span></span> <span data-ttu-id="b35ac-113">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="b35ac-113">Valid values are described in the following table.</span></span> <span data-ttu-id="b35ac-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b35ac-114">Read-only.</span></span>|
|<span data-ttu-id="b35ac-115">details</span><span class="sxs-lookup"><span data-stu-id="b35ac-115">details</span></span>|<span data-ttu-id="b35ac-116">Коллекция Принтжобпроцессингдетаил</span><span class="sxs-lookup"><span data-stu-id="b35ac-116">printJobProcessingDetail collection</span></span>|<span data-ttu-id="b35ac-117">Дополнительные сведения о состоянии задания печати.</span><span class="sxs-lookup"><span data-stu-id="b35ac-117">Additional details for print job state.</span></span> <span data-ttu-id="b35ac-118">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="b35ac-118">Valid values are described in the following table.</span></span> <span data-ttu-id="b35ac-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b35ac-119">Read-only.</span></span>|
|<span data-ttu-id="b35ac-120">description</span><span class="sxs-lookup"><span data-stu-id="b35ac-120">description</span></span>|<span data-ttu-id="b35ac-121">Строка</span><span class="sxs-lookup"><span data-stu-id="b35ac-121">String</span></span>|<span data-ttu-id="b35ac-122">Удобное для человека описание текущего состояния обработки задания печати.</span><span class="sxs-lookup"><span data-stu-id="b35ac-122">A human-readable description of the print job's current processing state.</span></span> <span data-ttu-id="b35ac-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b35ac-123">Read-only.</span></span>|
|<span data-ttu-id="b35ac-124">исаккуиредбипринтер</span><span class="sxs-lookup"><span data-stu-id="b35ac-124">isAcquiredByPrinter</span></span>|<span data-ttu-id="b35ac-125">Логический</span><span class="sxs-lookup"><span data-stu-id="b35ac-125">Boolean</span></span>|<span data-ttu-id="b35ac-126">Значение true, если задание было подтверждено принтером; в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="b35ac-126">True if the job was acknowledged by a printer; false otherwise.</span></span> <span data-ttu-id="b35ac-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b35ac-127">Read-only.</span></span>|

### <a name="printjobprocessingstate-values"></a><span data-ttu-id="b35ac-128">значения Принтжобпроцессингстате</span><span class="sxs-lookup"><span data-stu-id="b35ac-128">printJobProcessingState values</span></span>

|<span data-ttu-id="b35ac-129">Элемент</span><span class="sxs-lookup"><span data-stu-id="b35ac-129">Member</span></span>|<span data-ttu-id="b35ac-130">Значение</span><span class="sxs-lookup"><span data-stu-id="b35ac-130">Value</span></span>|<span data-ttu-id="b35ac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b35ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b35ac-132">unknown</span><span class="sxs-lookup"><span data-stu-id="b35ac-132">unknown</span></span>|<span data-ttu-id="b35ac-133">нуль</span><span class="sxs-lookup"><span data-stu-id="b35ac-133">0</span></span>|<span data-ttu-id="b35ac-134">Состояние обработки, сообщаемое принтером, не распознано.</span><span class="sxs-lookup"><span data-stu-id="b35ac-134">The processing state reported by the printer is not recognized.</span></span>|
|<span data-ttu-id="b35ac-135">закончен</span><span class="sxs-lookup"><span data-stu-id="b35ac-135">pending</span></span>|<span data-ttu-id="b35ac-136">1,1</span><span class="sxs-lookup"><span data-stu-id="b35ac-136">1</span></span>|<span data-ttu-id="b35ac-137">Задание печати ожидает обработки принтером.</span><span class="sxs-lookup"><span data-stu-id="b35ac-137">The print job is pending processing by the printer.</span></span>|
|<span data-ttu-id="b35ac-138">двухпроцессорной</span><span class="sxs-lookup"><span data-stu-id="b35ac-138">processing</span></span>|<span data-ttu-id="b35ac-139">2</span><span class="sxs-lookup"><span data-stu-id="b35ac-139">2</span></span>|<span data-ttu-id="b35ac-140">Задание печати в настоящее время обрабатывается принтером.</span><span class="sxs-lookup"><span data-stu-id="b35ac-140">The print job is currently being processed by the printer.</span></span>|
|<span data-ttu-id="b35ac-141">приостановлено</span><span class="sxs-lookup"><span data-stu-id="b35ac-141">paused</span></span>|<span data-ttu-id="b35ac-142">4</span><span class="sxs-lookup"><span data-stu-id="b35ac-142">3</span></span>|<span data-ttu-id="b35ac-143">Задание печати приостановлено.</span><span class="sxs-lookup"><span data-stu-id="b35ac-143">The print job has been paused.</span></span>|
|<span data-ttu-id="b35ac-144">отключен</span><span class="sxs-lookup"><span data-stu-id="b35ac-144">stopped</span></span>|<span data-ttu-id="b35ac-145">4 </span><span class="sxs-lookup"><span data-stu-id="b35ac-145">4</span></span>|<span data-ttu-id="b35ac-146">Задание печати остановлено, так как перед продолжением выполнения задания необходимо устранить проблемы с принтером.</span><span class="sxs-lookup"><span data-stu-id="b35ac-146">The print job has been stopped because an issue with the printer needs to be addressed before the job can continue.</span></span> <span data-ttu-id="b35ac-147">Дополнительные сведения можно найти в ресурсе "состояние принтера".</span><span class="sxs-lookup"><span data-stu-id="b35ac-147">More information can be found in the printer state resource.</span></span>|
|<span data-ttu-id="b35ac-148">готовы</span><span class="sxs-lookup"><span data-stu-id="b35ac-148">completed</span></span>|<span data-ttu-id="b35ac-149">5 </span><span class="sxs-lookup"><span data-stu-id="b35ac-149">5</span></span>|<span data-ttu-id="b35ac-150">Задание печати успешно завершено, дальнейшая обработка выполняться не будет.</span><span class="sxs-lookup"><span data-stu-id="b35ac-150">The print job has completed successfully and no further processing will take place.</span></span>|
|<span data-ttu-id="b35ac-151">закрыт</span><span class="sxs-lookup"><span data-stu-id="b35ac-151">canceled</span></span>|<span data-ttu-id="b35ac-152">6 </span><span class="sxs-lookup"><span data-stu-id="b35ac-152">6</span></span>|<span data-ttu-id="b35ac-153">Задание печати отменено пользователем, дальнейшая обработка не будет выполнена.</span><span class="sxs-lookup"><span data-stu-id="b35ac-153">The print job has been canceled by a user and no further processing will take place.</span></span>|
|<span data-ttu-id="b35ac-154">прерван</span><span class="sxs-lookup"><span data-stu-id="b35ac-154">aborted</span></span>|<span data-ttu-id="b35ac-155">7 </span><span class="sxs-lookup"><span data-stu-id="b35ac-155">7</span></span>|<span data-ttu-id="b35ac-156">Задание печати было прервано пользователем или принтером, и дальнейшая обработка не будет выполнена.</span><span class="sxs-lookup"><span data-stu-id="b35ac-156">The print job has been aborted by a user or the printer and no further processing will take place.</span></span>|

### <a name="printjobprocessingdetail-values"></a><span data-ttu-id="b35ac-157">значения Принтжобпроцессингдетаил</span><span class="sxs-lookup"><span data-stu-id="b35ac-157">printJobProcessingDetail values</span></span>

|<span data-ttu-id="b35ac-158">Элемент</span><span class="sxs-lookup"><span data-stu-id="b35ac-158">Member</span></span>|<span data-ttu-id="b35ac-159">Значение</span><span class="sxs-lookup"><span data-stu-id="b35ac-159">Value</span></span>|<span data-ttu-id="b35ac-160">Описание</span><span class="sxs-lookup"><span data-stu-id="b35ac-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b35ac-161">уплоадпендинг</span><span class="sxs-lookup"><span data-stu-id="b35ac-161">uploadPending</span></span>|<span data-ttu-id="b35ac-162">нуль</span><span class="sxs-lookup"><span data-stu-id="b35ac-162">0</span></span>|<span data-ttu-id="b35ac-163">Полезные данные документа не были отправлены.</span><span class="sxs-lookup"><span data-stu-id="b35ac-163">Document payload has not been uploaded.</span></span>|
|<span data-ttu-id="b35ac-164">Преобразование</span><span class="sxs-lookup"><span data-stu-id="b35ac-164">transforming</span></span>|<span data-ttu-id="b35ac-165">1,1</span><span class="sxs-lookup"><span data-stu-id="b35ac-165">1</span></span>|<span data-ttu-id="b35ac-166">Выполняется преобразование полезных данных документа.</span><span class="sxs-lookup"><span data-stu-id="b35ac-166">Document payload is being transformed.</span></span>|
|<span data-ttu-id="b35ac-167">комплетедсукцессфулли</span><span class="sxs-lookup"><span data-stu-id="b35ac-167">completedSuccessfully</span></span>|<span data-ttu-id="b35ac-168">2</span><span class="sxs-lookup"><span data-stu-id="b35ac-168">2</span></span>|<span data-ttu-id="b35ac-169">Задание успешно завершено.</span><span class="sxs-lookup"><span data-stu-id="b35ac-169">Job has been completed successfully.</span></span>|
|<span data-ttu-id="b35ac-170">комплетедвисварнингс</span><span class="sxs-lookup"><span data-stu-id="b35ac-170">completedWithWarnings</span></span>|<span data-ttu-id="b35ac-171">4</span><span class="sxs-lookup"><span data-stu-id="b35ac-171">3</span></span>|<span data-ttu-id="b35ac-172">Задание было завершено с предупреждениями.</span><span class="sxs-lookup"><span data-stu-id="b35ac-172">Job has been completed with warnings.</span></span>|
|<span data-ttu-id="b35ac-173">комплетедвисеррорс</span><span class="sxs-lookup"><span data-stu-id="b35ac-173">completedWithErrors</span></span>|<span data-ttu-id="b35ac-174">4 </span><span class="sxs-lookup"><span data-stu-id="b35ac-174">4</span></span>|<span data-ttu-id="b35ac-175">Задание выполнено с ошибками.</span><span class="sxs-lookup"><span data-stu-id="b35ac-175">Job has been completed with errors.</span></span>|
|<span data-ttu-id="b35ac-176">релеасеваит</span><span class="sxs-lookup"><span data-stu-id="b35ac-176">releaseWait</span></span>|<span data-ttu-id="b35ac-177">5 </span><span class="sxs-lookup"><span data-stu-id="b35ac-177">5</span></span>|<span data-ttu-id="b35ac-178">Ожидается выпуск задания.</span><span class="sxs-lookup"><span data-stu-id="b35ac-178">Job is pending to be released.</span></span>|
|<span data-ttu-id="b35ac-179">интерпретации</span><span class="sxs-lookup"><span data-stu-id="b35ac-179">interpreting</span></span>|<span data-ttu-id="b35ac-180">6 </span><span class="sxs-lookup"><span data-stu-id="b35ac-180">6</span></span>|<span data-ttu-id="b35ac-181">Задание находится в состоянии "обработка", но точнее, интерпретация полезных данных документа.</span><span class="sxs-lookup"><span data-stu-id="b35ac-181">Job is in 'processing' state, but more specifically, document payload is being interpreted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b35ac-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b35ac-182">JSON representation</span></span>

<span data-ttu-id="b35ac-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b35ac-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobStatus"
}-->

```json
{
    "state": "String",
    "description": "String",
    "isAcquiredByPrinter": true,    
    "details": ["String"]
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

