---
title: тип ресурса принтера
description: Представляет физическое устройство принтера, зарегистрированное в службе универсальной печати. Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d90bf05b77c8843fc9fa5e5f32ecae29ffdaf48e
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765918"
---
# <a name="printer-resource-type"></a><span data-ttu-id="ab50f-104">тип ресурса принтера</span><span class="sxs-lookup"><span data-stu-id="ab50f-104">printer resource type</span></span>

<span data-ttu-id="ab50f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab50f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab50f-106">Представляет устройство принтера, зарегистрированное в службе универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="ab50f-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="ab50f-107">Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.</span><span class="sxs-lookup"><span data-stu-id="ab50f-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

<span data-ttu-id="ab50f-108">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="ab50f-108">This resource supports:</span></span>
* <span data-ttu-id="ab50f-109">[Подписка на изменение уведомлений.](/graph/universal-print-webhook-notifications)</span><span class="sxs-lookup"><span data-stu-id="ab50f-109">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="ab50f-110">Методы</span><span class="sxs-lookup"><span data-stu-id="ab50f-110">Methods</span></span>

| <span data-ttu-id="ab50f-111">Метод</span><span class="sxs-lookup"><span data-stu-id="ab50f-111">Method</span></span>       | <span data-ttu-id="ab50f-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ab50f-112">Return Type</span></span> | <span data-ttu-id="ab50f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ab50f-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ab50f-114">Создание</span><span class="sxs-lookup"><span data-stu-id="ab50f-114">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="ab50f-115">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="ab50f-115">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="ab50f-116">Создание (регистрация) нового принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="ab50f-116">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="ab50f-117">Get</span><span class="sxs-lookup"><span data-stu-id="ab50f-117">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="ab50f-118">printer</span><span class="sxs-lookup"><span data-stu-id="ab50f-118">printer</span></span>](printer.md) | <span data-ttu-id="ab50f-119">Ознакомьтесь с свойствами и отношениями объекта принтера.</span><span class="sxs-lookup"><span data-stu-id="ab50f-119">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="ab50f-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="ab50f-120">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="ab50f-121">printer</span><span class="sxs-lookup"><span data-stu-id="ab50f-121">printer</span></span>](printer.md) | <span data-ttu-id="ab50f-122">Обновление объекта принтера.</span><span class="sxs-lookup"><span data-stu-id="ab50f-122">Update the printer object.</span></span> |
| [<span data-ttu-id="ab50f-123">Delete</span><span class="sxs-lookup"><span data-stu-id="ab50f-123">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="ab50f-124">Нет</span><span class="sxs-lookup"><span data-stu-id="ab50f-124">None</span></span> | <span data-ttu-id="ab50f-125">Отрегистрим физический принтер из службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="ab50f-125">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="ab50f-126">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="ab50f-126">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="ab50f-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ab50f-127">None</span></span> | <span data-ttu-id="ab50f-128">Восстановление параметров по умолчанию принтера до значений, заданных производителем.</span><span class="sxs-lookup"><span data-stu-id="ab50f-128">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="ab50f-129">Список заданий</span><span class="sxs-lookup"><span data-stu-id="ab50f-129">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="ab50f-130">[коллекция printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="ab50f-130">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="ab50f-131">Получите список заданий печати, которые в очереди для обработки принтером.</span><span class="sxs-lookup"><span data-stu-id="ab50f-131">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="ab50f-132">Создание задания</span><span class="sxs-lookup"><span data-stu-id="ab50f-132">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="ab50f-133">printJob</span><span class="sxs-lookup"><span data-stu-id="ab50f-133">printJob</span></span>](printjob.md) | <span data-ttu-id="ab50f-134">Создайте новое задание печати для принтера.</span><span class="sxs-lookup"><span data-stu-id="ab50f-134">Create a new print job for the printer.</span></span> <span data-ttu-id="ab50f-135">Чтобы приступить к печати задания, используйте [start](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="ab50f-135">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="ab50f-136">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="ab50f-136">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="ab50f-137">[коллекция printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="ab50f-137">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="ab50f-138">Получите список соединитений, с которые связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="ab50f-138">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="ab50f-139">Перечисление taskTriggers</span><span class="sxs-lookup"><span data-stu-id="ab50f-139">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="ab50f-140">Нет</span><span class="sxs-lookup"><span data-stu-id="ab50f-140">None</span></span> | <span data-ttu-id="ab50f-141">Список [printTaskTriggers, связанных](printtasktrigger.md) с этим принтером.</span><span class="sxs-lookup"><span data-stu-id="ab50f-141">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="ab50f-142">Создание taskTrigger</span><span class="sxs-lookup"><span data-stu-id="ab50f-142">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="ab50f-143">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="ab50f-143">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="ab50f-144">Создайте [printTaskTrigger,](printtasktrigger.md) который запускается при печатных событиях.</span><span class="sxs-lookup"><span data-stu-id="ab50f-144">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="ab50f-145">Удаление taskTrigger</span><span class="sxs-lookup"><span data-stu-id="ab50f-145">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="ab50f-146">Нет</span><span class="sxs-lookup"><span data-stu-id="ab50f-146">None</span></span> | <span data-ttu-id="ab50f-147">Удалите [печатьTaskTrigger,](printtasktrigger.md) связанную с принтером.</span><span class="sxs-lookup"><span data-stu-id="ab50f-147">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="ab50f-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab50f-148">Properties</span></span>
| <span data-ttu-id="ab50f-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab50f-149">Property</span></span>     | <span data-ttu-id="ab50f-150">Тип</span><span class="sxs-lookup"><span data-stu-id="ab50f-150">Type</span></span>        | <span data-ttu-id="ab50f-151">Описание</span><span class="sxs-lookup"><span data-stu-id="ab50f-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ab50f-152">id</span><span class="sxs-lookup"><span data-stu-id="ab50f-152">id</span></span>|<span data-ttu-id="ab50f-153">String</span><span class="sxs-lookup"><span data-stu-id="ab50f-153">String</span></span>|<span data-ttu-id="ab50f-154">Идентификатор принтера.</span><span class="sxs-lookup"><span data-stu-id="ab50f-154">The printer's identifier.</span></span> <span data-ttu-id="ab50f-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50f-155">Read-only.</span></span>|
|<span data-ttu-id="ab50f-156">displayName</span><span class="sxs-lookup"><span data-stu-id="ab50f-156">displayName</span></span>|<span data-ttu-id="ab50f-157">String</span><span class="sxs-lookup"><span data-stu-id="ab50f-157">String</span></span>|<span data-ttu-id="ab50f-158">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="ab50f-158">The name of the printer.</span></span>|
|<span data-ttu-id="ab50f-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ab50f-159">manufacturer</span></span>|<span data-ttu-id="ab50f-160">String</span><span class="sxs-lookup"><span data-stu-id="ab50f-160">String</span></span>|<span data-ttu-id="ab50f-161">Производитель сообщил на принтере.</span><span class="sxs-lookup"><span data-stu-id="ab50f-161">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="ab50f-162">model</span><span class="sxs-lookup"><span data-stu-id="ab50f-162">model</span></span>|<span data-ttu-id="ab50f-163">String</span><span class="sxs-lookup"><span data-stu-id="ab50f-163">String</span></span>|<span data-ttu-id="ab50f-164">Имя модели, о чем сообщает принтер.</span><span class="sxs-lookup"><span data-stu-id="ab50f-164">The model name reported by the printer.</span></span>|
|<span data-ttu-id="ab50f-165">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="ab50f-165">registeredDateTime</span></span>|<span data-ttu-id="ab50f-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab50f-166">DateTimeOffset</span></span>|<span data-ttu-id="ab50f-167">DateTimeOffset при регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="ab50f-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="ab50f-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50f-168">Read-only.</span></span>|
|<span data-ttu-id="ab50f-169">status</span><span class="sxs-lookup"><span data-stu-id="ab50f-169">status</span></span>|[<span data-ttu-id="ab50f-170">printerStatus</span><span class="sxs-lookup"><span data-stu-id="ab50f-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="ab50f-171">Состояние обработки принтера, включая ошибки.</span><span class="sxs-lookup"><span data-stu-id="ab50f-171">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="ab50f-172">IsShared</span><span class="sxs-lookup"><span data-stu-id="ab50f-172">isShared</span></span>|<span data-ttu-id="ab50f-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab50f-173">Boolean</span></span>|<span data-ttu-id="ab50f-174">True, если принтер является общим; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="ab50f-174">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="ab50f-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50f-175">Read-only.</span></span>|
|<span data-ttu-id="ab50f-176">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="ab50f-176">hasPhysicalDevice</span></span>|<span data-ttu-id="ab50f-177">Логический</span><span class="sxs-lookup"><span data-stu-id="ab50f-177">Boolean</span></span>|<span data-ttu-id="ab50f-178">True, если на принтере есть физическое устройство для печати.</span><span class="sxs-lookup"><span data-stu-id="ab50f-178">True if the printer has a physical device for printing.</span></span> <span data-ttu-id="ab50f-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50f-179">Read-only.</span></span>|
|<span data-ttu-id="ab50f-180">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="ab50f-180">isAcceptingJobs</span></span>|<span data-ttu-id="ab50f-181">Логический</span><span class="sxs-lookup"><span data-stu-id="ab50f-181">Boolean</span></span>|<span data-ttu-id="ab50f-182">Принимает ли принтер новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="ab50f-182">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="ab50f-183">расположение</span><span class="sxs-lookup"><span data-stu-id="ab50f-183">location</span></span>|[<span data-ttu-id="ab50f-184">printerLocation</span><span class="sxs-lookup"><span data-stu-id="ab50f-184">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="ab50f-185">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="ab50f-185">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="ab50f-186">defaults</span><span class="sxs-lookup"><span data-stu-id="ab50f-186">defaults</span></span>|[<span data-ttu-id="ab50f-187">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="ab50f-187">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="ab50f-188">Параметры печати принтера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ab50f-188">The printer's default print settings.</span></span>|
|<span data-ttu-id="ab50f-189">capabilities</span><span class="sxs-lookup"><span data-stu-id="ab50f-189">capabilities</span></span>|[<span data-ttu-id="ab50f-190">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="ab50f-190">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="ab50f-191">Возможности принтера.</span><span class="sxs-lookup"><span data-stu-id="ab50f-191">The capabilities of the printer.</span></span>|
|<span data-ttu-id="ab50f-192">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="ab50f-192">lastSeenDateTime</span></span>|<span data-ttu-id="ab50f-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab50f-193">DateTimeOffset</span></span>|<span data-ttu-id="ab50f-194">Самая недавняя датаTimeOffset при взаимодействии принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="ab50f-194">The most recent dateTimeOffset when a printer interacted with Universal Print.</span></span> <span data-ttu-id="ab50f-195">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50f-195">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab50f-196">Связи</span><span class="sxs-lookup"><span data-stu-id="ab50f-196">Relationships</span></span>
| <span data-ttu-id="ab50f-197">Связь</span><span class="sxs-lookup"><span data-stu-id="ab50f-197">Relationship</span></span> | <span data-ttu-id="ab50f-198">Тип</span><span class="sxs-lookup"><span data-stu-id="ab50f-198">Type</span></span>        | <span data-ttu-id="ab50f-199">Описание</span><span class="sxs-lookup"><span data-stu-id="ab50f-199">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ab50f-200">jobs</span><span class="sxs-lookup"><span data-stu-id="ab50f-200">jobs</span></span>|<span data-ttu-id="ab50f-201">[коллекция printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="ab50f-201">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="ab50f-202">Список заданий, которые в очереди для печати принтером.</span><span class="sxs-lookup"><span data-stu-id="ab50f-202">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="ab50f-203">shares</span><span class="sxs-lookup"><span data-stu-id="ab50f-203">shares</span></span>|<span data-ttu-id="ab50f-204">[коллекция printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="ab50f-204">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="ab50f-205">Список принтеров, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="ab50f-205">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="ab50f-206">В настоящее время только один принтер Может быть связан с принтером.</span><span class="sxs-lookup"><span data-stu-id="ab50f-206">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="ab50f-207">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50f-207">Read-only.</span></span> <span data-ttu-id="ab50f-208">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ab50f-208">Nullable.</span></span>|
|<span data-ttu-id="ab50f-209">соединители</span><span class="sxs-lookup"><span data-stu-id="ab50f-209">connectors</span></span>|[<span data-ttu-id="ab50f-210">printConnector</span><span class="sxs-lookup"><span data-stu-id="ab50f-210">printConnector</span></span>](printconnector.md)|<span data-ttu-id="ab50f-211">Соединители, связанные с принтером.</span><span class="sxs-lookup"><span data-stu-id="ab50f-211">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="ab50f-212">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="ab50f-212">taskTriggers</span></span>|<span data-ttu-id="ab50f-213">[printTaskTrigger](printtasktrigger.md) collection</span><span class="sxs-lookup"><span data-stu-id="ab50f-213">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="ab50f-214">Список триггеров задач, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="ab50f-214">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab50f-215">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab50f-215">JSON representation</span></span>

<span data-ttu-id="ab50f-216">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab50f-216">The following is a JSON representation of the resource.</span></span>

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
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"},
  "lastSeenDateTime": "String (timestamp)"
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


