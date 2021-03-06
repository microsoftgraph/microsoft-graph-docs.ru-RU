---
title: тип ресурса printJob
description: Представляет задание печати, которое выстроилось в очередь для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 170f413c7607933c2651720c9c9c463f90cf55df
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516530"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="094a0-103">тип ресурса printJob</span><span class="sxs-lookup"><span data-stu-id="094a0-103">printJob resource type</span></span>

<span data-ttu-id="094a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="094a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="094a0-105">Представляет задание печати, которое выстроилось в очередь для принтера.</span><span class="sxs-lookup"><span data-stu-id="094a0-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="094a0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="094a0-106">Methods</span></span>

| <span data-ttu-id="094a0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="094a0-107">Method</span></span>       | <span data-ttu-id="094a0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="094a0-108">Return Type</span></span> | <span data-ttu-id="094a0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="094a0-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="094a0-110">[получение](../api/printjob-get.md);</span><span class="sxs-lookup"><span data-stu-id="094a0-110">[Get](../api/printjob-get.md)</span></span> | [<span data-ttu-id="094a0-111">printJob</span><span class="sxs-lookup"><span data-stu-id="094a0-111">printJob</span></span>](printjob.md) | <span data-ttu-id="094a0-112">Чтение свойств и связей объекта printJob.</span><span class="sxs-lookup"><span data-stu-id="094a0-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="094a0-113">Создание</span><span class="sxs-lookup"><span data-stu-id="094a0-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="094a0-114">printJob</span><span class="sxs-lookup"><span data-stu-id="094a0-114">printJob</span></span>](printjob.md) | <span data-ttu-id="094a0-115">Создание нового объекта задания печати.</span><span class="sxs-lookup"><span data-stu-id="094a0-115">Create a new print job object.</span></span> |
| <span data-ttu-id="094a0-116">[обновление](../api/printjob-update.md).</span><span class="sxs-lookup"><span data-stu-id="094a0-116">[Update](../api/printjob-update.md)</span></span> | [<span data-ttu-id="094a0-117">printJob</span><span class="sxs-lookup"><span data-stu-id="094a0-117">printJob</span></span>](printjob.md) | <span data-ttu-id="094a0-118">Обновление объекта задания печати.</span><span class="sxs-lookup"><span data-stu-id="094a0-118">Update a print job object.</span></span> |
| [<span data-ttu-id="094a0-119">Начало</span><span class="sxs-lookup"><span data-stu-id="094a0-119">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="094a0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="094a0-120">None</span></span>|<span data-ttu-id="094a0-121">Запустите задание печати.</span><span class="sxs-lookup"><span data-stu-id="094a0-121">Start the print job.</span></span>|
| [<span data-ttu-id="094a0-122">Отмена</span><span class="sxs-lookup"><span data-stu-id="094a0-122">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="094a0-123">Нет</span><span class="sxs-lookup"><span data-stu-id="094a0-123">None</span></span>|<span data-ttu-id="094a0-124">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="094a0-124">Cancel the print job.</span></span>|
| [<span data-ttu-id="094a0-125">Прервать</span><span class="sxs-lookup"><span data-stu-id="094a0-125">Abort</span></span>](../api/printjob-abort.md)|<span data-ttu-id="094a0-126">Нет</span><span class="sxs-lookup"><span data-stu-id="094a0-126">None</span></span>|<span data-ttu-id="094a0-127">Прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="094a0-127">Abort the print job.</span></span>|
| [<span data-ttu-id="094a0-128">Перенаправление (на другой принтер)</span><span class="sxs-lookup"><span data-stu-id="094a0-128">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="094a0-129">printJob</span><span class="sxs-lookup"><span data-stu-id="094a0-129">printJob</span></span>](printjob.md) | <span data-ttu-id="094a0-130">Задание печати, которое находится в очереди для принтера назначения.</span><span class="sxs-lookup"><span data-stu-id="094a0-130">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="094a0-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="094a0-131">Properties</span></span>
| <span data-ttu-id="094a0-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="094a0-132">Property</span></span>     | <span data-ttu-id="094a0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="094a0-133">Type</span></span>        | <span data-ttu-id="094a0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="094a0-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="094a0-135">id</span><span class="sxs-lookup"><span data-stu-id="094a0-135">id</span></span>|<span data-ttu-id="094a0-136">String</span><span class="sxs-lookup"><span data-stu-id="094a0-136">String</span></span>|<span data-ttu-id="094a0-137">GUID принтера.</span><span class="sxs-lookup"><span data-stu-id="094a0-137">The printer's GUID.</span></span> <span data-ttu-id="094a0-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="094a0-138">Read-only.</span></span>|
|<span data-ttu-id="094a0-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="094a0-139">createdDateTime</span></span>|<span data-ttu-id="094a0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="094a0-140">DateTimeOffset</span></span>|<span data-ttu-id="094a0-141">DateTimeOffset, когда задание было создано.</span><span class="sxs-lookup"><span data-stu-id="094a0-141">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="094a0-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="094a0-142">Read-only.</span></span>|
|<span data-ttu-id="094a0-143">status</span><span class="sxs-lookup"><span data-stu-id="094a0-143">status</span></span>|[<span data-ttu-id="094a0-144">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="094a0-144">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="094a0-145">Состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="094a0-145">The status of the print job.</span></span> <span data-ttu-id="094a0-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="094a0-146">Read-only.</span></span>|
|<span data-ttu-id="094a0-147">configuration</span><span class="sxs-lookup"><span data-stu-id="094a0-147">configuration</span></span>|[<span data-ttu-id="094a0-148">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="094a0-148">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="094a0-149">Группа параметров, которые принтер должен использовать для печати задания.</span><span class="sxs-lookup"><span data-stu-id="094a0-149">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="094a0-150">isFetchable</span><span class="sxs-lookup"><span data-stu-id="094a0-150">isFetchable</span></span>|<span data-ttu-id="094a0-151">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="094a0-151">Edm.Boolean</span></span>|<span data-ttu-id="094a0-152">Если это так, документ можно получить на принтере.</span><span class="sxs-lookup"><span data-stu-id="094a0-152">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="094a0-153">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="094a0-153">redirectedFrom</span></span>|<span data-ttu-id="094a0-154">Edm.String</span><span class="sxs-lookup"><span data-stu-id="094a0-154">Edm.String</span></span>|<span data-ttu-id="094a0-155">Содержит URL-адрес задания источника, если задание было перенаправлено с другого принтера.</span><span class="sxs-lookup"><span data-stu-id="094a0-155">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="094a0-156">redirectedTo</span><span class="sxs-lookup"><span data-stu-id="094a0-156">redirectedTo</span></span>|<span data-ttu-id="094a0-157">Edm.String</span><span class="sxs-lookup"><span data-stu-id="094a0-157">Edm.String</span></span>|<span data-ttu-id="094a0-158">Содержит URL-адрес задания назначения, если задание было перенаправлено на другой принтер.</span><span class="sxs-lookup"><span data-stu-id="094a0-158">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="094a0-159">Связи</span><span class="sxs-lookup"><span data-stu-id="094a0-159">Relationships</span></span>
| <span data-ttu-id="094a0-160">Связь</span><span class="sxs-lookup"><span data-stu-id="094a0-160">Relationship</span></span> | <span data-ttu-id="094a0-161">Тип</span><span class="sxs-lookup"><span data-stu-id="094a0-161">Type</span></span>        | <span data-ttu-id="094a0-162">Описание</span><span class="sxs-lookup"><span data-stu-id="094a0-162">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="094a0-163">createdBy</span><span class="sxs-lookup"><span data-stu-id="094a0-163">createdBy</span></span>|[<span data-ttu-id="094a0-164">userIdentity</span><span class="sxs-lookup"><span data-stu-id="094a0-164">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="094a0-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="094a0-165">Read-only.</span></span> <span data-ttu-id="094a0-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="094a0-166">Nullable.</span></span>|
|<span data-ttu-id="094a0-167">документы</span><span class="sxs-lookup"><span data-stu-id="094a0-167">documents</span></span>|<span data-ttu-id="094a0-168">[коллекция printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="094a0-168">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="094a0-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="094a0-169">Read-only.</span></span>|
|<span data-ttu-id="094a0-170">tasks</span><span class="sxs-lookup"><span data-stu-id="094a0-170">tasks</span></span>|<span data-ttu-id="094a0-171">[printTask](printtask.md) collection</span><span class="sxs-lookup"><span data-stu-id="094a0-171">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="094a0-172">Список [printTasks,](printtask.md) которые были вызваны этим заданием печати.</span><span class="sxs-lookup"><span data-stu-id="094a0-172">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="094a0-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="094a0-173">JSON representation</span></span>

<span data-ttu-id="094a0-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="094a0-174">The following is a JSON representation of the resource.</span></span>

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

