---
title: тип ресурса archivedPrintJob
description: Запись задания печати "окончательное состояние" (завершено, прервано или не выполнено) для отчетов. Это не активная работа печати.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2132b5a7cdf5024fb13845c57844220594ba6e1f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517965"
---
# <a name="archivedprintjob-resource-type"></a><span data-ttu-id="e951a-104">тип ресурса archivedPrintJob</span><span class="sxs-lookup"><span data-stu-id="e951a-104">archivedPrintJob resource type</span></span>

<span data-ttu-id="e951a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e951a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e951a-106">Запись задания печати "окончательное состояние" (завершено, прервано или не выполнено) для отчетов.</span><span class="sxs-lookup"><span data-stu-id="e951a-106">A record of a "final state" (completed, aborted or failed) print job that is used for reporting purposes.</span></span> <span data-ttu-id="e951a-107">Это не активная работа печати.</span><span class="sxs-lookup"><span data-stu-id="e951a-107">This is not an active print job.</span></span>

## <a name="properties"></a><span data-ttu-id="e951a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e951a-108">Properties</span></span>
| <span data-ttu-id="e951a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e951a-109">Property</span></span>     | <span data-ttu-id="e951a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e951a-110">Type</span></span>        | <span data-ttu-id="e951a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e951a-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e951a-112">id</span><span class="sxs-lookup"><span data-stu-id="e951a-112">id</span></span>|<span data-ttu-id="e951a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e951a-113">String</span></span>|<span data-ttu-id="e951a-114">GUID архивного задания печати.</span><span class="sxs-lookup"><span data-stu-id="e951a-114">The archived print job's GUID.</span></span> <span data-ttu-id="e951a-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e951a-115">Read-only.</span></span>|
|<span data-ttu-id="e951a-116">printerId</span><span class="sxs-lookup"><span data-stu-id="e951a-116">printerId</span></span>|<span data-ttu-id="e951a-117">Строка</span><span class="sxs-lookup"><span data-stu-id="e951a-117">String</span></span>|<span data-ttu-id="e951a-118">ID принтера, для работы в очереди.</span><span class="sxs-lookup"><span data-stu-id="e951a-118">The printer ID that the job was queued for.</span></span> <span data-ttu-id="e951a-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e951a-119">Read-only.</span></span>|
|<span data-ttu-id="e951a-120">processingState</span><span class="sxs-lookup"><span data-stu-id="e951a-120">processingState</span></span>|<span data-ttu-id="e951a-121">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="e951a-121">printJobProcessingState</span></span>|<span data-ttu-id="e951a-122">Окончательное состояние обработки задания печати.</span><span class="sxs-lookup"><span data-stu-id="e951a-122">The print job's final processing state.</span></span> <span data-ttu-id="e951a-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e951a-123">Read-only.</span></span>|
|<span data-ttu-id="e951a-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e951a-124">createdDateTime</span></span>|<span data-ttu-id="e951a-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e951a-125">DateTimeOffset</span></span>|<span data-ttu-id="e951a-126">DateTimeOffset, когда было создано задание.</span><span class="sxs-lookup"><span data-stu-id="e951a-126">The dateTimeOffset when the job was created.</span></span> <span data-ttu-id="e951a-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e951a-127">Read-only.</span></span>|
|<span data-ttu-id="e951a-128">acquiredDateTime</span><span class="sxs-lookup"><span data-stu-id="e951a-128">acquiredDateTime</span></span>|<span data-ttu-id="e951a-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e951a-129">DateTimeOffset</span></span>|<span data-ttu-id="e951a-130">DateTimeOffset, когда задание было приобретено принтером, если таково.</span><span class="sxs-lookup"><span data-stu-id="e951a-130">The dateTimeOffset when the job was acquired by the printer, if any.</span></span> <span data-ttu-id="e951a-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e951a-131">Read-only.</span></span>|
|<span data-ttu-id="e951a-132">completionDateTime</span><span class="sxs-lookup"><span data-stu-id="e951a-132">completionDateTime</span></span>|<span data-ttu-id="e951a-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e951a-133">DateTimeOffset</span></span>|<span data-ttu-id="e951a-134">DateTimeOffset, когда задание было завершено, отменено или прервано.</span><span class="sxs-lookup"><span data-stu-id="e951a-134">The dateTimeOffset when the job was completed, canceled or aborted.</span></span> <span data-ttu-id="e951a-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e951a-135">Read-only.</span></span>|
|<span data-ttu-id="e951a-136">acquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="e951a-136">acquiredByPrinter</span></span>|<span data-ttu-id="e951a-137">Логический</span><span class="sxs-lookup"><span data-stu-id="e951a-137">Boolean</span></span>|<span data-ttu-id="e951a-138">True, если задание было приобретено принтером; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="e951a-138">True if the job was acquired by a printer; false otherwise.</span></span> <span data-ttu-id="e951a-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e951a-139">Read-only.</span></span>|
|<span data-ttu-id="e951a-140">copiesPrinted</span><span class="sxs-lookup"><span data-stu-id="e951a-140">copiesPrinted</span></span>|<span data-ttu-id="e951a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e951a-141">Int32</span></span>|<span data-ttu-id="e951a-142">Количество напечатанных копий.</span><span class="sxs-lookup"><span data-stu-id="e951a-142">The number of copies that were printed.</span></span> <span data-ttu-id="e951a-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e951a-143">Read-only.</span></span>|
|<span data-ttu-id="e951a-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="e951a-144">createdBy</span></span>|[<span data-ttu-id="e951a-145">userIdentity</span><span class="sxs-lookup"><span data-stu-id="e951a-145">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="e951a-146">Пользователь, создавший задание печати.</span><span class="sxs-lookup"><span data-stu-id="e951a-146">The user who created the print job.</span></span> <span data-ttu-id="e951a-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e951a-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e951a-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e951a-148">JSON representation</span></span>

<span data-ttu-id="e951a-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e951a-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.archivedPrintJob"
}-->
```json
    {   
  "@odata.type": "#microsoft.graph.archivedPrintJob",   
  "id": "String (identifier)",  
  "printerId": "String",    
  "processingState": "String",  
  "createdDateTime": "String (timestamp)",  
  "acquiredDateTime": "String (timestamp)", 
  "completionDateTime": "String (timestamp)",   
  "acquiredByPrinter": "Boolean",   
  "copiesPrinted": "Integer",   
  "createdBy": {    
    "@odata.type": "microsoft.graph.userIdentity"   
  } 
}
```