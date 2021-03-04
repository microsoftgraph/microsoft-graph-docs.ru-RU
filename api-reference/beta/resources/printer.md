---
title: тип ресурса принтера
description: Представляет физическое устройство принтера, зарегистрированное в службе универсальной печати. Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9adb08cd553857cbc7f7f9ebb257773b8775fa3f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442889"
---
# <a name="printer-resource-type"></a><span data-ttu-id="08aa4-104">тип ресурса принтера</span><span class="sxs-lookup"><span data-stu-id="08aa4-104">printer resource type</span></span>

<span data-ttu-id="08aa4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08aa4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08aa4-106">Представляет устройство принтера, зарегистрированное в службе универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="08aa4-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="08aa4-107">Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.</span><span class="sxs-lookup"><span data-stu-id="08aa4-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

<span data-ttu-id="08aa4-108">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="08aa4-108">This resource supports:</span></span>
* <span data-ttu-id="08aa4-109">[Подписка на изменение уведомлений.](/graph/universal-print-webhook-notifications)</span><span class="sxs-lookup"><span data-stu-id="08aa4-109">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="08aa4-110">Методы</span><span class="sxs-lookup"><span data-stu-id="08aa4-110">Methods</span></span>

| <span data-ttu-id="08aa4-111">Метод</span><span class="sxs-lookup"><span data-stu-id="08aa4-111">Method</span></span>       | <span data-ttu-id="08aa4-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="08aa4-112">Return Type</span></span> | <span data-ttu-id="08aa4-113">Описание</span><span class="sxs-lookup"><span data-stu-id="08aa4-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="08aa4-114">Создание</span><span class="sxs-lookup"><span data-stu-id="08aa4-114">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="08aa4-115">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="08aa4-115">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="08aa4-116">Создание (регистрация) нового принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="08aa4-116">Create (register) a new printer with Universal Print.</span></span> |
| <span data-ttu-id="08aa4-117">[получение](../api/printer-get.md);</span><span class="sxs-lookup"><span data-stu-id="08aa4-117">[Get](../api/printer-get.md)</span></span> | [<span data-ttu-id="08aa4-118">printer</span><span class="sxs-lookup"><span data-stu-id="08aa4-118">printer</span></span>](printer.md) | <span data-ttu-id="08aa4-119">Ознакомьтесь с свойствами и отношениями объекта принтера.</span><span class="sxs-lookup"><span data-stu-id="08aa4-119">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="08aa4-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="08aa4-120">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="08aa4-121">printer</span><span class="sxs-lookup"><span data-stu-id="08aa4-121">printer</span></span>](printer.md) | <span data-ttu-id="08aa4-122">Обновление объекта принтера.</span><span class="sxs-lookup"><span data-stu-id="08aa4-122">Update the printer object.</span></span> |
| <span data-ttu-id="08aa4-123">[удаление](../api/printer-delete.md);</span><span class="sxs-lookup"><span data-stu-id="08aa4-123">[Delete](../api/printer-delete.md)</span></span> | <span data-ttu-id="08aa4-124">Нет</span><span class="sxs-lookup"><span data-stu-id="08aa4-124">None</span></span> | <span data-ttu-id="08aa4-125">Отрегистрим физический принтер из службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="08aa4-125">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="08aa4-126">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="08aa4-126">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="08aa4-127">Нет</span><span class="sxs-lookup"><span data-stu-id="08aa4-127">None</span></span> | <span data-ttu-id="08aa4-128">Восстановление параметров по умолчанию принтера до значений, заданных производителем.</span><span class="sxs-lookup"><span data-stu-id="08aa4-128">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="08aa4-129">Список заданий</span><span class="sxs-lookup"><span data-stu-id="08aa4-129">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="08aa4-130">[коллекция printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="08aa4-130">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="08aa4-131">Получите список заданий печати, которые в очереди для обработки принтером.</span><span class="sxs-lookup"><span data-stu-id="08aa4-131">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="08aa4-132">Создание задания</span><span class="sxs-lookup"><span data-stu-id="08aa4-132">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="08aa4-133">printJob</span><span class="sxs-lookup"><span data-stu-id="08aa4-133">printJob</span></span>](printjob.md) | <span data-ttu-id="08aa4-134">Создайте новое задание печати для принтера.</span><span class="sxs-lookup"><span data-stu-id="08aa4-134">Create a new print job for the printer.</span></span> <span data-ttu-id="08aa4-135">Чтобы приступить к печати задания, используйте [start](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="08aa4-135">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="08aa4-136">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="08aa4-136">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="08aa4-137">[коллекция printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="08aa4-137">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="08aa4-138">Получите список соединитений, с которые связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="08aa4-138">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="08aa4-139">Перечисление taskTriggers</span><span class="sxs-lookup"><span data-stu-id="08aa4-139">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="08aa4-140">Нет</span><span class="sxs-lookup"><span data-stu-id="08aa4-140">None</span></span> | <span data-ttu-id="08aa4-141">Список [printTaskTriggers, связанных](printtasktrigger.md) с этим принтером.</span><span class="sxs-lookup"><span data-stu-id="08aa4-141">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="08aa4-142">Создание taskTrigger</span><span class="sxs-lookup"><span data-stu-id="08aa4-142">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="08aa4-143">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="08aa4-143">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="08aa4-144">Создайте [printTaskTrigger,](printtasktrigger.md) который запускается при печатных событиях.</span><span class="sxs-lookup"><span data-stu-id="08aa4-144">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="08aa4-145">Удаление taskTrigger</span><span class="sxs-lookup"><span data-stu-id="08aa4-145">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="08aa4-146">Нет</span><span class="sxs-lookup"><span data-stu-id="08aa4-146">None</span></span> | <span data-ttu-id="08aa4-147">Удалите [печатьTaskTrigger,](printtasktrigger.md) связанную с принтером.</span><span class="sxs-lookup"><span data-stu-id="08aa4-147">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="08aa4-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="08aa4-148">Properties</span></span>
| <span data-ttu-id="08aa4-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="08aa4-149">Property</span></span>     | <span data-ttu-id="08aa4-150">Тип</span><span class="sxs-lookup"><span data-stu-id="08aa4-150">Type</span></span>        | <span data-ttu-id="08aa4-151">Описание</span><span class="sxs-lookup"><span data-stu-id="08aa4-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08aa4-152">id</span><span class="sxs-lookup"><span data-stu-id="08aa4-152">id</span></span>|<span data-ttu-id="08aa4-153">String</span><span class="sxs-lookup"><span data-stu-id="08aa4-153">String</span></span>|<span data-ttu-id="08aa4-154">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="08aa4-154">The document's identifier.</span></span> <span data-ttu-id="08aa4-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08aa4-155">Read-only.</span></span>|
|<span data-ttu-id="08aa4-156">displayName</span><span class="sxs-lookup"><span data-stu-id="08aa4-156">displayName</span></span>|<span data-ttu-id="08aa4-157">String</span><span class="sxs-lookup"><span data-stu-id="08aa4-157">String</span></span>|<span data-ttu-id="08aa4-158">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="08aa4-158">The name of the printer.</span></span>|
|<span data-ttu-id="08aa4-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="08aa4-159">manufacturer</span></span>|<span data-ttu-id="08aa4-160">String</span><span class="sxs-lookup"><span data-stu-id="08aa4-160">String</span></span>|<span data-ttu-id="08aa4-161">Производитель сообщил на принтере.</span><span class="sxs-lookup"><span data-stu-id="08aa4-161">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="08aa4-162">model</span><span class="sxs-lookup"><span data-stu-id="08aa4-162">model</span></span>|<span data-ttu-id="08aa4-163">String</span><span class="sxs-lookup"><span data-stu-id="08aa4-163">String</span></span>|<span data-ttu-id="08aa4-164">Имя модели, о чем сообщает принтер.</span><span class="sxs-lookup"><span data-stu-id="08aa4-164">The model name reported by the printer.</span></span>|
|<span data-ttu-id="08aa4-165">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="08aa4-165">registeredDateTime</span></span>|<span data-ttu-id="08aa4-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08aa4-166">DateTimeOffset</span></span>|<span data-ttu-id="08aa4-167">DateTimeOffset при регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="08aa4-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="08aa4-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08aa4-168">Read-only.</span></span>|
|<span data-ttu-id="08aa4-169">status</span><span class="sxs-lookup"><span data-stu-id="08aa4-169">status</span></span>|[<span data-ttu-id="08aa4-170">printerStatus</span><span class="sxs-lookup"><span data-stu-id="08aa4-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="08aa4-171">Состояние обработки принтера, включая ошибки.</span><span class="sxs-lookup"><span data-stu-id="08aa4-171">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="08aa4-172">IsShared</span><span class="sxs-lookup"><span data-stu-id="08aa4-172">isShared</span></span>|<span data-ttu-id="08aa4-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="08aa4-173">Boolean</span></span>|<span data-ttu-id="08aa4-174">True, если принтер является общим; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="08aa4-174">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="08aa4-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08aa4-175">Read-only.</span></span>|
|<span data-ttu-id="08aa4-176">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="08aa4-176">hasPhysicalDevice</span></span>|<span data-ttu-id="08aa4-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="08aa4-177">Boolean</span></span>|<span data-ttu-id="08aa4-178">True, если на принтере есть физическое устройство для печати.</span><span class="sxs-lookup"><span data-stu-id="08aa4-178">True if the printer has a physical device for printing.</span></span> <span data-ttu-id="08aa4-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08aa4-179">Read-only.</span></span>|
|<span data-ttu-id="08aa4-180">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="08aa4-180">isAcceptingJobs</span></span>|<span data-ttu-id="08aa4-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="08aa4-181">Boolean</span></span>|<span data-ttu-id="08aa4-182">Принимает ли принтер новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="08aa4-182">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="08aa4-183">расположение</span><span class="sxs-lookup"><span data-stu-id="08aa4-183">location</span></span>|[<span data-ttu-id="08aa4-184">printerLocation</span><span class="sxs-lookup"><span data-stu-id="08aa4-184">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="08aa4-185">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="08aa4-185">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="08aa4-186">defaults</span><span class="sxs-lookup"><span data-stu-id="08aa4-186">defaults</span></span>|[<span data-ttu-id="08aa4-187">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="08aa4-187">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="08aa4-188">Параметры печати принтера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="08aa4-188">The printer's default print settings.</span></span>|
|<span data-ttu-id="08aa4-189">capabilities</span><span class="sxs-lookup"><span data-stu-id="08aa4-189">capabilities</span></span>|[<span data-ttu-id="08aa4-190">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="08aa4-190">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="08aa4-191">Возможности принтера, связанного с этим разделом принтера.</span><span class="sxs-lookup"><span data-stu-id="08aa4-191">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="08aa4-192">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="08aa4-192">lastSeenDateTime</span></span>|<span data-ttu-id="08aa4-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08aa4-193">DateTimeOffset</span></span>|<span data-ttu-id="08aa4-194">Самая недавняя датаTimeOffset при взаимодействии принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="08aa4-194">The most recent dateTimeOffset when a printer interacted with Universal Print.</span></span> <span data-ttu-id="08aa4-195">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08aa4-195">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08aa4-196">Связи</span><span class="sxs-lookup"><span data-stu-id="08aa4-196">Relationships</span></span>
| <span data-ttu-id="08aa4-197">Связь</span><span class="sxs-lookup"><span data-stu-id="08aa4-197">Relationship</span></span> | <span data-ttu-id="08aa4-198">Тип</span><span class="sxs-lookup"><span data-stu-id="08aa4-198">Type</span></span>        | <span data-ttu-id="08aa4-199">Описание</span><span class="sxs-lookup"><span data-stu-id="08aa4-199">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08aa4-200">jobs</span><span class="sxs-lookup"><span data-stu-id="08aa4-200">jobs</span></span>|<span data-ttu-id="08aa4-201">[коллекция printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="08aa4-201">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="08aa4-202">Список заданий, которые в очереди для печати принтером.</span><span class="sxs-lookup"><span data-stu-id="08aa4-202">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="08aa4-203">shares</span><span class="sxs-lookup"><span data-stu-id="08aa4-203">shares</span></span>|<span data-ttu-id="08aa4-204">[коллекция printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="08aa4-204">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="08aa4-205">Список принтеров, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="08aa4-205">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="08aa4-206">В настоящее время только один принтер Может быть связан с принтером.</span><span class="sxs-lookup"><span data-stu-id="08aa4-206">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="08aa4-207">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08aa4-207">Read-only.</span></span> <span data-ttu-id="08aa4-208">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="08aa4-208">Nullable.</span></span>|
|<span data-ttu-id="08aa4-209">соединители</span><span class="sxs-lookup"><span data-stu-id="08aa4-209">connectors</span></span>|[<span data-ttu-id="08aa4-210">printConnector</span><span class="sxs-lookup"><span data-stu-id="08aa4-210">printConnector</span></span>](printconnector.md)|<span data-ttu-id="08aa4-211">Соединители, связанные с принтером.</span><span class="sxs-lookup"><span data-stu-id="08aa4-211">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="08aa4-212">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="08aa4-212">taskTriggers</span></span>|<span data-ttu-id="08aa4-213">[printTaskTrigger](printtasktrigger.md) collection</span><span class="sxs-lookup"><span data-stu-id="08aa4-213">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="08aa4-214">Список триггеров задач, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="08aa4-214">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08aa4-215">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08aa4-215">JSON representation</span></span>

<span data-ttu-id="08aa4-216">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08aa4-216">The following is a JSON representation of the resource.</span></span>

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


