---
title: Тип ресурса printJob
description: Представляет задание печати, которое было в очереди для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 43b08c39715c9984a1692c0bcb823881be4ab4d1
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784831"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="2a436-103">Тип ресурса printJob</span><span class="sxs-lookup"><span data-stu-id="2a436-103">printJob resource type</span></span>

<span data-ttu-id="2a436-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a436-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a436-105">Представляет задание печати, которое было в очереди для принтера.</span><span class="sxs-lookup"><span data-stu-id="2a436-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="2a436-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2a436-106">Methods</span></span>

| <span data-ttu-id="2a436-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2a436-107">Method</span></span>       | <span data-ttu-id="2a436-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2a436-108">Return Type</span></span> | <span data-ttu-id="2a436-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2a436-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2a436-110">[получение](../api/printjob-get.md);</span><span class="sxs-lookup"><span data-stu-id="2a436-110">[Get](../api/printjob-get.md)</span></span> | [<span data-ttu-id="2a436-111">printJob</span><span class="sxs-lookup"><span data-stu-id="2a436-111">printJob</span></span>](printjob.md) | <span data-ttu-id="2a436-112">Чтение свойств и связей объекта printJob.</span><span class="sxs-lookup"><span data-stu-id="2a436-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="2a436-113">Создание</span><span class="sxs-lookup"><span data-stu-id="2a436-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="2a436-114">printJob</span><span class="sxs-lookup"><span data-stu-id="2a436-114">printJob</span></span>](printjob.md) | <span data-ttu-id="2a436-115">Создание объекта задания печати.</span><span class="sxs-lookup"><span data-stu-id="2a436-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="2a436-116">Начало</span><span class="sxs-lookup"><span data-stu-id="2a436-116">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="2a436-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2a436-117">None</span></span>|<span data-ttu-id="2a436-118">Запустите задание печати.</span><span class="sxs-lookup"><span data-stu-id="2a436-118">Start the print job.</span></span>|
| [<span data-ttu-id="2a436-119">Отмена</span><span class="sxs-lookup"><span data-stu-id="2a436-119">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="2a436-120">Нет</span><span class="sxs-lookup"><span data-stu-id="2a436-120">None</span></span>|<span data-ttu-id="2a436-121">Отмените задание печати.</span><span class="sxs-lookup"><span data-stu-id="2a436-121">Cancel the print job.</span></span>|
| [<span data-ttu-id="2a436-122">Прервать</span><span class="sxs-lookup"><span data-stu-id="2a436-122">Abort</span></span>](../api/printjob-abort.md)|<span data-ttu-id="2a436-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2a436-123">None</span></span>|<span data-ttu-id="2a436-124">Отменить задание печати.</span><span class="sxs-lookup"><span data-stu-id="2a436-124">Abort the print job.</span></span>|
| [<span data-ttu-id="2a436-125">Перенаправление (на другой принтер)</span><span class="sxs-lookup"><span data-stu-id="2a436-125">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="2a436-126">printJob</span><span class="sxs-lookup"><span data-stu-id="2a436-126">printJob</span></span>](printjob.md) | <span data-ttu-id="2a436-127">Задание печати, которое находится в очереди для принтера назначения.</span><span class="sxs-lookup"><span data-stu-id="2a436-127">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="2a436-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a436-128">Properties</span></span>
| <span data-ttu-id="2a436-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a436-129">Property</span></span>     | <span data-ttu-id="2a436-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2a436-130">Type</span></span>        | <span data-ttu-id="2a436-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2a436-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2a436-132">id</span><span class="sxs-lookup"><span data-stu-id="2a436-132">id</span></span>|<span data-ttu-id="2a436-133">String</span><span class="sxs-lookup"><span data-stu-id="2a436-133">String</span></span>|<span data-ttu-id="2a436-134">GUID принтера.</span><span class="sxs-lookup"><span data-stu-id="2a436-134">The printer's GUID.</span></span> <span data-ttu-id="2a436-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a436-135">Read-only.</span></span>|
|<span data-ttu-id="2a436-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a436-136">createdDateTime</span></span>|<span data-ttu-id="2a436-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a436-137">DateTimeOffset</span></span>|<span data-ttu-id="2a436-138">DateTimeOffset, когда было создано задание.</span><span class="sxs-lookup"><span data-stu-id="2a436-138">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="2a436-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a436-139">Read-only.</span></span>|
|<span data-ttu-id="2a436-140">status</span><span class="sxs-lookup"><span data-stu-id="2a436-140">status</span></span>|[<span data-ttu-id="2a436-141">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="2a436-141">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="2a436-142">Состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="2a436-142">The status of the print job.</span></span> <span data-ttu-id="2a436-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a436-143">Read-only.</span></span>|
|<span data-ttu-id="2a436-144">configuration</span><span class="sxs-lookup"><span data-stu-id="2a436-144">configuration</span></span>|[<span data-ttu-id="2a436-145">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a436-145">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="2a436-146">Группа параметров, которые принтер должен использовать для печати задания.</span><span class="sxs-lookup"><span data-stu-id="2a436-146">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="2a436-147">isFetchable</span><span class="sxs-lookup"><span data-stu-id="2a436-147">isFetchable</span></span>|<span data-ttu-id="2a436-148">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="2a436-148">Edm.Boolean</span></span>|<span data-ttu-id="2a436-149">Если засвеяно, документ может быть извлечен принтером.</span><span class="sxs-lookup"><span data-stu-id="2a436-149">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="2a436-150">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="2a436-150">redirectedFrom</span></span>|<span data-ttu-id="2a436-151">Edm.String</span><span class="sxs-lookup"><span data-stu-id="2a436-151">Edm.String</span></span>|<span data-ttu-id="2a436-152">Содержит URL-адрес задания источника, если задание было перенаправлено с другого принтера.</span><span class="sxs-lookup"><span data-stu-id="2a436-152">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="2a436-153">redirectedTo</span><span class="sxs-lookup"><span data-stu-id="2a436-153">redirectedTo</span></span>|<span data-ttu-id="2a436-154">Edm.String</span><span class="sxs-lookup"><span data-stu-id="2a436-154">Edm.String</span></span>|<span data-ttu-id="2a436-155">Содержит URL-адрес задания назначения, если задание было перенаправлено на другой принтер.</span><span class="sxs-lookup"><span data-stu-id="2a436-155">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a436-156">Связи</span><span class="sxs-lookup"><span data-stu-id="2a436-156">Relationships</span></span>
| <span data-ttu-id="2a436-157">Связь</span><span class="sxs-lookup"><span data-stu-id="2a436-157">Relationship</span></span> | <span data-ttu-id="2a436-158">Тип</span><span class="sxs-lookup"><span data-stu-id="2a436-158">Type</span></span>        | <span data-ttu-id="2a436-159">Описание</span><span class="sxs-lookup"><span data-stu-id="2a436-159">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2a436-160">createdBy</span><span class="sxs-lookup"><span data-stu-id="2a436-160">createdBy</span></span>|[<span data-ttu-id="2a436-161">userIdentity</span><span class="sxs-lookup"><span data-stu-id="2a436-161">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="2a436-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a436-162">Read-only.</span></span> <span data-ttu-id="2a436-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2a436-163">Nullable.</span></span>|
|<span data-ttu-id="2a436-164">documents</span><span class="sxs-lookup"><span data-stu-id="2a436-164">documents</span></span>|<span data-ttu-id="2a436-165">[Коллекция printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="2a436-165">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="2a436-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a436-166">Read-only.</span></span>|
|<span data-ttu-id="2a436-167">tasks</span><span class="sxs-lookup"><span data-stu-id="2a436-167">tasks</span></span>|<span data-ttu-id="2a436-168">[Коллекция printTask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="2a436-168">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="2a436-169">Список [printTasks,](printtask.md) которые были инициированы этим заданием печати.</span><span class="sxs-lookup"><span data-stu-id="2a436-169">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a436-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a436-170">JSON representation</span></span>

<span data-ttu-id="2a436-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a436-171">The following is a JSON representation of the resource.</span></span>

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

