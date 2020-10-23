---
title: Тип ресурса printJob
description: Представляет задание печати, помещенное в очередь для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7810c8cd864020c42de4482deea67620950f6cf0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726306"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="38aa0-103">Тип ресурса printJob</span><span class="sxs-lookup"><span data-stu-id="38aa0-103">printJob resource type</span></span>

<span data-ttu-id="38aa0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38aa0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38aa0-105">Представляет задание печати, помещенное в очередь для принтера.</span><span class="sxs-lookup"><span data-stu-id="38aa0-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="38aa0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="38aa0-106">Methods</span></span>

| <span data-ttu-id="38aa0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="38aa0-107">Method</span></span>       | <span data-ttu-id="38aa0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="38aa0-108">Return Type</span></span> | <span data-ttu-id="38aa0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="38aa0-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="38aa0-110">[получение](../api/printjob-get.md);</span><span class="sxs-lookup"><span data-stu-id="38aa0-110">[Get](../api/printjob-get.md)</span></span> | [<span data-ttu-id="38aa0-111">printJob</span><span class="sxs-lookup"><span data-stu-id="38aa0-111">printJob</span></span>](printjob.md) | <span data-ttu-id="38aa0-112">Чтение свойств и связей объекта printJob.</span><span class="sxs-lookup"><span data-stu-id="38aa0-112">Read properties and relationships of printJob object.</span></span> |
| <span data-ttu-id="38aa0-113">[создание](../api/printer-post-jobs.md);</span><span class="sxs-lookup"><span data-stu-id="38aa0-113">[Create](../api/printer-post-jobs.md)</span></span> | [<span data-ttu-id="38aa0-114">printJob</span><span class="sxs-lookup"><span data-stu-id="38aa0-114">printJob</span></span>](printjob.md) | <span data-ttu-id="38aa0-115">Создание нового объекта задания печати.</span><span class="sxs-lookup"><span data-stu-id="38aa0-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="38aa0-116">Начало</span><span class="sxs-lookup"><span data-stu-id="38aa0-116">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="38aa0-117">Нет</span><span class="sxs-lookup"><span data-stu-id="38aa0-117">None</span></span>|<span data-ttu-id="38aa0-118">Запустите задание печати.</span><span class="sxs-lookup"><span data-stu-id="38aa0-118">Start the print job.</span></span>|
| [<span data-ttu-id="38aa0-119">Отмена</span><span class="sxs-lookup"><span data-stu-id="38aa0-119">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="38aa0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="38aa0-120">None</span></span>|<span data-ttu-id="38aa0-121">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="38aa0-121">Cancel the print job.</span></span>|
| [<span data-ttu-id="38aa0-122">Перенаправление (на другой принтер)</span><span class="sxs-lookup"><span data-stu-id="38aa0-122">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="38aa0-123">printJob</span><span class="sxs-lookup"><span data-stu-id="38aa0-123">printJob</span></span>](printjob.md) | <span data-ttu-id="38aa0-124">Задание печати, помещенное в очередь для конечного принтера.</span><span class="sxs-lookup"><span data-stu-id="38aa0-124">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="38aa0-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="38aa0-125">Properties</span></span>
| <span data-ttu-id="38aa0-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="38aa0-126">Property</span></span>     | <span data-ttu-id="38aa0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="38aa0-127">Type</span></span>        | <span data-ttu-id="38aa0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="38aa0-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="38aa0-129">id</span><span class="sxs-lookup"><span data-stu-id="38aa0-129">id</span></span>|<span data-ttu-id="38aa0-130">Строка</span><span class="sxs-lookup"><span data-stu-id="38aa0-130">String</span></span>|<span data-ttu-id="38aa0-131">GUID принтера.</span><span class="sxs-lookup"><span data-stu-id="38aa0-131">The printer's GUID.</span></span> <span data-ttu-id="38aa0-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38aa0-132">Read-only.</span></span>|
|<span data-ttu-id="38aa0-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38aa0-133">createdDateTime</span></span>|<span data-ttu-id="38aa0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38aa0-134">DateTimeOffset</span></span>|<span data-ttu-id="38aa0-135">Значение DateTimeOffset при создании задания.</span><span class="sxs-lookup"><span data-stu-id="38aa0-135">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="38aa0-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38aa0-136">Read-only.</span></span>|
|<span data-ttu-id="38aa0-137">status</span><span class="sxs-lookup"><span data-stu-id="38aa0-137">status</span></span>|[<span data-ttu-id="38aa0-138">принтжобстатус</span><span class="sxs-lookup"><span data-stu-id="38aa0-138">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="38aa0-139">Состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="38aa0-139">The status of the print job.</span></span> <span data-ttu-id="38aa0-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38aa0-140">Read-only.</span></span>|
|<span data-ttu-id="38aa0-141">configuration</span><span class="sxs-lookup"><span data-stu-id="38aa0-141">configuration</span></span>|[<span data-ttu-id="38aa0-142">принтжобконфигуратион</span><span class="sxs-lookup"><span data-stu-id="38aa0-142">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="38aa0-143">Группа параметров, которые принтер должен использовать для печати задания.</span><span class="sxs-lookup"><span data-stu-id="38aa0-143">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="38aa0-144">подбираемый</span><span class="sxs-lookup"><span data-stu-id="38aa0-144">isFetchable</span></span>|<span data-ttu-id="38aa0-145">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="38aa0-145">Edm.Boolean</span></span>|<span data-ttu-id="38aa0-146">Если этот параметр имеет значение true, документ может быть извлечен принтером.</span><span class="sxs-lookup"><span data-stu-id="38aa0-146">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="38aa0-147">редиректедфром</span><span class="sxs-lookup"><span data-stu-id="38aa0-147">redirectedFrom</span></span>|<span data-ttu-id="38aa0-148">Edm.String</span><span class="sxs-lookup"><span data-stu-id="38aa0-148">Edm.String</span></span>|<span data-ttu-id="38aa0-149">Содержит URL-адрес исходного задания, если задание было перенаправлено с другого принтера.</span><span class="sxs-lookup"><span data-stu-id="38aa0-149">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="38aa0-150">редиректедто</span><span class="sxs-lookup"><span data-stu-id="38aa0-150">redirectedTo</span></span>|<span data-ttu-id="38aa0-151">Edm.String</span><span class="sxs-lookup"><span data-stu-id="38aa0-151">Edm.String</span></span>|<span data-ttu-id="38aa0-152">Содержит URL-адрес конечного задания, если задание было перенаправлено на другой принтер.</span><span class="sxs-lookup"><span data-stu-id="38aa0-152">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38aa0-153">Связи</span><span class="sxs-lookup"><span data-stu-id="38aa0-153">Relationships</span></span>
| <span data-ttu-id="38aa0-154">Связь</span><span class="sxs-lookup"><span data-stu-id="38aa0-154">Relationship</span></span> | <span data-ttu-id="38aa0-155">Тип</span><span class="sxs-lookup"><span data-stu-id="38aa0-155">Type</span></span>        | <span data-ttu-id="38aa0-156">Описание</span><span class="sxs-lookup"><span data-stu-id="38aa0-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="38aa0-157">createdBy</span><span class="sxs-lookup"><span data-stu-id="38aa0-157">createdBy</span></span>|[<span data-ttu-id="38aa0-158">userIdentity</span><span class="sxs-lookup"><span data-stu-id="38aa0-158">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="38aa0-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38aa0-159">Read-only.</span></span> <span data-ttu-id="38aa0-160">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="38aa0-160">Nullable.</span></span>|
|<span data-ttu-id="38aa0-161">настоящему</span><span class="sxs-lookup"><span data-stu-id="38aa0-161">documents</span></span>|<span data-ttu-id="38aa0-162">Коллекция [printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="38aa0-162">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="38aa0-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38aa0-163">Read-only.</span></span>|
|<span data-ttu-id="38aa0-164">tasks</span><span class="sxs-lookup"><span data-stu-id="38aa0-164">tasks</span></span>|<span data-ttu-id="38aa0-165">Коллекция [принттаск](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="38aa0-165">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="38aa0-166">Список [принттаскс](printtask.md) , которые были активированы этим заданием печати.</span><span class="sxs-lookup"><span data-stu-id="38aa0-166">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38aa0-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38aa0-167">JSON representation</span></span>

<span data-ttu-id="38aa0-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38aa0-168">The following is a JSON representation of the resource.</span></span>

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

