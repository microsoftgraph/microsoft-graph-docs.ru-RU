---
title: Тип ресурса Принттаск
description: Представляет задачу, которая выполняется или была выполнена в результате универсального события печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fb41bc68112aa04e1eea825d45982f2f3f0db48c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973794"
---
# <a name="printtask-resource-type"></a><span data-ttu-id="8a0f3-103">Тип ресурса Принттаск</span><span class="sxs-lookup"><span data-stu-id="8a0f3-103">printTask resource type</span></span>

<span data-ttu-id="8a0f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a0f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a0f3-105">Представляет задачу, которая выполняется или была выполнена в результате универсального события печати.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-105">Represents a task that is executing or has been executed as a result of a Universal Print event.</span></span>

<span data-ttu-id="8a0f3-106">Дополнительные сведения о том, как использовать этот ресурс для поддержки печати по запросу в универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="8a0f3-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="8a0f3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8a0f3-107">Methods</span></span>

| <span data-ttu-id="8a0f3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8a0f3-108">Method</span></span>       | <span data-ttu-id="8a0f3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a0f3-109">Return Type</span></span> | <span data-ttu-id="8a0f3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0f3-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8a0f3-111">Список (из Принттаскдефинтион)</span><span class="sxs-lookup"><span data-stu-id="8a0f3-111">List (from printTaskDefintion)</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="8a0f3-112">printTask</span><span class="sxs-lookup"><span data-stu-id="8a0f3-112">printTask</span></span>](printtask.md) | <span data-ttu-id="8a0f3-113">Получение списка задач, созданных на основе определенного Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-113">Get a list of tasks that have been created based on a particular printTaskDefinition.</span></span> <span data-ttu-id="8a0f3-114">Список содержит текущие выполняемые задачи и недавно выполненные задачи.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-114">The list includes currently running tasks and recently completed tasks.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a0f3-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a0f3-115">Properties</span></span>
| <span data-ttu-id="8a0f3-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a0f3-116">Property</span></span>     | <span data-ttu-id="8a0f3-117">Тип</span><span class="sxs-lookup"><span data-stu-id="8a0f3-117">Type</span></span>        | <span data-ttu-id="8a0f3-118">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0f3-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a0f3-119">id</span><span class="sxs-lookup"><span data-stu-id="8a0f3-119">id</span></span>|<span data-ttu-id="8a0f3-120">String</span><span class="sxs-lookup"><span data-stu-id="8a0f3-120">String</span></span>|<span data-ttu-id="8a0f3-121">Идентификатор Принттаск.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-121">The printTask's identifier.</span></span> <span data-ttu-id="8a0f3-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-122">Read-only.</span></span>|
|<span data-ttu-id="8a0f3-123">status</span><span class="sxs-lookup"><span data-stu-id="8a0f3-123">status</span></span>|[<span data-ttu-id="8a0f3-124">printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="8a0f3-124">printTaskStatus</span></span>](printtaskstatus.md)|<span data-ttu-id="8a0f3-125">Текущее состояние выполнения этого Принттаск.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-125">The current execution status of this printTask.</span></span> <span data-ttu-id="8a0f3-126">**Вызывающее приложение несет ответственность за обновление этого состояния после завершения обработки, если связанный с ним метод printJob не будет перенаправлен на другой принтер.**</span><span class="sxs-lookup"><span data-stu-id="8a0f3-126">**The calling application is responsible for updating this status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="8a0f3-127">Если не выполнить отчет о завершении, то соответствующее задание печати блокируется для печати и в конечном итоге удалено.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-127">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |
|<span data-ttu-id="8a0f3-128">parentUrl</span><span class="sxs-lookup"><span data-stu-id="8a0f3-128">parentUrl</span></span>|<span data-ttu-id="8a0f3-129">String</span><span class="sxs-lookup"><span data-stu-id="8a0f3-129">String</span></span>|<span data-ttu-id="8a0f3-130">URL-адрес объекта печати, который инициировал эту задачу.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-130">The URL for the print entity that triggered this task.</span></span> <span data-ttu-id="8a0f3-131">Например, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-131">For example, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span></span> <span data-ttu-id="8a0f3-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a0f3-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="8a0f3-133">Relationships</span></span>
| <span data-ttu-id="8a0f3-134">Связь</span><span class="sxs-lookup"><span data-stu-id="8a0f3-134">Relationship</span></span> | <span data-ttu-id="8a0f3-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8a0f3-135">Type</span></span>        | <span data-ttu-id="8a0f3-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0f3-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a0f3-137">активирован</span><span class="sxs-lookup"><span data-stu-id="8a0f3-137">trigger</span></span>|[<span data-ttu-id="8a0f3-138">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="8a0f3-138">printTaskTrigger</span></span>](printtasktrigger.md)|<span data-ttu-id="8a0f3-139">Принттасктригжер, который инициировал выполнение этой задачи.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-139">The printTaskTrigger that triggered this task's execution.</span></span> <span data-ttu-id="8a0f3-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-140">Read-only.</span></span>|
|<span data-ttu-id="8a0f3-141">RDLC</span><span class="sxs-lookup"><span data-stu-id="8a0f3-141">definition</span></span>|[<span data-ttu-id="8a0f3-142">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="8a0f3-142">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="8a0f3-143">Принттаскдефинитион, который использовался для создания этой задачи.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-143">The printTaskDefinition that was used to create this task.</span></span> <span data-ttu-id="8a0f3-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-144">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a0f3-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a0f3-145">JSON representation</span></span>

<span data-ttu-id="8a0f3-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a0f3-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTask",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.printTaskStatus"},
  "parentUrl": "String",
  "trigger": {"@odata.type": "microsoft.graph.printTaskTrigger"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


