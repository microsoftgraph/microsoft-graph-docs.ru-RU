---
title: Тип ресурса printJob
description: Представляет задание печати, которое было в очереди для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5124f3123331c4889f5e16110109938e7f264925
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883039"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="95f95-103">Тип ресурса printJob</span><span class="sxs-lookup"><span data-stu-id="95f95-103">printJob resource type</span></span>

<span data-ttu-id="95f95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95f95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95f95-105">Представляет задание печати, которое было в очереди для принтера.</span><span class="sxs-lookup"><span data-stu-id="95f95-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="95f95-106">Методы</span><span class="sxs-lookup"><span data-stu-id="95f95-106">Methods</span></span>

| <span data-ttu-id="95f95-107">Метод</span><span class="sxs-lookup"><span data-stu-id="95f95-107">Method</span></span>       | <span data-ttu-id="95f95-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="95f95-108">Return Type</span></span> | <span data-ttu-id="95f95-109">Описание</span><span class="sxs-lookup"><span data-stu-id="95f95-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="95f95-110">[получение](../api/printjob-get.md);</span><span class="sxs-lookup"><span data-stu-id="95f95-110">[Get](../api/printjob-get.md)</span></span> | [<span data-ttu-id="95f95-111">printJob</span><span class="sxs-lookup"><span data-stu-id="95f95-111">printJob</span></span>](printjob.md) | <span data-ttu-id="95f95-112">Чтение свойств и связей объекта printJob.</span><span class="sxs-lookup"><span data-stu-id="95f95-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="95f95-113">Создание</span><span class="sxs-lookup"><span data-stu-id="95f95-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="95f95-114">printJob</span><span class="sxs-lookup"><span data-stu-id="95f95-114">printJob</span></span>](printjob.md) | <span data-ttu-id="95f95-115">Создание объекта задания печати.</span><span class="sxs-lookup"><span data-stu-id="95f95-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="95f95-116">Начало</span><span class="sxs-lookup"><span data-stu-id="95f95-116">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="95f95-117">Нет</span><span class="sxs-lookup"><span data-stu-id="95f95-117">None</span></span>|<span data-ttu-id="95f95-118">Запустите задание печати.</span><span class="sxs-lookup"><span data-stu-id="95f95-118">Start the print job.</span></span>|
| [<span data-ttu-id="95f95-119">Отмена</span><span class="sxs-lookup"><span data-stu-id="95f95-119">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="95f95-120">Нет</span><span class="sxs-lookup"><span data-stu-id="95f95-120">None</span></span>|<span data-ttu-id="95f95-121">Отмените задание печати.</span><span class="sxs-lookup"><span data-stu-id="95f95-121">Cancel the print job.</span></span>|
| [<span data-ttu-id="95f95-122">Прервать</span><span class="sxs-lookup"><span data-stu-id="95f95-122">Abort</span></span>](../api/printjob-abort.md)|<span data-ttu-id="95f95-123">Нет</span><span class="sxs-lookup"><span data-stu-id="95f95-123">None</span></span>|<span data-ttu-id="95f95-124">Отменить задание печати.</span><span class="sxs-lookup"><span data-stu-id="95f95-124">Abort the print job.</span></span>|
| [<span data-ttu-id="95f95-125">Перенаправление (на другой принтер)</span><span class="sxs-lookup"><span data-stu-id="95f95-125">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="95f95-126">printJob</span><span class="sxs-lookup"><span data-stu-id="95f95-126">printJob</span></span>](printjob.md) | <span data-ttu-id="95f95-127">Задание печати, которое находится в очереди для принтера назначения.</span><span class="sxs-lookup"><span data-stu-id="95f95-127">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="95f95-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="95f95-128">Properties</span></span>
| <span data-ttu-id="95f95-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="95f95-129">Property</span></span>     | <span data-ttu-id="95f95-130">Тип</span><span class="sxs-lookup"><span data-stu-id="95f95-130">Type</span></span>        | <span data-ttu-id="95f95-131">Описание</span><span class="sxs-lookup"><span data-stu-id="95f95-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="95f95-132">id</span><span class="sxs-lookup"><span data-stu-id="95f95-132">id</span></span>|<span data-ttu-id="95f95-133">Строка</span><span class="sxs-lookup"><span data-stu-id="95f95-133">String</span></span>|<span data-ttu-id="95f95-134">GUID принтера.</span><span class="sxs-lookup"><span data-stu-id="95f95-134">The printer's GUID.</span></span> <span data-ttu-id="95f95-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95f95-135">Read-only.</span></span>|
|<span data-ttu-id="95f95-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95f95-136">createdDateTime</span></span>|<span data-ttu-id="95f95-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95f95-137">DateTimeOffset</span></span>|<span data-ttu-id="95f95-138">DateTimeOffset, когда было создано задание.</span><span class="sxs-lookup"><span data-stu-id="95f95-138">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="95f95-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95f95-139">Read-only.</span></span>|
|<span data-ttu-id="95f95-140">status</span><span class="sxs-lookup"><span data-stu-id="95f95-140">status</span></span>|[<span data-ttu-id="95f95-141">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="95f95-141">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="95f95-142">Состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="95f95-142">The status of the print job.</span></span> <span data-ttu-id="95f95-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95f95-143">Read-only.</span></span>|
|<span data-ttu-id="95f95-144">configuration</span><span class="sxs-lookup"><span data-stu-id="95f95-144">configuration</span></span>|[<span data-ttu-id="95f95-145">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="95f95-145">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="95f95-146">Группа параметров, которые принтер должен использовать для печати задания.</span><span class="sxs-lookup"><span data-stu-id="95f95-146">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="95f95-147">isFetchable</span><span class="sxs-lookup"><span data-stu-id="95f95-147">isFetchable</span></span>|<span data-ttu-id="95f95-148">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="95f95-148">Edm.Boolean</span></span>|<span data-ttu-id="95f95-149">Если засвеяно, документ может быть извлечен принтером.</span><span class="sxs-lookup"><span data-stu-id="95f95-149">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="95f95-150">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="95f95-150">redirectedFrom</span></span>|<span data-ttu-id="95f95-151">Edm.String</span><span class="sxs-lookup"><span data-stu-id="95f95-151">Edm.String</span></span>|<span data-ttu-id="95f95-152">Содержит URL-адрес задания источника, если задание было перенаправлено с другого принтера.</span><span class="sxs-lookup"><span data-stu-id="95f95-152">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="95f95-153">redirectedTo</span><span class="sxs-lookup"><span data-stu-id="95f95-153">redirectedTo</span></span>|<span data-ttu-id="95f95-154">Edm.String</span><span class="sxs-lookup"><span data-stu-id="95f95-154">Edm.String</span></span>|<span data-ttu-id="95f95-155">Содержит URL-адрес задания назначения, если задание было перенаправлено на другой принтер.</span><span class="sxs-lookup"><span data-stu-id="95f95-155">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95f95-156">Связи</span><span class="sxs-lookup"><span data-stu-id="95f95-156">Relationships</span></span>
| <span data-ttu-id="95f95-157">Связь</span><span class="sxs-lookup"><span data-stu-id="95f95-157">Relationship</span></span> | <span data-ttu-id="95f95-158">Тип</span><span class="sxs-lookup"><span data-stu-id="95f95-158">Type</span></span>        | <span data-ttu-id="95f95-159">Описание</span><span class="sxs-lookup"><span data-stu-id="95f95-159">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="95f95-160">createdBy</span><span class="sxs-lookup"><span data-stu-id="95f95-160">createdBy</span></span>|[<span data-ttu-id="95f95-161">userIdentity</span><span class="sxs-lookup"><span data-stu-id="95f95-161">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="95f95-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95f95-162">Read-only.</span></span> <span data-ttu-id="95f95-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="95f95-163">Nullable.</span></span>|
|<span data-ttu-id="95f95-164">documents</span><span class="sxs-lookup"><span data-stu-id="95f95-164">documents</span></span>|<span data-ttu-id="95f95-165">[Коллекция printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="95f95-165">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="95f95-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95f95-166">Read-only.</span></span>|
|<span data-ttu-id="95f95-167">tasks</span><span class="sxs-lookup"><span data-stu-id="95f95-167">tasks</span></span>|<span data-ttu-id="95f95-168">[Коллекция printTask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="95f95-168">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="95f95-169">Список [printTasks,](printtask.md) которые были инициированы этим заданием печати.</span><span class="sxs-lookup"><span data-stu-id="95f95-169">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95f95-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95f95-170">JSON representation</span></span>

<span data-ttu-id="95f95-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95f95-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJob",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "isFetchable": "Boolean",
  "redirectedFrom": "String",
  "redirectedTo": "String",
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
  "configuration": {"@odata.type": "microsoft.graph.printJobConfiguration"},
  "documents": [ {"@odata.type": "microsoft.graph.printDocument"} ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

