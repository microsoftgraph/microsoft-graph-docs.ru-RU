---
title: Тип ресурса Printer
description: Представляет физическое устройство печати, зарегистрированное в универсальной службе печати. Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2f1decf04f48f7ee8dc074997e6d503130bc74bc
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848621"
---
# <a name="printer-resource-type"></a><span data-ttu-id="b5bfb-104">Тип ресурса Printer</span><span class="sxs-lookup"><span data-stu-id="b5bfb-104">printer resource type</span></span>

<span data-ttu-id="b5bfb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5bfb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5bfb-106">Представляет устройство принтера, зарегистрированное в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="b5bfb-107">Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="b5bfb-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b5bfb-108">Methods</span></span>

| <span data-ttu-id="b5bfb-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b5bfb-109">Method</span></span>       | <span data-ttu-id="b5bfb-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b5bfb-110">Return Type</span></span> | <span data-ttu-id="b5bfb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b5bfb-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b5bfb-112">Создание</span><span class="sxs-lookup"><span data-stu-id="b5bfb-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="b5bfb-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="b5bfb-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="b5bfb-114">Создание (регистрация) нового принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-114">Create (register) a new printer with Universal Print.</span></span> |
| <span data-ttu-id="b5bfb-115">[получение](../api/printer-get.md);</span><span class="sxs-lookup"><span data-stu-id="b5bfb-115">[Get](../api/printer-get.md)</span></span> | [<span data-ttu-id="b5bfb-116">Printer</span><span class="sxs-lookup"><span data-stu-id="b5bfb-116">printer</span></span>](printer.md) | <span data-ttu-id="b5bfb-117">Чтение свойств и связей объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-117">Read the properties and relationships of the printer object.</span></span> |
| <span data-ttu-id="b5bfb-118">[обновление](../api/printer-update.md).</span><span class="sxs-lookup"><span data-stu-id="b5bfb-118">[Update](../api/printer-update.md)</span></span> | [<span data-ttu-id="b5bfb-119">Printer</span><span class="sxs-lookup"><span data-stu-id="b5bfb-119">printer</span></span>](printer.md) | <span data-ttu-id="b5bfb-120">Обновление объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-120">Update the printer object.</span></span> |
| <span data-ttu-id="b5bfb-121">[удаление](../api/printer-delete.md);</span><span class="sxs-lookup"><span data-stu-id="b5bfb-121">[Delete](../api/printer-delete.md)</span></span> | <span data-ttu-id="b5bfb-122">Нет</span><span class="sxs-lookup"><span data-stu-id="b5bfb-122">None</span></span> | <span data-ttu-id="b5bfb-123">Отмените регистрацию физического принтера в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-123">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="b5bfb-124">ресторефакторидефаултс</span><span class="sxs-lookup"><span data-stu-id="b5bfb-124">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="b5bfb-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b5bfb-125">None</span></span> | <span data-ttu-id="b5bfb-126">Восстановите параметры принтера по умолчанию на значения, заданные производителем.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-126">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="b5bfb-127">Список заданий</span><span class="sxs-lookup"><span data-stu-id="b5bfb-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="b5bfb-128">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="b5bfb-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="b5bfb-129">Получение списка заданий печати, помещенных в очередь для обработки принтером.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="b5bfb-130">Создание задания</span><span class="sxs-lookup"><span data-stu-id="b5bfb-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="b5bfb-131">printJob</span><span class="sxs-lookup"><span data-stu-id="b5bfb-131">printJob</span></span>](printjob.md) | <span data-ttu-id="b5bfb-132">Создание нового задания печати для принтера.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-132">Create a new print job for the printer.</span></span> <span data-ttu-id="b5bfb-133">Чтобы начать печать задания, используйте [Start](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="b5bfb-133">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="b5bfb-134">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="b5bfb-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="b5bfb-135">Коллекция [принтконнектор](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="b5bfb-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="b5bfb-136">Получение списка соединителей, с которыми связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="b5bfb-137">Перечисление taskTriggers</span><span class="sxs-lookup"><span data-stu-id="b5bfb-137">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="b5bfb-138">Нет</span><span class="sxs-lookup"><span data-stu-id="b5bfb-138">None</span></span> | <span data-ttu-id="b5bfb-139">Список [принттасктригжерс](printtasktrigger.md) , связанных с этим принтером.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-139">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="b5bfb-140">Создание taskTrigger</span><span class="sxs-lookup"><span data-stu-id="b5bfb-140">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="b5bfb-141">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="b5bfb-141">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="b5bfb-142">Создание [принттасктригжер](printtasktrigger.md) , выполняемого при возникновении событий печати.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-142">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="b5bfb-143">Удаление taskTrigger</span><span class="sxs-lookup"><span data-stu-id="b5bfb-143">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="b5bfb-144">Нет</span><span class="sxs-lookup"><span data-stu-id="b5bfb-144">None</span></span> | <span data-ttu-id="b5bfb-145">Удаление [принттасктригжер](printtasktrigger.md) , связанного с принтером.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-145">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="b5bfb-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5bfb-146">Properties</span></span>
| <span data-ttu-id="b5bfb-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5bfb-147">Property</span></span>     | <span data-ttu-id="b5bfb-148">Тип</span><span class="sxs-lookup"><span data-stu-id="b5bfb-148">Type</span></span>        | <span data-ttu-id="b5bfb-149">Описание</span><span class="sxs-lookup"><span data-stu-id="b5bfb-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b5bfb-150">id</span><span class="sxs-lookup"><span data-stu-id="b5bfb-150">id</span></span>|<span data-ttu-id="b5bfb-151">String</span><span class="sxs-lookup"><span data-stu-id="b5bfb-151">String</span></span>|<span data-ttu-id="b5bfb-152">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-152">The document's identifier.</span></span> <span data-ttu-id="b5bfb-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-153">Read-only.</span></span>|
|<span data-ttu-id="b5bfb-154">displayName</span><span class="sxs-lookup"><span data-stu-id="b5bfb-154">displayName</span></span>|<span data-ttu-id="b5bfb-155">String</span><span class="sxs-lookup"><span data-stu-id="b5bfb-155">String</span></span>|<span data-ttu-id="b5bfb-156">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-156">The name of the printer.</span></span>|
|<span data-ttu-id="b5bfb-157">manufacturer</span><span class="sxs-lookup"><span data-stu-id="b5bfb-157">manufacturer</span></span>|<span data-ttu-id="b5bfb-158">String</span><span class="sxs-lookup"><span data-stu-id="b5bfb-158">String</span></span>|<span data-ttu-id="b5bfb-159">Производитель, сообщаемый принтером.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-159">The manufacturer reported by the printer.</span></span> <span data-ttu-id="b5bfb-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-160">Read-only.</span></span>|
|<span data-ttu-id="b5bfb-161">model</span><span class="sxs-lookup"><span data-stu-id="b5bfb-161">model</span></span>|<span data-ttu-id="b5bfb-162">String</span><span class="sxs-lookup"><span data-stu-id="b5bfb-162">String</span></span>|<span data-ttu-id="b5bfb-163">Имя модели, сообщаемое принтером.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-163">The model name reported by the printer.</span></span> <span data-ttu-id="b5bfb-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-164">Read-only.</span></span>|
|<span data-ttu-id="b5bfb-165">регистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="b5bfb-165">registeredDateTime</span></span>|<span data-ttu-id="b5bfb-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5bfb-166">DateTimeOffset</span></span>|<span data-ttu-id="b5bfb-167">Значение DateTimeOffset при регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="b5bfb-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-168">Read-only.</span></span>|
|<span data-ttu-id="b5bfb-169">status</span><span class="sxs-lookup"><span data-stu-id="b5bfb-169">status</span></span>|[<span data-ttu-id="b5bfb-170">принтерстатус</span><span class="sxs-lookup"><span data-stu-id="b5bfb-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="b5bfb-171">Состояние обработки принтера, включая ошибки.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-171">The processing status of the printer, including any errors.</span></span> <span data-ttu-id="b5bfb-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-172">Read-only.</span></span>|
|<span data-ttu-id="b5bfb-173">IsShared</span><span class="sxs-lookup"><span data-stu-id="b5bfb-173">isShared</span></span>|<span data-ttu-id="b5bfb-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5bfb-174">Boolean</span></span>|<span data-ttu-id="b5bfb-175">Значение true, если принтер является общим; в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-175">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="b5bfb-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-176">Read-only.</span></span>|
|<span data-ttu-id="b5bfb-177">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="b5bfb-177">isAcceptingJobs</span></span>|<span data-ttu-id="b5bfb-178">Логический</span><span class="sxs-lookup"><span data-stu-id="b5bfb-178">Boolean</span></span>|<span data-ttu-id="b5bfb-179">Принимает ли принтер новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-179">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="b5bfb-180">location</span><span class="sxs-lookup"><span data-stu-id="b5bfb-180">location</span></span>|[<span data-ttu-id="b5bfb-181">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="b5bfb-181">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="b5bfb-182">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-182">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="b5bfb-183">defaults</span><span class="sxs-lookup"><span data-stu-id="b5bfb-183">defaults</span></span>|[<span data-ttu-id="b5bfb-184">принтердефаултс</span><span class="sxs-lookup"><span data-stu-id="b5bfb-184">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="b5bfb-185">Параметры печати по умолчанию для принтера.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-185">The printer's default print settings.</span></span>|
|<span data-ttu-id="b5bfb-186">capabilities</span><span class="sxs-lookup"><span data-stu-id="b5bfb-186">capabilities</span></span>|[<span data-ttu-id="b5bfb-187">принтеркапабилитиес</span><span class="sxs-lookup"><span data-stu-id="b5bfb-187">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="b5bfb-188">Возможности принтера, связанного с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-188">The capabilities of the printer associated with this printer share.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5bfb-189">Связи</span><span class="sxs-lookup"><span data-stu-id="b5bfb-189">Relationships</span></span>
| <span data-ttu-id="b5bfb-190">Связь</span><span class="sxs-lookup"><span data-stu-id="b5bfb-190">Relationship</span></span> | <span data-ttu-id="b5bfb-191">Тип</span><span class="sxs-lookup"><span data-stu-id="b5bfb-191">Type</span></span>        | <span data-ttu-id="b5bfb-192">Описание</span><span class="sxs-lookup"><span data-stu-id="b5bfb-192">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b5bfb-193">jobs</span><span class="sxs-lookup"><span data-stu-id="b5bfb-193">jobs</span></span>|<span data-ttu-id="b5bfb-194">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="b5bfb-194">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="b5bfb-195">Список заданий, помещенных в очередь на печать принтером.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-195">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="b5bfb-196">shares</span><span class="sxs-lookup"><span data-stu-id="b5bfb-196">shares</span></span>|<span data-ttu-id="b5bfb-197">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="b5bfb-197">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="b5bfb-198">Список Принтершарес, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-198">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="b5bfb-199">В настоящее время с принтером может быть связан только один Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-199">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="b5bfb-200">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-200">Read-only.</span></span> <span data-ttu-id="b5bfb-201">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-201">Nullable.</span></span>|
|<span data-ttu-id="b5bfb-202">аудиовыход</span><span class="sxs-lookup"><span data-stu-id="b5bfb-202">connectors</span></span>|[<span data-ttu-id="b5bfb-203">принтконнектор</span><span class="sxs-lookup"><span data-stu-id="b5bfb-203">printConnector</span></span>](printconnector.md)|<span data-ttu-id="b5bfb-204">Соединители, связанные с принтером.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-204">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="b5bfb-205">тасктригжерс</span><span class="sxs-lookup"><span data-stu-id="b5bfb-205">taskTriggers</span></span>|<span data-ttu-id="b5bfb-206">Коллекция [принттасктригжер](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="b5bfb-206">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="b5bfb-207">Список триггеров задач, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-207">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5bfb-208">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b5bfb-208">JSON representation</span></span>

<span data-ttu-id="b5bfb-209">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5bfb-209">The following is a JSON representation of the resource.</span></span>

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


