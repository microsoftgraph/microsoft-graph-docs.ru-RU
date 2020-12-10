---
title: Тип ресурса Printer
description: Представляет физическое устройство печати, зарегистрированное в универсальной службе печати. Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5833dc1f37620a419153100ebf9ce6d7f141fa5d
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617012"
---
# <a name="printer-resource-type"></a><span data-ttu-id="1762e-104">Тип ресурса Printer</span><span class="sxs-lookup"><span data-stu-id="1762e-104">printer resource type</span></span>

<span data-ttu-id="1762e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1762e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1762e-106">Представляет устройство принтера, зарегистрированное в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="1762e-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="1762e-107">Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.</span><span class="sxs-lookup"><span data-stu-id="1762e-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="1762e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1762e-108">Methods</span></span>

| <span data-ttu-id="1762e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1762e-109">Method</span></span>       | <span data-ttu-id="1762e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1762e-110">Return Type</span></span> | <span data-ttu-id="1762e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1762e-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1762e-112">Создание</span><span class="sxs-lookup"><span data-stu-id="1762e-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="1762e-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="1762e-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="1762e-114">Создание (регистрация) нового принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="1762e-114">Create (register) a new printer with Universal Print.</span></span> |
| <span data-ttu-id="1762e-115">[получение](../api/printer-get.md);</span><span class="sxs-lookup"><span data-stu-id="1762e-115">[Get](../api/printer-get.md)</span></span> | [<span data-ttu-id="1762e-116">Printer</span><span class="sxs-lookup"><span data-stu-id="1762e-116">printer</span></span>](printer.md) | <span data-ttu-id="1762e-117">Чтение свойств и связей объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="1762e-117">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="1762e-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="1762e-118">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="1762e-119">Printer</span><span class="sxs-lookup"><span data-stu-id="1762e-119">printer</span></span>](printer.md) | <span data-ttu-id="1762e-120">Обновление объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="1762e-120">Update the printer object.</span></span> |
| [<span data-ttu-id="1762e-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="1762e-121">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="1762e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="1762e-122">None</span></span> | <span data-ttu-id="1762e-123">Отмените регистрацию физического принтера в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="1762e-123">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="1762e-124">ресторефакторидефаултс</span><span class="sxs-lookup"><span data-stu-id="1762e-124">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="1762e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="1762e-125">None</span></span> | <span data-ttu-id="1762e-126">Восстановите параметры принтера по умолчанию на значения, заданные производителем.</span><span class="sxs-lookup"><span data-stu-id="1762e-126">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="1762e-127">Список заданий</span><span class="sxs-lookup"><span data-stu-id="1762e-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="1762e-128">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="1762e-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="1762e-129">Получение списка заданий печати, помещенных в очередь для обработки принтером.</span><span class="sxs-lookup"><span data-stu-id="1762e-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="1762e-130">Создание задания</span><span class="sxs-lookup"><span data-stu-id="1762e-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="1762e-131">printJob</span><span class="sxs-lookup"><span data-stu-id="1762e-131">printJob</span></span>](printjob.md) | <span data-ttu-id="1762e-132">Создание нового задания печати для принтера.</span><span class="sxs-lookup"><span data-stu-id="1762e-132">Create a new print job for the printer.</span></span> <span data-ttu-id="1762e-133">Чтобы начать печать задания, используйте [Start](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="1762e-133">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="1762e-134">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="1762e-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="1762e-135">Коллекция [принтконнектор](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="1762e-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="1762e-136">Получение списка соединителей, с которыми связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="1762e-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="1762e-137">Перечисление taskTriggers</span><span class="sxs-lookup"><span data-stu-id="1762e-137">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="1762e-138">Нет</span><span class="sxs-lookup"><span data-stu-id="1762e-138">None</span></span> | <span data-ttu-id="1762e-139">Список [принттасктригжерс](printtasktrigger.md) , связанных с этим принтером.</span><span class="sxs-lookup"><span data-stu-id="1762e-139">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="1762e-140">Создание taskTrigger</span><span class="sxs-lookup"><span data-stu-id="1762e-140">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="1762e-141">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="1762e-141">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="1762e-142">Создание [принттасктригжер](printtasktrigger.md) , выполняемого при возникновении событий печати.</span><span class="sxs-lookup"><span data-stu-id="1762e-142">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="1762e-143">Удаление taskTrigger</span><span class="sxs-lookup"><span data-stu-id="1762e-143">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="1762e-144">Нет</span><span class="sxs-lookup"><span data-stu-id="1762e-144">None</span></span> | <span data-ttu-id="1762e-145">Удаление [принттасктригжер](printtasktrigger.md) , связанного с принтером.</span><span class="sxs-lookup"><span data-stu-id="1762e-145">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="1762e-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="1762e-146">Properties</span></span>
| <span data-ttu-id="1762e-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="1762e-147">Property</span></span>     | <span data-ttu-id="1762e-148">Тип</span><span class="sxs-lookup"><span data-stu-id="1762e-148">Type</span></span>        | <span data-ttu-id="1762e-149">Описание</span><span class="sxs-lookup"><span data-stu-id="1762e-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1762e-150">id</span><span class="sxs-lookup"><span data-stu-id="1762e-150">id</span></span>|<span data-ttu-id="1762e-151">String</span><span class="sxs-lookup"><span data-stu-id="1762e-151">String</span></span>|<span data-ttu-id="1762e-152">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="1762e-152">The document's identifier.</span></span> <span data-ttu-id="1762e-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1762e-153">Read-only.</span></span>|
|<span data-ttu-id="1762e-154">displayName</span><span class="sxs-lookup"><span data-stu-id="1762e-154">displayName</span></span>|<span data-ttu-id="1762e-155">String</span><span class="sxs-lookup"><span data-stu-id="1762e-155">String</span></span>|<span data-ttu-id="1762e-156">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="1762e-156">The name of the printer.</span></span>|
|<span data-ttu-id="1762e-157">manufacturer</span><span class="sxs-lookup"><span data-stu-id="1762e-157">manufacturer</span></span>|<span data-ttu-id="1762e-158">String</span><span class="sxs-lookup"><span data-stu-id="1762e-158">String</span></span>|<span data-ttu-id="1762e-159">Производитель, сообщаемый принтером.</span><span class="sxs-lookup"><span data-stu-id="1762e-159">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="1762e-160">model</span><span class="sxs-lookup"><span data-stu-id="1762e-160">model</span></span>|<span data-ttu-id="1762e-161">String</span><span class="sxs-lookup"><span data-stu-id="1762e-161">String</span></span>|<span data-ttu-id="1762e-162">Имя модели, сообщаемое принтером.</span><span class="sxs-lookup"><span data-stu-id="1762e-162">The model name reported by the printer.</span></span>|
|<span data-ttu-id="1762e-163">регистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="1762e-163">registeredDateTime</span></span>|<span data-ttu-id="1762e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1762e-164">DateTimeOffset</span></span>|<span data-ttu-id="1762e-165">Значение DateTimeOffset при регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="1762e-165">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="1762e-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1762e-166">Read-only.</span></span>|
|<span data-ttu-id="1762e-167">status</span><span class="sxs-lookup"><span data-stu-id="1762e-167">status</span></span>|[<span data-ttu-id="1762e-168">принтерстатус</span><span class="sxs-lookup"><span data-stu-id="1762e-168">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="1762e-169">Состояние обработки принтера, включая ошибки.</span><span class="sxs-lookup"><span data-stu-id="1762e-169">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="1762e-170">IsShared</span><span class="sxs-lookup"><span data-stu-id="1762e-170">isShared</span></span>|<span data-ttu-id="1762e-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="1762e-171">Boolean</span></span>|<span data-ttu-id="1762e-172">Значение true, если принтер является общим; в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="1762e-172">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="1762e-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1762e-173">Read-only.</span></span>|
|<span data-ttu-id="1762e-174">хасфисикалдевице</span><span class="sxs-lookup"><span data-stu-id="1762e-174">hasPhysicalDevice</span></span>|<span data-ttu-id="1762e-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="1762e-175">Boolean</span></span>|<span data-ttu-id="1762e-176">Значение true, если у принтера есть физическое устройство для печати.</span><span class="sxs-lookup"><span data-stu-id="1762e-176">True if the printer has a physical device for printing.</span></span> <span data-ttu-id="1762e-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1762e-177">Read-only.</span></span>|
|<span data-ttu-id="1762e-178">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="1762e-178">isAcceptingJobs</span></span>|<span data-ttu-id="1762e-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="1762e-179">Boolean</span></span>|<span data-ttu-id="1762e-180">Принимает ли принтер новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="1762e-180">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="1762e-181">location</span><span class="sxs-lookup"><span data-stu-id="1762e-181">location</span></span>|[<span data-ttu-id="1762e-182">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="1762e-182">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="1762e-183">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="1762e-183">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="1762e-184">defaults</span><span class="sxs-lookup"><span data-stu-id="1762e-184">defaults</span></span>|[<span data-ttu-id="1762e-185">принтердефаултс</span><span class="sxs-lookup"><span data-stu-id="1762e-185">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="1762e-186">Параметры печати по умолчанию для принтера.</span><span class="sxs-lookup"><span data-stu-id="1762e-186">The printer's default print settings.</span></span>|
|<span data-ttu-id="1762e-187">capabilities</span><span class="sxs-lookup"><span data-stu-id="1762e-187">capabilities</span></span>|[<span data-ttu-id="1762e-188">принтеркапабилитиес</span><span class="sxs-lookup"><span data-stu-id="1762e-188">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="1762e-189">Возможности принтера, связанного с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="1762e-189">The capabilities of the printer associated with this printer share.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1762e-190">Связи</span><span class="sxs-lookup"><span data-stu-id="1762e-190">Relationships</span></span>
| <span data-ttu-id="1762e-191">Связь</span><span class="sxs-lookup"><span data-stu-id="1762e-191">Relationship</span></span> | <span data-ttu-id="1762e-192">Тип</span><span class="sxs-lookup"><span data-stu-id="1762e-192">Type</span></span>        | <span data-ttu-id="1762e-193">Описание</span><span class="sxs-lookup"><span data-stu-id="1762e-193">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1762e-194">jobs</span><span class="sxs-lookup"><span data-stu-id="1762e-194">jobs</span></span>|<span data-ttu-id="1762e-195">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="1762e-195">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="1762e-196">Список заданий, помещенных в очередь на печать принтером.</span><span class="sxs-lookup"><span data-stu-id="1762e-196">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="1762e-197">shares</span><span class="sxs-lookup"><span data-stu-id="1762e-197">shares</span></span>|<span data-ttu-id="1762e-198">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="1762e-198">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="1762e-199">Список Принтершарес, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="1762e-199">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="1762e-200">В настоящее время с принтером может быть связан только один Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="1762e-200">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="1762e-201">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1762e-201">Read-only.</span></span> <span data-ttu-id="1762e-202">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1762e-202">Nullable.</span></span>|
|<span data-ttu-id="1762e-203">аудиовыход</span><span class="sxs-lookup"><span data-stu-id="1762e-203">connectors</span></span>|[<span data-ttu-id="1762e-204">принтконнектор</span><span class="sxs-lookup"><span data-stu-id="1762e-204">printConnector</span></span>](printconnector.md)|<span data-ttu-id="1762e-205">Соединители, связанные с принтером.</span><span class="sxs-lookup"><span data-stu-id="1762e-205">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="1762e-206">тасктригжерс</span><span class="sxs-lookup"><span data-stu-id="1762e-206">taskTriggers</span></span>|<span data-ttu-id="1762e-207">Коллекция [принттасктригжер](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="1762e-207">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="1762e-208">Список триггеров задач, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="1762e-208">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1762e-209">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1762e-209">JSON representation</span></span>

<span data-ttu-id="1762e-210">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1762e-210">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printer",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "hasPhysicalDevice": true,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


