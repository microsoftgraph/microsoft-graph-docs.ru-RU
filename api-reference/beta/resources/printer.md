---
title: Тип ресурса Printer
description: Представляет физическое устройство печати, зарегистрированное в универсальной службе печати. Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b86d3607decc8aca5b24b2be6f8344da87693fde
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703575"
---
# <a name="printer-resource-type"></a><span data-ttu-id="9b577-104">Тип ресурса Printer</span><span class="sxs-lookup"><span data-stu-id="9b577-104">printer resource type</span></span>

<span data-ttu-id="9b577-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b577-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b577-106">Представляет устройство принтера, зарегистрированное в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="9b577-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="9b577-107">Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.</span><span class="sxs-lookup"><span data-stu-id="9b577-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="9b577-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9b577-108">Methods</span></span>

| <span data-ttu-id="9b577-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9b577-109">Method</span></span>       | <span data-ttu-id="9b577-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9b577-110">Return Type</span></span> | <span data-ttu-id="9b577-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9b577-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9b577-112">Создание</span><span class="sxs-lookup"><span data-stu-id="9b577-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="9b577-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="9b577-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="9b577-114">Создание (регистрация) нового принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="9b577-114">Create (register) a new printer with Universal Print.</span></span> |
| <span data-ttu-id="9b577-115">[получение](../api/printer-get.md);</span><span class="sxs-lookup"><span data-stu-id="9b577-115">[Get](../api/printer-get.md)</span></span> | [<span data-ttu-id="9b577-116">Printer</span><span class="sxs-lookup"><span data-stu-id="9b577-116">printer</span></span>](printer.md) | <span data-ttu-id="9b577-117">Чтение свойств и связей объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="9b577-117">Read the properties and relationships of the printer object.</span></span> |
| <span data-ttu-id="9b577-118">[обновление](../api/printer-update.md).</span><span class="sxs-lookup"><span data-stu-id="9b577-118">[Update](../api/printer-update.md)</span></span> | [<span data-ttu-id="9b577-119">Printer</span><span class="sxs-lookup"><span data-stu-id="9b577-119">printer</span></span>](printer.md) | <span data-ttu-id="9b577-120">Обновление объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="9b577-120">Update the printer object.</span></span> |
| <span data-ttu-id="9b577-121">[удаление](../api/printer-delete.md);</span><span class="sxs-lookup"><span data-stu-id="9b577-121">[Delete](../api/printer-delete.md)</span></span> | <span data-ttu-id="9b577-122">Нет</span><span class="sxs-lookup"><span data-stu-id="9b577-122">None</span></span> | <span data-ttu-id="9b577-123">Отмените регистрацию физического принтера в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="9b577-123">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="9b577-124">ресторефакторидефаултс</span><span class="sxs-lookup"><span data-stu-id="9b577-124">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="9b577-125">Нет</span><span class="sxs-lookup"><span data-stu-id="9b577-125">None</span></span> | <span data-ttu-id="9b577-126">Восстановление стандартных параметров принтера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9b577-126">Restore a printer's defaults settings to factory defaults.</span></span> |
| [<span data-ttu-id="9b577-127">Список заданий</span><span class="sxs-lookup"><span data-stu-id="9b577-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="9b577-128">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="9b577-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="9b577-129">Получение списка заданий печати, помещенных в очередь для обработки принтером.</span><span class="sxs-lookup"><span data-stu-id="9b577-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="9b577-130">Создание задания</span><span class="sxs-lookup"><span data-stu-id="9b577-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="9b577-131">printJob</span><span class="sxs-lookup"><span data-stu-id="9b577-131">printJob</span></span>](printjob.md) | <span data-ttu-id="9b577-132">Создание нового задания печати для принтера.</span><span class="sxs-lookup"><span data-stu-id="9b577-132">Create a new print job for the printer.</span></span> <span data-ttu-id="9b577-133">Чтобы начать печать задания, используйте [Start](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="9b577-133">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="9b577-134">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="9b577-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="9b577-135">Коллекция [принтконнектор](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="9b577-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="9b577-136">Получение списка соединителей, с которыми связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="9b577-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="9b577-137">Перечисление taskTriggers</span><span class="sxs-lookup"><span data-stu-id="9b577-137">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="9b577-138">Нет</span><span class="sxs-lookup"><span data-stu-id="9b577-138">None</span></span> | <span data-ttu-id="9b577-139">Список [принттасктригжерс](printtasktrigger.md) , связанных с этим принтером.</span><span class="sxs-lookup"><span data-stu-id="9b577-139">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="9b577-140">Создание taskTrigger</span><span class="sxs-lookup"><span data-stu-id="9b577-140">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="9b577-141">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="9b577-141">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="9b577-142">Создание [принттасктригжер](printtasktrigger.md) , выполняемого при возникновении событий печати.</span><span class="sxs-lookup"><span data-stu-id="9b577-142">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="9b577-143">Удаление taskTrigger</span><span class="sxs-lookup"><span data-stu-id="9b577-143">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="9b577-144">Нет</span><span class="sxs-lookup"><span data-stu-id="9b577-144">None</span></span> | <span data-ttu-id="9b577-145">Удаление [принттасктригжер](printtasktrigger.md) , связанного с принтером.</span><span class="sxs-lookup"><span data-stu-id="9b577-145">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="9b577-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b577-146">Properties</span></span>
| <span data-ttu-id="9b577-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b577-147">Property</span></span>     | <span data-ttu-id="9b577-148">Тип</span><span class="sxs-lookup"><span data-stu-id="9b577-148">Type</span></span>        | <span data-ttu-id="9b577-149">Описание</span><span class="sxs-lookup"><span data-stu-id="9b577-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b577-150">id</span><span class="sxs-lookup"><span data-stu-id="9b577-150">id</span></span>|<span data-ttu-id="9b577-151">Строка</span><span class="sxs-lookup"><span data-stu-id="9b577-151">String</span></span>|<span data-ttu-id="9b577-152">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="9b577-152">The document's identifier.</span></span> <span data-ttu-id="9b577-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b577-153">Read-only.</span></span>|
|<span data-ttu-id="9b577-154">displayName</span><span class="sxs-lookup"><span data-stu-id="9b577-154">displayName</span></span>|<span data-ttu-id="9b577-155">Строка</span><span class="sxs-lookup"><span data-stu-id="9b577-155">String</span></span>|<span data-ttu-id="9b577-156">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="9b577-156">The name of the printer.</span></span>|
|<span data-ttu-id="9b577-157">manufacturer</span><span class="sxs-lookup"><span data-stu-id="9b577-157">manufacturer</span></span>|<span data-ttu-id="9b577-158">String</span><span class="sxs-lookup"><span data-stu-id="9b577-158">String</span></span>|<span data-ttu-id="9b577-159">Производитель, сообщаемый принтером.</span><span class="sxs-lookup"><span data-stu-id="9b577-159">The manufacturer reported by the printer.</span></span> <span data-ttu-id="9b577-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b577-160">Read-only.</span></span>|
|<span data-ttu-id="9b577-161">model</span><span class="sxs-lookup"><span data-stu-id="9b577-161">model</span></span>|<span data-ttu-id="9b577-162">String</span><span class="sxs-lookup"><span data-stu-id="9b577-162">String</span></span>|<span data-ttu-id="9b577-163">Имя модели, сообщаемое принтером.</span><span class="sxs-lookup"><span data-stu-id="9b577-163">The model name reported by the printer.</span></span> <span data-ttu-id="9b577-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b577-164">Read-only.</span></span>|
|<span data-ttu-id="9b577-165">регистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="9b577-165">registeredDateTime</span></span>|<span data-ttu-id="9b577-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b577-166">DateTimeOffset</span></span>|<span data-ttu-id="9b577-167">Значение DateTimeOffset при регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="9b577-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="9b577-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b577-168">Read-only.</span></span>|
|<span data-ttu-id="9b577-169">status</span><span class="sxs-lookup"><span data-stu-id="9b577-169">status</span></span>|[<span data-ttu-id="9b577-170">принтерстатус</span><span class="sxs-lookup"><span data-stu-id="9b577-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="9b577-171">Состояние обработки принтера, включая ошибки.</span><span class="sxs-lookup"><span data-stu-id="9b577-171">The processing status of the printer, including any errors.</span></span> <span data-ttu-id="9b577-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b577-172">Read-only.</span></span>|
|<span data-ttu-id="9b577-173">IsShared</span><span class="sxs-lookup"><span data-stu-id="9b577-173">isShared</span></span>|<span data-ttu-id="9b577-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b577-174">Boolean</span></span>|<span data-ttu-id="9b577-175">Значение true, если принтер является общим; в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="9b577-175">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="9b577-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b577-176">Read-only.</span></span>|
|<span data-ttu-id="9b577-177">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="9b577-177">isAcceptingJobs</span></span>|<span data-ttu-id="9b577-178">Логический</span><span class="sxs-lookup"><span data-stu-id="9b577-178">Boolean</span></span>|<span data-ttu-id="9b577-179">Принимает ли принтер новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="9b577-179">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="9b577-180">location</span><span class="sxs-lookup"><span data-stu-id="9b577-180">location</span></span>|[<span data-ttu-id="9b577-181">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="9b577-181">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="9b577-182">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="9b577-182">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="9b577-183">defaults</span><span class="sxs-lookup"><span data-stu-id="9b577-183">defaults</span></span>|[<span data-ttu-id="9b577-184">принтердефаултс</span><span class="sxs-lookup"><span data-stu-id="9b577-184">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="9b577-185">Параметры печати по умолчанию для принтера.</span><span class="sxs-lookup"><span data-stu-id="9b577-185">The printer's default print settings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b577-186">Связи</span><span class="sxs-lookup"><span data-stu-id="9b577-186">Relationships</span></span>
| <span data-ttu-id="9b577-187">Связь</span><span class="sxs-lookup"><span data-stu-id="9b577-187">Relationship</span></span> | <span data-ttu-id="9b577-188">Тип</span><span class="sxs-lookup"><span data-stu-id="9b577-188">Type</span></span>        | <span data-ttu-id="9b577-189">Описание</span><span class="sxs-lookup"><span data-stu-id="9b577-189">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b577-190">jobs</span><span class="sxs-lookup"><span data-stu-id="9b577-190">jobs</span></span>|<span data-ttu-id="9b577-191">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="9b577-191">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="9b577-192">Список заданий, помещенных в очередь на печать принтером.</span><span class="sxs-lookup"><span data-stu-id="9b577-192">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="9b577-193">shares</span><span class="sxs-lookup"><span data-stu-id="9b577-193">shares</span></span>|<span data-ttu-id="9b577-194">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="9b577-194">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="9b577-195">Список Принтершарес, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="9b577-195">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="9b577-196">В настоящее время с принтером может быть связан только один Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="9b577-196">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="9b577-197">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b577-197">Read-only.</span></span> <span data-ttu-id="9b577-198">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9b577-198">Nullable.</span></span>|
|<span data-ttu-id="9b577-199">аудиовыход</span><span class="sxs-lookup"><span data-stu-id="9b577-199">connectors</span></span>|[<span data-ttu-id="9b577-200">принтконнектор</span><span class="sxs-lookup"><span data-stu-id="9b577-200">printConnector</span></span>](printconnector.md)|<span data-ttu-id="9b577-201">Соединители, связанные с принтером.</span><span class="sxs-lookup"><span data-stu-id="9b577-201">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="9b577-202">тасктригжерс</span><span class="sxs-lookup"><span data-stu-id="9b577-202">taskTriggers</span></span>|<span data-ttu-id="9b577-203">Коллекция [принттасктригжер](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="9b577-203">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="9b577-204">Список триггеров задач, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="9b577-204">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b577-205">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b577-205">JSON representation</span></span>

<span data-ttu-id="9b577-206">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b577-206">The following is a JSON representation of the resource.</span></span>

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
  "name": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "acceptingJobs": true,
  "registeredBy": {"@odata.type": "microsoft.graph.printUserIdentity"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"}
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


