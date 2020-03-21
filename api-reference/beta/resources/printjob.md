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
# <a name="printjob-resource-type"></a><span data-ttu-id="da32a-103">Тип ресурса printJob</span><span class="sxs-lookup"><span data-stu-id="da32a-103">printJob resource type</span></span>

<span data-ttu-id="da32a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da32a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da32a-105">Представляет задание печати, помещенное в очередь для принтера.</span><span class="sxs-lookup"><span data-stu-id="da32a-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="da32a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="da32a-106">Methods</span></span>

| <span data-ttu-id="da32a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="da32a-107">Method</span></span>       | <span data-ttu-id="da32a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="da32a-108">Return Type</span></span> | <span data-ttu-id="da32a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="da32a-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="da32a-110">[получение](../api/printjob-get.md);</span><span class="sxs-lookup"><span data-stu-id="da32a-110">[Get](../api/printjob-get.md)</span></span> | [<span data-ttu-id="da32a-111">printJob</span><span class="sxs-lookup"><span data-stu-id="da32a-111">printJob</span></span>](printjob.md) | <span data-ttu-id="da32a-112">Чтение свойств и связей объекта printJob.</span><span class="sxs-lookup"><span data-stu-id="da32a-112">Read properties and relationships of printJob object.</span></span> |
| <span data-ttu-id="da32a-113">[создание](../api/printer-post-jobs.md);</span><span class="sxs-lookup"><span data-stu-id="da32a-113">[Create](../api/printer-post-jobs.md)</span></span> | [<span data-ttu-id="da32a-114">printJob</span><span class="sxs-lookup"><span data-stu-id="da32a-114">printJob</span></span>](printjob.md) | <span data-ttu-id="da32a-115">Создание нового объекта задания печати.</span><span class="sxs-lookup"><span data-stu-id="da32a-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="da32a-116">Начало</span><span class="sxs-lookup"><span data-stu-id="da32a-116">Start</span></span>](../api/printjob-startprintjob.md)|<span data-ttu-id="da32a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="da32a-117">None</span></span>|<span data-ttu-id="da32a-118">Запустите задание печати.</span><span class="sxs-lookup"><span data-stu-id="da32a-118">Start the print job.</span></span>|
| [<span data-ttu-id="da32a-119">Отмена</span><span class="sxs-lookup"><span data-stu-id="da32a-119">Cancel</span></span>](../api/printjob-cancelprintjob.md)|<span data-ttu-id="da32a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="da32a-120">None</span></span>|<span data-ttu-id="da32a-121">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="da32a-121">Cancel the print job.</span></span>|

## <a name="properties"></a><span data-ttu-id="da32a-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="da32a-122">Properties</span></span>
| <span data-ttu-id="da32a-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="da32a-123">Property</span></span>     | <span data-ttu-id="da32a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="da32a-124">Type</span></span>        | <span data-ttu-id="da32a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="da32a-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da32a-126">id</span><span class="sxs-lookup"><span data-stu-id="da32a-126">id</span></span>|<span data-ttu-id="da32a-127">String</span><span class="sxs-lookup"><span data-stu-id="da32a-127">String</span></span>|<span data-ttu-id="da32a-128">GUID принтера.</span><span class="sxs-lookup"><span data-stu-id="da32a-128">The printer's GUID.</span></span> <span data-ttu-id="da32a-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da32a-129">Read-only.</span></span>|
|<span data-ttu-id="da32a-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da32a-130">createdDateTime</span></span>|<span data-ttu-id="da32a-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da32a-131">DateTimeOffset</span></span>|<span data-ttu-id="da32a-132">Значение DateTimeOffset при создании задания.</span><span class="sxs-lookup"><span data-stu-id="da32a-132">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="da32a-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da32a-133">Read-only.</span></span>|
|<span data-ttu-id="da32a-134">status</span><span class="sxs-lookup"><span data-stu-id="da32a-134">status</span></span>|[<span data-ttu-id="da32a-135">принтжобстатус</span><span class="sxs-lookup"><span data-stu-id="da32a-135">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="da32a-136">Состояние задания печати.</span><span class="sxs-lookup"><span data-stu-id="da32a-136">The status of the print job.</span></span> <span data-ttu-id="da32a-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da32a-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da32a-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="da32a-138">Relationships</span></span>
| <span data-ttu-id="da32a-139">Связь</span><span class="sxs-lookup"><span data-stu-id="da32a-139">Relationship</span></span> | <span data-ttu-id="da32a-140">Тип</span><span class="sxs-lookup"><span data-stu-id="da32a-140">Type</span></span>        | <span data-ttu-id="da32a-141">Описание</span><span class="sxs-lookup"><span data-stu-id="da32a-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da32a-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="da32a-142">createdBy</span></span>|[<span data-ttu-id="da32a-143">userIdentity</span><span class="sxs-lookup"><span data-stu-id="da32a-143">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="da32a-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da32a-144">Read-only.</span></span> <span data-ttu-id="da32a-145">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="da32a-145">Nullable.</span></span>|
|<span data-ttu-id="da32a-146">настоящему</span><span class="sxs-lookup"><span data-stu-id="da32a-146">documents</span></span>|<span data-ttu-id="da32a-147">Коллекция [printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="da32a-147">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="da32a-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da32a-148">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da32a-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da32a-149">JSON representation</span></span>

<span data-ttu-id="da32a-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da32a-150">The following is a JSON representation of the resource.</span></span>

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