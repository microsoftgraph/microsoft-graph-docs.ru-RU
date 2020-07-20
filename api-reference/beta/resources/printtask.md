---
title: Тип ресурса Принттаск
description: Представляет задачу, которая выполняется или была выполнена в результате универсального события печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 9700f81d2f3a1e488bf9c9c61da3d0f649f46194
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091753"
---
# <a name="printtask-resource-type"></a><span data-ttu-id="75631-103">Тип ресурса Принттаск</span><span class="sxs-lookup"><span data-stu-id="75631-103">printTask resource type</span></span>

<span data-ttu-id="75631-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75631-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75631-105">Представляет задачу, которая выполняется или была выполнена в результате универсального события печати.</span><span class="sxs-lookup"><span data-stu-id="75631-105">Represents a task that is executing or has been executed as a result of a Universal Print event.</span></span>

<span data-ttu-id="75631-106">Дополнительные сведения о том, как использовать этот ресурс для поддержки печати по запросу в универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="75631-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="75631-107">Методы</span><span class="sxs-lookup"><span data-stu-id="75631-107">Methods</span></span>

| <span data-ttu-id="75631-108">Метод</span><span class="sxs-lookup"><span data-stu-id="75631-108">Method</span></span>       | <span data-ttu-id="75631-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="75631-109">Return Type</span></span> | <span data-ttu-id="75631-110">Описание</span><span class="sxs-lookup"><span data-stu-id="75631-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="75631-111">Список (из Принттаскдефинтион)</span><span class="sxs-lookup"><span data-stu-id="75631-111">List (from printTaskDefintion)</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="75631-112">принттаск</span><span class="sxs-lookup"><span data-stu-id="75631-112">printTask</span></span>](printtask.md) | <span data-ttu-id="75631-113">Получение списка задач, созданных на основе определенного Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="75631-113">Get a list of tasks that have been created based on a particular printTaskDefinition.</span></span> <span data-ttu-id="75631-114">Список содержит текущие выполняемые задачи и недавно выполненные задачи.</span><span class="sxs-lookup"><span data-stu-id="75631-114">The list includes currently running tasks and recently completed tasks.</span></span> |

## <a name="properties"></a><span data-ttu-id="75631-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="75631-115">Properties</span></span>
| <span data-ttu-id="75631-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="75631-116">Property</span></span>     | <span data-ttu-id="75631-117">Тип</span><span class="sxs-lookup"><span data-stu-id="75631-117">Type</span></span>        | <span data-ttu-id="75631-118">Описание</span><span class="sxs-lookup"><span data-stu-id="75631-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="75631-119">id</span><span class="sxs-lookup"><span data-stu-id="75631-119">id</span></span>|<span data-ttu-id="75631-120">String</span><span class="sxs-lookup"><span data-stu-id="75631-120">String</span></span>|<span data-ttu-id="75631-121">Идентификатор Принттаск.</span><span class="sxs-lookup"><span data-stu-id="75631-121">The printTask's identifier.</span></span> <span data-ttu-id="75631-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75631-122">Read-only.</span></span>|
|<span data-ttu-id="75631-123">status</span><span class="sxs-lookup"><span data-stu-id="75631-123">status</span></span>|[<span data-ttu-id="75631-124">принттаскстатус</span><span class="sxs-lookup"><span data-stu-id="75631-124">printTaskStatus</span></span>](printtaskstatus.md)|<span data-ttu-id="75631-125">Текущее состояние выполнения этого Принттаск.</span><span class="sxs-lookup"><span data-stu-id="75631-125">The current execution status of this printTask.</span></span> <span data-ttu-id="75631-126">**Вызывающее приложение несет ответственность за обновление этого состояния после завершения обработки, если связанный с ним метод printJob не будет перенаправлен на другой принтер.**</span><span class="sxs-lookup"><span data-stu-id="75631-126">**The calling application is responsible for updating this status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="75631-127">Если не выполнить отчет о завершении, то соответствующее задание печати блокируется для печати и в конечном итоге удалено.</span><span class="sxs-lookup"><span data-stu-id="75631-127">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |
|<span data-ttu-id="75631-128">parentUrl</span><span class="sxs-lookup"><span data-stu-id="75631-128">parentUrl</span></span>|<span data-ttu-id="75631-129">String</span><span class="sxs-lookup"><span data-stu-id="75631-129">String</span></span>|<span data-ttu-id="75631-130">URL-адрес объекта печати, который инициировал эту задачу.</span><span class="sxs-lookup"><span data-stu-id="75631-130">The URL for the print entity that triggered this task.</span></span> <span data-ttu-id="75631-131">Например, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span><span class="sxs-lookup"><span data-stu-id="75631-131">For example, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span></span> <span data-ttu-id="75631-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75631-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75631-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="75631-133">Relationships</span></span>
| <span data-ttu-id="75631-134">Связь</span><span class="sxs-lookup"><span data-stu-id="75631-134">Relationship</span></span> | <span data-ttu-id="75631-135">Тип</span><span class="sxs-lookup"><span data-stu-id="75631-135">Type</span></span>        | <span data-ttu-id="75631-136">Описание</span><span class="sxs-lookup"><span data-stu-id="75631-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="75631-137">активирован</span><span class="sxs-lookup"><span data-stu-id="75631-137">trigger</span></span>|[<span data-ttu-id="75631-138">принттасктригжер</span><span class="sxs-lookup"><span data-stu-id="75631-138">printTaskTrigger</span></span>](printtasktrigger.md)|<span data-ttu-id="75631-139">Принттасктригжер, который инициировал выполнение этой задачи.</span><span class="sxs-lookup"><span data-stu-id="75631-139">The printTaskTrigger that triggered this task's execution.</span></span> <span data-ttu-id="75631-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75631-140">Read-only.</span></span>|
|<span data-ttu-id="75631-141">RDLC</span><span class="sxs-lookup"><span data-stu-id="75631-141">definition</span></span>|[<span data-ttu-id="75631-142">принттаскдефинитион</span><span class="sxs-lookup"><span data-stu-id="75631-142">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="75631-143">Принттаскдефинитион, который использовался для создания этой задачи.</span><span class="sxs-lookup"><span data-stu-id="75631-143">The printTaskDefinition that was used to create this task.</span></span> <span data-ttu-id="75631-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75631-144">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75631-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75631-145">JSON representation</span></span>

<span data-ttu-id="75631-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75631-146">The following is a JSON representation of the resource.</span></span>

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
