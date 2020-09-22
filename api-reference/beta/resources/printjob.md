---
title: Тип ресурса printJob
description: Представляет задание печати, помещенное в очередь для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2c0a1bdb4ec3ebe3c87b5b40595d30cf9108c5bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048743"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="f970c-103">Тип ресурса printJob</span><span class="sxs-lookup"><span data-stu-id="f970c-103">printJob resource type</span></span>

<span data-ttu-id="f970c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f970c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f970c-105">Представляет задание печати, помещенное в очередь для принтера.</span><span class="sxs-lookup"><span data-stu-id="f970c-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="f970c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f970c-106">Methods</span></span>

| <span data-ttu-id="f970c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f970c-107">Method</span></span>       | <span data-ttu-id="f970c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f970c-108">Return Type</span></span> | <span data-ttu-id="f970c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f970c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f970c-110">Получение</span><span class="sxs-lookup"><span data-stu-id="f970c-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="f970c-111">printJob</span><span class="sxs-lookup"><span data-stu-id="f970c-111">printJob</span></span>](printjob.md) | <span data-ttu-id="f970c-112">Чтение свойств и связей объекта printJob.</span><span class="sxs-lookup"><span data-stu-id="f970c-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="f970c-113">Создание</span><span class="sxs-lookup"><span data-stu-id="f970c-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="f970c-114">printJob</span><span class="sxs-lookup"><span data-stu-id="f970c-114">printJob</span></span>](printjob.md) | <span data-ttu-id="f970c-115">Создание нового объекта задания печати.</span><span class="sxs-lookup"><span data-stu-id="f970c-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="f970c-116">Начало</span><span class="sxs-lookup"><span data-stu-id="f970c-116">Start</span></span>](../api/printjob-startprintjob.md)|<span data-ttu-id="f970c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f970c-117">None</span></span>|<span data-ttu-id="f970c-118">Запустите задание печати.</span><span class="sxs-lookup"><span data-stu-id="f970c-118">Start the print job.</span></span>|
| [<span data-ttu-id="f970c-119">Отмена</span><span class="sxs-lookup"><span data-stu-id="f970c-119">Cancel</span></span>](../api/printjob-cancelprintjob.md)|<span data-ttu-id="f970c-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f970c-120">None</span></span>|<span data-ttu-id="f970c-121">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="f970c-121">Cancel the print job.</span></span>|
| [<span data-ttu-id="f970c-122">Перенаправление (на другой принтер)</span><span class="sxs-lookup"><span data-stu-id="f970c-122">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="f970c-123">printJob</span><span class="sxs-lookup"><span data-stu-id="f970c-123">printJob</span></span>](printjob.md) | <span data-ttu-id="f970c-124">Задание печати, помещенное в очередь для конечного принтера.</span><span class="sxs-lookup"><span data-stu-id="f970c-124">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="f970c-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="f970c-125">Properties</span></span>
| <span data-ttu-id="f970c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f970c-126">Property</span></span>     | <span data-ttu-id="f970c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f970c-127">Type</span></span>        | <span data-ttu-id="f970c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f970c-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f970c-129">id</span><span class="sxs-lookup"><span data-stu-id="f970c-129">id</span></span>|<span data-ttu-id="f970c-130">Строка</span><span class="sxs-lookup"><span data-stu-id="f970c-130">String</span></span>|<span data-ttu-id="f970c-131">GUID принтера.</span><span class="sxs-lookup"><span data-stu-id="f970c-131">The printer's GUID.</span></span> <span data-ttu-id="f970c-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f970c-132">Read-only.</span></span>|
|<span data-ttu-id="f970c-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f970c-133">createdDateTime</span></span>|<span data-ttu-id="f970c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f970c-134">DateTimeOffset</span></span>|<span data-ttu-id="f970c-135">Значение DateTimeOffset при создании задания.</span><span class="sxs-lookup"><span data-stu-id="f970c-135">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="f970c-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f970c-136">Read-only.</span></span>|
|<span data-ttu-id="f970c-137">status</span><span class="sxs-lookup"><span data-stu-id="f970c-137">status</span></span>|[<span data-ttu-id="f970c-138">принтжобстатус</span><span class="sxs-lookup"><span data-stu-id="f970c-138">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="f970c-139">Состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="f970c-139">The status of the print job.</span></span> <span data-ttu-id="f970c-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f970c-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f970c-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="f970c-141">Relationships</span></span>
| <span data-ttu-id="f970c-142">Связь</span><span class="sxs-lookup"><span data-stu-id="f970c-142">Relationship</span></span> | <span data-ttu-id="f970c-143">Тип</span><span class="sxs-lookup"><span data-stu-id="f970c-143">Type</span></span>        | <span data-ttu-id="f970c-144">Описание</span><span class="sxs-lookup"><span data-stu-id="f970c-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f970c-145">createdBy</span><span class="sxs-lookup"><span data-stu-id="f970c-145">createdBy</span></span>|[<span data-ttu-id="f970c-146">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f970c-146">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="f970c-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f970c-147">Read-only.</span></span> <span data-ttu-id="f970c-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f970c-148">Nullable.</span></span>|
|<span data-ttu-id="f970c-149">настоящему</span><span class="sxs-lookup"><span data-stu-id="f970c-149">documents</span></span>|<span data-ttu-id="f970c-150">Коллекция [printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="f970c-150">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="f970c-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f970c-151">Read-only.</span></span>|
|<span data-ttu-id="f970c-152">tasks</span><span class="sxs-lookup"><span data-stu-id="f970c-152">tasks</span></span>|<span data-ttu-id="f970c-153">Коллекция [принттаск](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="f970c-153">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="f970c-154">Список [принттаскс](printtask.md) , которые были активированы этим заданием печати.</span><span class="sxs-lookup"><span data-stu-id="f970c-154">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f970c-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f970c-155">JSON representation</span></span>

<span data-ttu-id="f970c-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f970c-156">The following is a JSON representation of the resource.</span></span>

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
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
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

