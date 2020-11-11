---
title: Тип ресурса Printer
description: Представляет физическое устройство печати, зарегистрированное в универсальной службе печати. Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 37c552a1239ee1d374c22be77ba81004cfc92e1f
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/11/2020
ms.locfileid: "48993964"
---
# <a name="printer-resource-type"></a><span data-ttu-id="61147-104">Тип ресурса Printer</span><span class="sxs-lookup"><span data-stu-id="61147-104">printer resource type</span></span>

<span data-ttu-id="61147-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61147-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61147-106">Представляет устройство принтера, зарегистрированное в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="61147-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="61147-107">Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.</span><span class="sxs-lookup"><span data-stu-id="61147-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="61147-108">Методы</span><span class="sxs-lookup"><span data-stu-id="61147-108">Methods</span></span>

| <span data-ttu-id="61147-109">Метод</span><span class="sxs-lookup"><span data-stu-id="61147-109">Method</span></span>       | <span data-ttu-id="61147-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="61147-110">Return Type</span></span> | <span data-ttu-id="61147-111">Описание</span><span class="sxs-lookup"><span data-stu-id="61147-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="61147-112">Создание</span><span class="sxs-lookup"><span data-stu-id="61147-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="61147-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="61147-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="61147-114">Создание (регистрация) нового принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="61147-114">Create (register) a new printer with Universal Print.</span></span> |
| <span data-ttu-id="61147-115">[получение](../api/printer-get.md);</span><span class="sxs-lookup"><span data-stu-id="61147-115">[Get](../api/printer-get.md)</span></span> | [<span data-ttu-id="61147-116">Printer</span><span class="sxs-lookup"><span data-stu-id="61147-116">printer</span></span>](printer.md) | <span data-ttu-id="61147-117">Чтение свойств и связей объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="61147-117">Read the properties and relationships of the printer object.</span></span> |
| <span data-ttu-id="61147-118">[обновление](../api/printer-update.md).</span><span class="sxs-lookup"><span data-stu-id="61147-118">[Update](../api/printer-update.md)</span></span> | [<span data-ttu-id="61147-119">Printer</span><span class="sxs-lookup"><span data-stu-id="61147-119">printer</span></span>](printer.md) | <span data-ttu-id="61147-120">Обновление объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="61147-120">Update the printer object.</span></span> |
| <span data-ttu-id="61147-121">[удаление](../api/printer-delete.md);</span><span class="sxs-lookup"><span data-stu-id="61147-121">[Delete](../api/printer-delete.md)</span></span> | <span data-ttu-id="61147-122">Нет</span><span class="sxs-lookup"><span data-stu-id="61147-122">None</span></span> | <span data-ttu-id="61147-123">Отмените регистрацию физического принтера в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="61147-123">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="61147-124">ресторефакторидефаултс</span><span class="sxs-lookup"><span data-stu-id="61147-124">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="61147-125">Нет</span><span class="sxs-lookup"><span data-stu-id="61147-125">None</span></span> | <span data-ttu-id="61147-126">Восстановите параметры принтера по умолчанию на значения, заданные производителем.</span><span class="sxs-lookup"><span data-stu-id="61147-126">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="61147-127">Список заданий</span><span class="sxs-lookup"><span data-stu-id="61147-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="61147-128">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="61147-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="61147-129">Получение списка заданий печати, помещенных в очередь для обработки принтером.</span><span class="sxs-lookup"><span data-stu-id="61147-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="61147-130">Создание задания</span><span class="sxs-lookup"><span data-stu-id="61147-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="61147-131">printJob</span><span class="sxs-lookup"><span data-stu-id="61147-131">printJob</span></span>](printjob.md) | <span data-ttu-id="61147-132">Создание нового задания печати для принтера.</span><span class="sxs-lookup"><span data-stu-id="61147-132">Create a new print job for the printer.</span></span> <span data-ttu-id="61147-133">Чтобы начать печать задания, используйте [Start](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="61147-133">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="61147-134">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="61147-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="61147-135">Коллекция [принтконнектор](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="61147-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="61147-136">Получение списка соединителей, с которыми связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="61147-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="61147-137">Перечисление taskTriggers</span><span class="sxs-lookup"><span data-stu-id="61147-137">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="61147-138">Нет</span><span class="sxs-lookup"><span data-stu-id="61147-138">None</span></span> | <span data-ttu-id="61147-139">Список [принттасктригжерс](printtasktrigger.md) , связанных с этим принтером.</span><span class="sxs-lookup"><span data-stu-id="61147-139">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="61147-140">Создание taskTrigger</span><span class="sxs-lookup"><span data-stu-id="61147-140">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="61147-141">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="61147-141">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="61147-142">Создание [принттасктригжер](printtasktrigger.md) , выполняемого при возникновении событий печати.</span><span class="sxs-lookup"><span data-stu-id="61147-142">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="61147-143">Удаление taskTrigger</span><span class="sxs-lookup"><span data-stu-id="61147-143">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="61147-144">Нет</span><span class="sxs-lookup"><span data-stu-id="61147-144">None</span></span> | <span data-ttu-id="61147-145">Удаление [принттасктригжер](printtasktrigger.md) , связанного с принтером.</span><span class="sxs-lookup"><span data-stu-id="61147-145">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="61147-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="61147-146">Properties</span></span>
| <span data-ttu-id="61147-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="61147-147">Property</span></span>     | <span data-ttu-id="61147-148">Тип</span><span class="sxs-lookup"><span data-stu-id="61147-148">Type</span></span>        | <span data-ttu-id="61147-149">Описание</span><span class="sxs-lookup"><span data-stu-id="61147-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="61147-150">id</span><span class="sxs-lookup"><span data-stu-id="61147-150">id</span></span>|<span data-ttu-id="61147-151">String</span><span class="sxs-lookup"><span data-stu-id="61147-151">String</span></span>|<span data-ttu-id="61147-152">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="61147-152">The document's identifier.</span></span> <span data-ttu-id="61147-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61147-153">Read-only.</span></span>|
|<span data-ttu-id="61147-154">displayName</span><span class="sxs-lookup"><span data-stu-id="61147-154">displayName</span></span>|<span data-ttu-id="61147-155">String</span><span class="sxs-lookup"><span data-stu-id="61147-155">String</span></span>|<span data-ttu-id="61147-156">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="61147-156">The name of the printer.</span></span>|
|<span data-ttu-id="61147-157">manufacturer</span><span class="sxs-lookup"><span data-stu-id="61147-157">manufacturer</span></span>|<span data-ttu-id="61147-158">String</span><span class="sxs-lookup"><span data-stu-id="61147-158">String</span></span>|<span data-ttu-id="61147-159">Производитель, сообщаемый принтером.</span><span class="sxs-lookup"><span data-stu-id="61147-159">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="61147-160">model</span><span class="sxs-lookup"><span data-stu-id="61147-160">model</span></span>|<span data-ttu-id="61147-161">String</span><span class="sxs-lookup"><span data-stu-id="61147-161">String</span></span>|<span data-ttu-id="61147-162">Имя модели, сообщаемое принтером.</span><span class="sxs-lookup"><span data-stu-id="61147-162">The model name reported by the printer.</span></span>|
|<span data-ttu-id="61147-163">регистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="61147-163">registeredDateTime</span></span>|<span data-ttu-id="61147-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61147-164">DateTimeOffset</span></span>|<span data-ttu-id="61147-165">Значение DateTimeOffset при регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="61147-165">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="61147-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61147-166">Read-only.</span></span>|
|<span data-ttu-id="61147-167">status</span><span class="sxs-lookup"><span data-stu-id="61147-167">status</span></span>|[<span data-ttu-id="61147-168">принтерстатус</span><span class="sxs-lookup"><span data-stu-id="61147-168">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="61147-169">Состояние обработки принтера, включая ошибки.</span><span class="sxs-lookup"><span data-stu-id="61147-169">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="61147-170">IsShared</span><span class="sxs-lookup"><span data-stu-id="61147-170">isShared</span></span>|<span data-ttu-id="61147-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="61147-171">Boolean</span></span>|<span data-ttu-id="61147-172">Значение true, если принтер является общим; в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="61147-172">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="61147-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61147-173">Read-only.</span></span>|
|<span data-ttu-id="61147-174">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="61147-174">isAcceptingJobs</span></span>|<span data-ttu-id="61147-175">Логический</span><span class="sxs-lookup"><span data-stu-id="61147-175">Boolean</span></span>|<span data-ttu-id="61147-176">Принимает ли принтер новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="61147-176">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="61147-177">расположение</span><span class="sxs-lookup"><span data-stu-id="61147-177">location</span></span>|[<span data-ttu-id="61147-178">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="61147-178">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="61147-179">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="61147-179">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="61147-180">defaults</span><span class="sxs-lookup"><span data-stu-id="61147-180">defaults</span></span>|[<span data-ttu-id="61147-181">принтердефаултс</span><span class="sxs-lookup"><span data-stu-id="61147-181">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="61147-182">Параметры печати по умолчанию для принтера.</span><span class="sxs-lookup"><span data-stu-id="61147-182">The printer's default print settings.</span></span>|
|<span data-ttu-id="61147-183">capabilities</span><span class="sxs-lookup"><span data-stu-id="61147-183">capabilities</span></span>|[<span data-ttu-id="61147-184">принтеркапабилитиес</span><span class="sxs-lookup"><span data-stu-id="61147-184">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="61147-185">Возможности принтера, связанного с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="61147-185">The capabilities of the printer associated with this printer share.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61147-186">Связи</span><span class="sxs-lookup"><span data-stu-id="61147-186">Relationships</span></span>
| <span data-ttu-id="61147-187">Связь</span><span class="sxs-lookup"><span data-stu-id="61147-187">Relationship</span></span> | <span data-ttu-id="61147-188">Тип</span><span class="sxs-lookup"><span data-stu-id="61147-188">Type</span></span>        | <span data-ttu-id="61147-189">Описание</span><span class="sxs-lookup"><span data-stu-id="61147-189">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="61147-190">jobs</span><span class="sxs-lookup"><span data-stu-id="61147-190">jobs</span></span>|<span data-ttu-id="61147-191">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="61147-191">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="61147-192">Список заданий, помещенных в очередь на печать принтером.</span><span class="sxs-lookup"><span data-stu-id="61147-192">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="61147-193">shares</span><span class="sxs-lookup"><span data-stu-id="61147-193">shares</span></span>|<span data-ttu-id="61147-194">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="61147-194">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="61147-195">Список Принтершарес, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="61147-195">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="61147-196">В настоящее время с принтером может быть связан только один Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="61147-196">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="61147-197">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61147-197">Read-only.</span></span> <span data-ttu-id="61147-198">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="61147-198">Nullable.</span></span>|
|<span data-ttu-id="61147-199">аудиовыход</span><span class="sxs-lookup"><span data-stu-id="61147-199">connectors</span></span>|[<span data-ttu-id="61147-200">принтконнектор</span><span class="sxs-lookup"><span data-stu-id="61147-200">printConnector</span></span>](printconnector.md)|<span data-ttu-id="61147-201">Соединители, связанные с принтером.</span><span class="sxs-lookup"><span data-stu-id="61147-201">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="61147-202">тасктригжерс</span><span class="sxs-lookup"><span data-stu-id="61147-202">taskTriggers</span></span>|<span data-ttu-id="61147-203">Коллекция [принттасктригжер](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="61147-203">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="61147-204">Список триггеров задач, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="61147-204">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61147-205">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61147-205">JSON representation</span></span>

<span data-ttu-id="61147-206">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61147-206">The following is a JSON representation of the resource.</span></span>

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


