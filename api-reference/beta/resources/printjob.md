---
title: Тип ресурса printJob
description: Представляет задание печати, помещенное в очередь для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5eff75fba2c9993275c277877fedec7705021c49
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896005"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="0e98d-103">Тип ресурса printJob</span><span class="sxs-lookup"><span data-stu-id="0e98d-103">printJob resource type</span></span>

<span data-ttu-id="0e98d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e98d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e98d-105">Представляет задание печати, помещенное в очередь для принтера.</span><span class="sxs-lookup"><span data-stu-id="0e98d-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="0e98d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0e98d-106">Methods</span></span>

| <span data-ttu-id="0e98d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0e98d-107">Method</span></span>       | <span data-ttu-id="0e98d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0e98d-108">Return Type</span></span> | <span data-ttu-id="0e98d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0e98d-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0e98d-110">[получение](../api/printjob-get.md);</span><span class="sxs-lookup"><span data-stu-id="0e98d-110">[Get](../api/printjob-get.md)</span></span> | [<span data-ttu-id="0e98d-111">printJob</span><span class="sxs-lookup"><span data-stu-id="0e98d-111">printJob</span></span>](printjob.md) | <span data-ttu-id="0e98d-112">Чтение свойств и связей объекта printJob.</span><span class="sxs-lookup"><span data-stu-id="0e98d-112">Read properties and relationships of printJob object.</span></span> |
| <span data-ttu-id="0e98d-113">[создание](../api/printer-post-jobs.md);</span><span class="sxs-lookup"><span data-stu-id="0e98d-113">[Create](../api/printer-post-jobs.md)</span></span> | [<span data-ttu-id="0e98d-114">printJob</span><span class="sxs-lookup"><span data-stu-id="0e98d-114">printJob</span></span>](printjob.md) | <span data-ttu-id="0e98d-115">Создание нового объекта задания печати.</span><span class="sxs-lookup"><span data-stu-id="0e98d-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="0e98d-116">Начало</span><span class="sxs-lookup"><span data-stu-id="0e98d-116">Start</span></span>](../api/printjob-startprintjob.md)|<span data-ttu-id="0e98d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="0e98d-117">None</span></span>|<span data-ttu-id="0e98d-118">Запустите задание печати.</span><span class="sxs-lookup"><span data-stu-id="0e98d-118">Start the print job.</span></span>|
| [<span data-ttu-id="0e98d-119">Отмена</span><span class="sxs-lookup"><span data-stu-id="0e98d-119">Cancel</span></span>](../api/printjob-cancelprintjob.md)|<span data-ttu-id="0e98d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="0e98d-120">None</span></span>|<span data-ttu-id="0e98d-121">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="0e98d-121">Cancel the print job.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e98d-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e98d-122">Properties</span></span>
| <span data-ttu-id="0e98d-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e98d-123">Property</span></span>     | <span data-ttu-id="0e98d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="0e98d-124">Type</span></span>        | <span data-ttu-id="0e98d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0e98d-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e98d-126">id</span><span class="sxs-lookup"><span data-stu-id="0e98d-126">id</span></span>|<span data-ttu-id="0e98d-127">String</span><span class="sxs-lookup"><span data-stu-id="0e98d-127">String</span></span>|<span data-ttu-id="0e98d-128">GUID принтера.</span><span class="sxs-lookup"><span data-stu-id="0e98d-128">The printer's GUID.</span></span> <span data-ttu-id="0e98d-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e98d-129">Read-only.</span></span>|
|<span data-ttu-id="0e98d-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e98d-130">createdDateTime</span></span>|<span data-ttu-id="0e98d-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e98d-131">DateTimeOffset</span></span>|<span data-ttu-id="0e98d-132">Значение DateTimeOffset при создании задания.</span><span class="sxs-lookup"><span data-stu-id="0e98d-132">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="0e98d-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e98d-133">Read-only.</span></span>|
|<span data-ttu-id="0e98d-134">status</span><span class="sxs-lookup"><span data-stu-id="0e98d-134">status</span></span>|[<span data-ttu-id="0e98d-135">принтжобстатус</span><span class="sxs-lookup"><span data-stu-id="0e98d-135">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="0e98d-136">Состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="0e98d-136">The status of the print job.</span></span> <span data-ttu-id="0e98d-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e98d-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e98d-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="0e98d-138">Relationships</span></span>
| <span data-ttu-id="0e98d-139">Связь</span><span class="sxs-lookup"><span data-stu-id="0e98d-139">Relationship</span></span> | <span data-ttu-id="0e98d-140">Тип</span><span class="sxs-lookup"><span data-stu-id="0e98d-140">Type</span></span>        | <span data-ttu-id="0e98d-141">Описание</span><span class="sxs-lookup"><span data-stu-id="0e98d-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e98d-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="0e98d-142">createdBy</span></span>|[<span data-ttu-id="0e98d-143">userIdentity</span><span class="sxs-lookup"><span data-stu-id="0e98d-143">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="0e98d-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e98d-144">Read-only.</span></span> <span data-ttu-id="0e98d-145">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0e98d-145">Nullable.</span></span>|
|<span data-ttu-id="0e98d-146">настоящему</span><span class="sxs-lookup"><span data-stu-id="0e98d-146">documents</span></span>|<span data-ttu-id="0e98d-147">Коллекция [printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="0e98d-147">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="0e98d-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e98d-148">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e98d-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e98d-149">JSON representation</span></span>

<span data-ttu-id="0e98d-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e98d-150">The following is a JSON representation of the resource.</span></span>

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