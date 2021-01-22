---
title: Тип ресурса printer
description: Представляет физическое принтерное устройство, зарегистрированное в службе универсальной печати. Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fab3e933608143846555c556a215025e39666257
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934875"
---
# <a name="printer-resource-type"></a><span data-ttu-id="a0b06-104">Тип ресурса printer</span><span class="sxs-lookup"><span data-stu-id="a0b06-104">printer resource type</span></span>

<span data-ttu-id="a0b06-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0b06-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0b06-106">Представляет принтер, зарегистрированный в службе универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="a0b06-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="a0b06-107">Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.</span><span class="sxs-lookup"><span data-stu-id="a0b06-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

<span data-ttu-id="a0b06-108">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="a0b06-108">This resource supports:</span></span>
* <span data-ttu-id="a0b06-109">[Подписка на уведомления об изменениях.](/graph/universal-print-webhook-notifications)</span><span class="sxs-lookup"><span data-stu-id="a0b06-109">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="a0b06-110">Методы</span><span class="sxs-lookup"><span data-stu-id="a0b06-110">Methods</span></span>

| <span data-ttu-id="a0b06-111">Метод</span><span class="sxs-lookup"><span data-stu-id="a0b06-111">Method</span></span>       | <span data-ttu-id="a0b06-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a0b06-112">Return Type</span></span> | <span data-ttu-id="a0b06-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a0b06-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a0b06-114">Создание</span><span class="sxs-lookup"><span data-stu-id="a0b06-114">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="a0b06-115">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="a0b06-115">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="a0b06-116">Создайте (зарегистрируйте) новый принтер с помощью универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="a0b06-116">Create (register) a new printer with Universal Print.</span></span> |
| <span data-ttu-id="a0b06-117">[получение](../api/printer-get.md);</span><span class="sxs-lookup"><span data-stu-id="a0b06-117">[Get](../api/printer-get.md)</span></span> | [<span data-ttu-id="a0b06-118">printer</span><span class="sxs-lookup"><span data-stu-id="a0b06-118">printer</span></span>](printer.md) | <span data-ttu-id="a0b06-119">Чтение свойств и связей объекта принтера.</span><span class="sxs-lookup"><span data-stu-id="a0b06-119">Read the properties and relationships of the printer object.</span></span> |
| <span data-ttu-id="a0b06-120">[обновление](../api/printer-update.md).</span><span class="sxs-lookup"><span data-stu-id="a0b06-120">[Update](../api/printer-update.md)</span></span> | [<span data-ttu-id="a0b06-121">printer</span><span class="sxs-lookup"><span data-stu-id="a0b06-121">printer</span></span>](printer.md) | <span data-ttu-id="a0b06-122">Обновление объекта принтера.</span><span class="sxs-lookup"><span data-stu-id="a0b06-122">Update the printer object.</span></span> |
| <span data-ttu-id="a0b06-123">[удаление](../api/printer-delete.md);</span><span class="sxs-lookup"><span data-stu-id="a0b06-123">[Delete](../api/printer-delete.md)</span></span> | <span data-ttu-id="a0b06-124">Нет</span><span class="sxs-lookup"><span data-stu-id="a0b06-124">None</span></span> | <span data-ttu-id="a0b06-125">Отостересть физического принтера от службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="a0b06-125">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="a0b06-126">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="a0b06-126">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="a0b06-127">Нет</span><span class="sxs-lookup"><span data-stu-id="a0b06-127">None</span></span> | <span data-ttu-id="a0b06-128">Восстановите параметры принтера по умолчанию до значений, указанных производителем.</span><span class="sxs-lookup"><span data-stu-id="a0b06-128">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="a0b06-129">Список заданий</span><span class="sxs-lookup"><span data-stu-id="a0b06-129">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="a0b06-130">[Коллекция printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="a0b06-130">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="a0b06-131">Получите список заданий печати, которые находятся в очереди для обработки принтером.</span><span class="sxs-lookup"><span data-stu-id="a0b06-131">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="a0b06-132">Создание задания</span><span class="sxs-lookup"><span data-stu-id="a0b06-132">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="a0b06-133">printJob</span><span class="sxs-lookup"><span data-stu-id="a0b06-133">printJob</span></span>](printjob.md) | <span data-ttu-id="a0b06-134">Создайте новое задание печати для принтера.</span><span class="sxs-lookup"><span data-stu-id="a0b06-134">Create a new print job for the printer.</span></span> <span data-ttu-id="a0b06-135">Чтобы начать печать задания, [используйте](../api/printjob-start.md)start .</span><span class="sxs-lookup"><span data-stu-id="a0b06-135">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="a0b06-136">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="a0b06-136">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="a0b06-137">[Коллекция printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="a0b06-137">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="a0b06-138">Получите список соединитений, с которые связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="a0b06-138">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="a0b06-139">Перечисление taskTriggers</span><span class="sxs-lookup"><span data-stu-id="a0b06-139">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="a0b06-140">Нет</span><span class="sxs-lookup"><span data-stu-id="a0b06-140">None</span></span> | <span data-ttu-id="a0b06-141">Список [printTaskTriggers,](printtasktrigger.md) связанных с этим принтером.</span><span class="sxs-lookup"><span data-stu-id="a0b06-141">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="a0b06-142">Создание taskTrigger</span><span class="sxs-lookup"><span data-stu-id="a0b06-142">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="a0b06-143">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="a0b06-143">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="a0b06-144">Создайте [printTaskTrigger,](printtasktrigger.md) который запускается при событиях печати.</span><span class="sxs-lookup"><span data-stu-id="a0b06-144">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="a0b06-145">Удаление taskTrigger</span><span class="sxs-lookup"><span data-stu-id="a0b06-145">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="a0b06-146">Нет</span><span class="sxs-lookup"><span data-stu-id="a0b06-146">None</span></span> | <span data-ttu-id="a0b06-147">Удалите [printTaskTrigger,](printtasktrigger.md) связанный с принтером.</span><span class="sxs-lookup"><span data-stu-id="a0b06-147">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="a0b06-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0b06-148">Properties</span></span>
| <span data-ttu-id="a0b06-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0b06-149">Property</span></span>     | <span data-ttu-id="a0b06-150">Тип</span><span class="sxs-lookup"><span data-stu-id="a0b06-150">Type</span></span>        | <span data-ttu-id="a0b06-151">Описание</span><span class="sxs-lookup"><span data-stu-id="a0b06-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0b06-152">id</span><span class="sxs-lookup"><span data-stu-id="a0b06-152">id</span></span>|<span data-ttu-id="a0b06-153">String</span><span class="sxs-lookup"><span data-stu-id="a0b06-153">String</span></span>|<span data-ttu-id="a0b06-154">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="a0b06-154">The document's identifier.</span></span> <span data-ttu-id="a0b06-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0b06-155">Read-only.</span></span>|
|<span data-ttu-id="a0b06-156">displayName</span><span class="sxs-lookup"><span data-stu-id="a0b06-156">displayName</span></span>|<span data-ttu-id="a0b06-157">String</span><span class="sxs-lookup"><span data-stu-id="a0b06-157">String</span></span>|<span data-ttu-id="a0b06-158">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="a0b06-158">The name of the printer.</span></span>|
|<span data-ttu-id="a0b06-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="a0b06-159">manufacturer</span></span>|<span data-ttu-id="a0b06-160">String</span><span class="sxs-lookup"><span data-stu-id="a0b06-160">String</span></span>|<span data-ttu-id="a0b06-161">Изготовитель, о чем сообщил принтер.</span><span class="sxs-lookup"><span data-stu-id="a0b06-161">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="a0b06-162">model</span><span class="sxs-lookup"><span data-stu-id="a0b06-162">model</span></span>|<span data-ttu-id="a0b06-163">String</span><span class="sxs-lookup"><span data-stu-id="a0b06-163">String</span></span>|<span data-ttu-id="a0b06-164">Имя модели, сообщаемая принтером.</span><span class="sxs-lookup"><span data-stu-id="a0b06-164">The model name reported by the printer.</span></span>|
|<span data-ttu-id="a0b06-165">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="a0b06-165">registeredDateTime</span></span>|<span data-ttu-id="a0b06-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0b06-166">DateTimeOffset</span></span>|<span data-ttu-id="a0b06-167">DateTimeOffset при регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="a0b06-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="a0b06-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0b06-168">Read-only.</span></span>|
|<span data-ttu-id="a0b06-169">status</span><span class="sxs-lookup"><span data-stu-id="a0b06-169">status</span></span>|[<span data-ttu-id="a0b06-170">printerStatus</span><span class="sxs-lookup"><span data-stu-id="a0b06-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="a0b06-171">Состояние обработки принтера, включая все ошибки.</span><span class="sxs-lookup"><span data-stu-id="a0b06-171">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="a0b06-172">IsShared</span><span class="sxs-lookup"><span data-stu-id="a0b06-172">isShared</span></span>|<span data-ttu-id="a0b06-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0b06-173">Boolean</span></span>|<span data-ttu-id="a0b06-174">Имеет true, если принтер является общим; в противном случае false.</span><span class="sxs-lookup"><span data-stu-id="a0b06-174">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="a0b06-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0b06-175">Read-only.</span></span>|
|<span data-ttu-id="a0b06-176">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="a0b06-176">hasPhysicalDevice</span></span>|<span data-ttu-id="a0b06-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0b06-177">Boolean</span></span>|<span data-ttu-id="a0b06-178">Имеет true, если принтер имеет физическое устройство для печати.</span><span class="sxs-lookup"><span data-stu-id="a0b06-178">True if the printer has a physical device for printing.</span></span> <span data-ttu-id="a0b06-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0b06-179">Read-only.</span></span>|
|<span data-ttu-id="a0b06-180">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="a0b06-180">isAcceptingJobs</span></span>|<span data-ttu-id="a0b06-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0b06-181">Boolean</span></span>|<span data-ttu-id="a0b06-182">Принимает ли принтер новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="a0b06-182">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="a0b06-183">location</span><span class="sxs-lookup"><span data-stu-id="a0b06-183">location</span></span>|[<span data-ttu-id="a0b06-184">printerLocation</span><span class="sxs-lookup"><span data-stu-id="a0b06-184">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="a0b06-185">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="a0b06-185">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="a0b06-186">defaults</span><span class="sxs-lookup"><span data-stu-id="a0b06-186">defaults</span></span>|[<span data-ttu-id="a0b06-187">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="a0b06-187">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="a0b06-188">Параметры печати принтера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a0b06-188">The printer's default print settings.</span></span>|
|<span data-ttu-id="a0b06-189">capabilities</span><span class="sxs-lookup"><span data-stu-id="a0b06-189">capabilities</span></span>|[<span data-ttu-id="a0b06-190">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="a0b06-190">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="a0b06-191">Возможности принтера, связанного с этой обоймой принтера.</span><span class="sxs-lookup"><span data-stu-id="a0b06-191">The capabilities of the printer associated with this printer share.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0b06-192">Связи</span><span class="sxs-lookup"><span data-stu-id="a0b06-192">Relationships</span></span>
| <span data-ttu-id="a0b06-193">Связь</span><span class="sxs-lookup"><span data-stu-id="a0b06-193">Relationship</span></span> | <span data-ttu-id="a0b06-194">Тип</span><span class="sxs-lookup"><span data-stu-id="a0b06-194">Type</span></span>        | <span data-ttu-id="a0b06-195">Описание</span><span class="sxs-lookup"><span data-stu-id="a0b06-195">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0b06-196">jobs</span><span class="sxs-lookup"><span data-stu-id="a0b06-196">jobs</span></span>|<span data-ttu-id="a0b06-197">[Коллекция printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="a0b06-197">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="a0b06-198">Список заданий, которые находятся в очереди для печати принтером.</span><span class="sxs-lookup"><span data-stu-id="a0b06-198">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="a0b06-199">shares</span><span class="sxs-lookup"><span data-stu-id="a0b06-199">shares</span></span>|<span data-ttu-id="a0b06-200">[Коллекция printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="a0b06-200">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="a0b06-201">Список printerShares, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="a0b06-201">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="a0b06-202">В настоящее время с принтером может быть связан только один printerShare.</span><span class="sxs-lookup"><span data-stu-id="a0b06-202">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="a0b06-203">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0b06-203">Read-only.</span></span> <span data-ttu-id="a0b06-204">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a0b06-204">Nullable.</span></span>|
|<span data-ttu-id="a0b06-205">соединители</span><span class="sxs-lookup"><span data-stu-id="a0b06-205">connectors</span></span>|[<span data-ttu-id="a0b06-206">printConnector</span><span class="sxs-lookup"><span data-stu-id="a0b06-206">printConnector</span></span>](printconnector.md)|<span data-ttu-id="a0b06-207">Соединители, связанные с принтером.</span><span class="sxs-lookup"><span data-stu-id="a0b06-207">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="a0b06-208">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="a0b06-208">taskTriggers</span></span>|<span data-ttu-id="a0b06-209">[Коллекция printTaskTrigger](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="a0b06-209">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="a0b06-210">Список триггеров задач, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="a0b06-210">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0b06-211">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0b06-211">JSON representation</span></span>

<span data-ttu-id="a0b06-212">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0b06-212">The following is a JSON representation of the resource.</span></span>

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


