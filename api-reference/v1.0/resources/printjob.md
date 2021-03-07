---
title: тип ресурса printJob
description: Представляет задание печати, которое выстроилось в очередь для принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 3115164fcc15ef6c2133ef3616624af9141da1af
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518068"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="3928b-103">тип ресурса printJob</span><span class="sxs-lookup"><span data-stu-id="3928b-103">printJob resource type</span></span>

<span data-ttu-id="3928b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3928b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="3928b-105">Представляет задание печати, которое выстроилось в очередь для принтера.</span><span class="sxs-lookup"><span data-stu-id="3928b-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="3928b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3928b-106">Methods</span></span>
| <span data-ttu-id="3928b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3928b-107">Method</span></span>       | <span data-ttu-id="3928b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3928b-108">Return Type</span></span> | <span data-ttu-id="3928b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3928b-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3928b-110">[получение](../api/printjob-get.md);</span><span class="sxs-lookup"><span data-stu-id="3928b-110">[Get](../api/printjob-get.md)</span></span> | [<span data-ttu-id="3928b-111">printJob</span><span class="sxs-lookup"><span data-stu-id="3928b-111">printJob</span></span>](printjob.md) | <span data-ttu-id="3928b-112">Чтение свойств и связей объекта printJob.</span><span class="sxs-lookup"><span data-stu-id="3928b-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="3928b-113">Создание</span><span class="sxs-lookup"><span data-stu-id="3928b-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="3928b-114">printJob</span><span class="sxs-lookup"><span data-stu-id="3928b-114">printJob</span></span>](printjob.md) | <span data-ttu-id="3928b-115">Создание нового объекта задания печати.</span><span class="sxs-lookup"><span data-stu-id="3928b-115">Create a new print job object.</span></span> |
| <span data-ttu-id="3928b-116">[обновление](../api/printjob-update.md).</span><span class="sxs-lookup"><span data-stu-id="3928b-116">[Update](../api/printjob-update.md)</span></span> | [<span data-ttu-id="3928b-117">printJob</span><span class="sxs-lookup"><span data-stu-id="3928b-117">printJob</span></span>](printjob.md) | <span data-ttu-id="3928b-118">Обновление объекта задания печати.</span><span class="sxs-lookup"><span data-stu-id="3928b-118">Update a print job object.</span></span> |
| [<span data-ttu-id="3928b-119">Начало</span><span class="sxs-lookup"><span data-stu-id="3928b-119">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="3928b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="3928b-120">None</span></span>|<span data-ttu-id="3928b-121">Запустите задание печати.</span><span class="sxs-lookup"><span data-stu-id="3928b-121">Start the print job.</span></span>|
| [<span data-ttu-id="3928b-122">Отмена</span><span class="sxs-lookup"><span data-stu-id="3928b-122">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="3928b-123">Нет</span><span class="sxs-lookup"><span data-stu-id="3928b-123">None</span></span>|<span data-ttu-id="3928b-124">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="3928b-124">Cancel the print job.</span></span>|
| [<span data-ttu-id="3928b-125">Прервать</span><span class="sxs-lookup"><span data-stu-id="3928b-125">Abort</span></span>](../api/printjob-abort.md)|<span data-ttu-id="3928b-126">Нет</span><span class="sxs-lookup"><span data-stu-id="3928b-126">None</span></span>|<span data-ttu-id="3928b-127">Прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="3928b-127">Abort the print job.</span></span>|
| [<span data-ttu-id="3928b-128">Перенаправление (на другой принтер)</span><span class="sxs-lookup"><span data-stu-id="3928b-128">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="3928b-129">printJob</span><span class="sxs-lookup"><span data-stu-id="3928b-129">printJob</span></span>](printjob.md) | <span data-ttu-id="3928b-130">Задание печати, которое находится в очереди для принтера назначения.</span><span class="sxs-lookup"><span data-stu-id="3928b-130">A print job that is queued for the destination printer.</span></span> |


## <a name="properties"></a><span data-ttu-id="3928b-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="3928b-131">Properties</span></span>
|<span data-ttu-id="3928b-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="3928b-132">Property</span></span>|<span data-ttu-id="3928b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="3928b-133">Type</span></span>|<span data-ttu-id="3928b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="3928b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3928b-135">id</span><span class="sxs-lookup"><span data-stu-id="3928b-135">id</span></span>|<span data-ttu-id="3928b-136">Строка</span><span class="sxs-lookup"><span data-stu-id="3928b-136">String</span></span>|<span data-ttu-id="3928b-137">GUID принтера.</span><span class="sxs-lookup"><span data-stu-id="3928b-137">The printer's GUID.</span></span> <span data-ttu-id="3928b-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3928b-138">Read-only.</span></span>|
|<span data-ttu-id="3928b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3928b-139">createdDateTime</span></span>|<span data-ttu-id="3928b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3928b-140">DateTimeOffset</span></span>|<span data-ttu-id="3928b-141">DateTimeOffset, когда задание было создано.</span><span class="sxs-lookup"><span data-stu-id="3928b-141">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="3928b-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3928b-142">Read-only.</span></span>|
|<span data-ttu-id="3928b-143">status</span><span class="sxs-lookup"><span data-stu-id="3928b-143">status</span></span>|[<span data-ttu-id="3928b-144">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="3928b-144">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="3928b-145">Состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="3928b-145">The status of the print job.</span></span> <span data-ttu-id="3928b-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3928b-146">Read-only.</span></span>|
|<span data-ttu-id="3928b-147">configuration</span><span class="sxs-lookup"><span data-stu-id="3928b-147">configuration</span></span>|[<span data-ttu-id="3928b-148">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="3928b-148">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="3928b-149">Группа параметров, которые принтер должен использовать для печати задания.</span><span class="sxs-lookup"><span data-stu-id="3928b-149">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="3928b-150">isFetchable</span><span class="sxs-lookup"><span data-stu-id="3928b-150">isFetchable</span></span>|<span data-ttu-id="3928b-151">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="3928b-151">Edm.Boolean</span></span>|<span data-ttu-id="3928b-152">Если это так, документ можно получить на принтере.</span><span class="sxs-lookup"><span data-stu-id="3928b-152">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="3928b-153">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="3928b-153">redirectedFrom</span></span>|<span data-ttu-id="3928b-154">Edm.String</span><span class="sxs-lookup"><span data-stu-id="3928b-154">Edm.String</span></span>|<span data-ttu-id="3928b-155">Содержит URL-адрес задания источника, если задание было перенаправлено с другого принтера.</span><span class="sxs-lookup"><span data-stu-id="3928b-155">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="3928b-156">redirectedTo</span><span class="sxs-lookup"><span data-stu-id="3928b-156">redirectedTo</span></span>|<span data-ttu-id="3928b-157">Edm.String</span><span class="sxs-lookup"><span data-stu-id="3928b-157">Edm.String</span></span>|<span data-ttu-id="3928b-158">Содержит URL-адрес задания назначения, если задание было перенаправлено на другой принтер.</span><span class="sxs-lookup"><span data-stu-id="3928b-158">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|
|<span data-ttu-id="3928b-159">createdBy</span><span class="sxs-lookup"><span data-stu-id="3928b-159">createdBy</span></span>|[<span data-ttu-id="3928b-160">userIdentity</span><span class="sxs-lookup"><span data-stu-id="3928b-160">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="3928b-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3928b-161">Read-only.</span></span> <span data-ttu-id="3928b-162">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3928b-162">Nullable.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3928b-163">Отношения</span><span class="sxs-lookup"><span data-stu-id="3928b-163">Relationships</span></span>
|<span data-ttu-id="3928b-164">Связь</span><span class="sxs-lookup"><span data-stu-id="3928b-164">Relationship</span></span>|<span data-ttu-id="3928b-165">Тип</span><span class="sxs-lookup"><span data-stu-id="3928b-165">Type</span></span>|<span data-ttu-id="3928b-166">Описание</span><span class="sxs-lookup"><span data-stu-id="3928b-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3928b-167">документы</span><span class="sxs-lookup"><span data-stu-id="3928b-167">documents</span></span>|<span data-ttu-id="3928b-168">[коллекция printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="3928b-168">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="3928b-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3928b-169">Read-only.</span></span>|
|<span data-ttu-id="3928b-170">tasks</span><span class="sxs-lookup"><span data-stu-id="3928b-170">tasks</span></span>|<span data-ttu-id="3928b-171">[printTask](printtask.md) collection</span><span class="sxs-lookup"><span data-stu-id="3928b-171">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="3928b-172">Список [printTasks,](printtask.md) которые были вызваны этим заданием печати.</span><span class="sxs-lookup"><span data-stu-id="3928b-172">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3928b-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3928b-173">JSON representation</span></span>
<span data-ttu-id="3928b-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3928b-174">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printJob",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJob",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "status": {
    "@odata.type": "microsoft.graph.printJobStatus"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "configuration": {
    "@odata.type": "microsoft.graph.printJobConfiguration"
  },
  "redirectedTo": "String",
  "redirectedFrom": "String",
  "isFetchable": "Boolean"
}
```

