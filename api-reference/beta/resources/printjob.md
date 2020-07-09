---
title: Тип ресурса printJob
description: Представляет задание печати, помещенное в очередь для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0d46263e5f393362cec155a9be3e2e5a54c3dfec
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091524"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="a51df-103">Тип ресурса printJob</span><span class="sxs-lookup"><span data-stu-id="a51df-103">printJob resource type</span></span>

<span data-ttu-id="a51df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a51df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a51df-105">Представляет задание печати, помещенное в очередь для принтера.</span><span class="sxs-lookup"><span data-stu-id="a51df-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="a51df-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a51df-106">Methods</span></span>

| <span data-ttu-id="a51df-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a51df-107">Method</span></span>       | <span data-ttu-id="a51df-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a51df-108">Return Type</span></span> | <span data-ttu-id="a51df-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a51df-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a51df-110">[получение](../api/printjob-get.md);</span><span class="sxs-lookup"><span data-stu-id="a51df-110">[Get](../api/printjob-get.md)</span></span> | [<span data-ttu-id="a51df-111">printJob</span><span class="sxs-lookup"><span data-stu-id="a51df-111">printJob</span></span>](printjob.md) | <span data-ttu-id="a51df-112">Чтение свойств и связей объекта printJob.</span><span class="sxs-lookup"><span data-stu-id="a51df-112">Read properties and relationships of printJob object.</span></span> |
| <span data-ttu-id="a51df-113">[Создание](../api/printer-post-jobs.md);</span><span class="sxs-lookup"><span data-stu-id="a51df-113">[Create](../api/printer-post-jobs.md)</span></span> | [<span data-ttu-id="a51df-114">printJob</span><span class="sxs-lookup"><span data-stu-id="a51df-114">printJob</span></span>](printjob.md) | <span data-ttu-id="a51df-115">Создание нового объекта задания печати.</span><span class="sxs-lookup"><span data-stu-id="a51df-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="a51df-116">Начало</span><span class="sxs-lookup"><span data-stu-id="a51df-116">Start</span></span>](../api/printjob-startprintjob.md)|<span data-ttu-id="a51df-117">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="a51df-117">None</span></span>|<span data-ttu-id="a51df-118">Запустите задание печати.</span><span class="sxs-lookup"><span data-stu-id="a51df-118">Start the print job.</span></span>|
| [<span data-ttu-id="a51df-119">Отмена</span><span class="sxs-lookup"><span data-stu-id="a51df-119">Cancel</span></span>](../api/printjob-cancelprintjob.md)|<span data-ttu-id="a51df-120">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="a51df-120">None</span></span>|<span data-ttu-id="a51df-121">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="a51df-121">Cancel the print job.</span></span>|
| [<span data-ttu-id="a51df-122">Перенаправление (на другой принтер)</span><span class="sxs-lookup"><span data-stu-id="a51df-122">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="a51df-123">printJob</span><span class="sxs-lookup"><span data-stu-id="a51df-123">printJob</span></span>](printjob.md) | <span data-ttu-id="a51df-124">Задание печати, помещенное в очередь для конечного принтера.</span><span class="sxs-lookup"><span data-stu-id="a51df-124">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="a51df-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="a51df-125">Properties</span></span>
| <span data-ttu-id="a51df-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a51df-126">Property</span></span>     | <span data-ttu-id="a51df-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a51df-127">Type</span></span>        | <span data-ttu-id="a51df-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a51df-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a51df-129">id</span><span class="sxs-lookup"><span data-stu-id="a51df-129">id</span></span>|<span data-ttu-id="a51df-130">String</span><span class="sxs-lookup"><span data-stu-id="a51df-130">String</span></span>|<span data-ttu-id="a51df-131">GUID принтера.</span><span class="sxs-lookup"><span data-stu-id="a51df-131">The printer's GUID.</span></span> <span data-ttu-id="a51df-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a51df-132">Read-only.</span></span>|
|<span data-ttu-id="a51df-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a51df-133">createdDateTime</span></span>|<span data-ttu-id="a51df-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a51df-134">DateTimeOffset</span></span>|<span data-ttu-id="a51df-135">Значение DateTimeOffset при создании задания.</span><span class="sxs-lookup"><span data-stu-id="a51df-135">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="a51df-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a51df-136">Read-only.</span></span>|
|<span data-ttu-id="a51df-137">status</span><span class="sxs-lookup"><span data-stu-id="a51df-137">status</span></span>|[<span data-ttu-id="a51df-138">принтжобстатус</span><span class="sxs-lookup"><span data-stu-id="a51df-138">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="a51df-139">Состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="a51df-139">The status of the print job.</span></span> <span data-ttu-id="a51df-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a51df-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a51df-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="a51df-141">Relationships</span></span>
| <span data-ttu-id="a51df-142">Связь</span><span class="sxs-lookup"><span data-stu-id="a51df-142">Relationship</span></span> | <span data-ttu-id="a51df-143">Тип</span><span class="sxs-lookup"><span data-stu-id="a51df-143">Type</span></span>        | <span data-ttu-id="a51df-144">Описание</span><span class="sxs-lookup"><span data-stu-id="a51df-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a51df-145">createdBy</span><span class="sxs-lookup"><span data-stu-id="a51df-145">createdBy</span></span>|[<span data-ttu-id="a51df-146">userIdentity</span><span class="sxs-lookup"><span data-stu-id="a51df-146">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="a51df-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a51df-147">Read-only.</span></span> <span data-ttu-id="a51df-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a51df-148">Nullable.</span></span>|
|<span data-ttu-id="a51df-149">настоящему</span><span class="sxs-lookup"><span data-stu-id="a51df-149">documents</span></span>|<span data-ttu-id="a51df-150">Коллекция [printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="a51df-150">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="a51df-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a51df-151">Read-only.</span></span>|
|<span data-ttu-id="a51df-152">tasks</span><span class="sxs-lookup"><span data-stu-id="a51df-152">tasks</span></span>|<span data-ttu-id="a51df-153">Коллекция [принттаск](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="a51df-153">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="a51df-154">Список [принттаскс](printtask.md) , которые были активированы этим заданием печати.</span><span class="sxs-lookup"><span data-stu-id="a51df-154">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a51df-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a51df-155">JSON representation</span></span>

<span data-ttu-id="a51df-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a51df-156">The following is a JSON representation of the resource.</span></span>

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