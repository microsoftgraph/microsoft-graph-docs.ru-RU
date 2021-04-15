---
title: тип ресурса printTask
description: Представляет задачу, выполненную или выполненную в результате события универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c684ff64aa4c3667214b61b70a422690381525b3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766303"
---
# <a name="printtask-resource-type"></a><span data-ttu-id="54de7-103">тип ресурса printTask</span><span class="sxs-lookup"><span data-stu-id="54de7-103">printTask resource type</span></span>

<span data-ttu-id="54de7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54de7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54de7-105">Представляет задачу, выполненную или выполненную в результате события универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="54de7-105">Represents a task that is executing or has been executed as a result of a Universal Print event.</span></span>

<span data-ttu-id="54de7-106">Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="54de7-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="54de7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="54de7-107">Methods</span></span>

| <span data-ttu-id="54de7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="54de7-108">Method</span></span>       | <span data-ttu-id="54de7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="54de7-109">Return Type</span></span> | <span data-ttu-id="54de7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="54de7-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="54de7-111">Список (от printTaskDefintion)</span><span class="sxs-lookup"><span data-stu-id="54de7-111">List (from printTaskDefintion)</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="54de7-112">printTask</span><span class="sxs-lookup"><span data-stu-id="54de7-112">printTask</span></span>](printtask.md) | <span data-ttu-id="54de7-113">Получите список задач, созданных на основе определенного шрифтаTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="54de7-113">Get a list of tasks that have been created based on a particular printTaskDefinition.</span></span> <span data-ttu-id="54de7-114">Список включает в себя выполнение текущих задач и недавно завершенных задач.</span><span class="sxs-lookup"><span data-stu-id="54de7-114">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="54de7-115">Get</span><span class="sxs-lookup"><span data-stu-id="54de7-115">Get</span></span>](../api/printtask-get.md) | [<span data-ttu-id="54de7-116">printTask</span><span class="sxs-lookup"><span data-stu-id="54de7-116">printTask</span></span>](printtask.md) | <span data-ttu-id="54de7-117">Сведения о задаче печати.</span><span class="sxs-lookup"><span data-stu-id="54de7-117">Get details about a print task.</span></span> |
| [<span data-ttu-id="54de7-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="54de7-118">Update</span></span>](../api/printtaskdefinition-update-task.md) | [<span data-ttu-id="54de7-119">printTask</span><span class="sxs-lookup"><span data-stu-id="54de7-119">printTask</span></span>](printtask.md) | <span data-ttu-id="54de7-120">Обновляет задачу печати.</span><span class="sxs-lookup"><span data-stu-id="54de7-120">Updates a print task.</span></span> |

## <a name="properties"></a><span data-ttu-id="54de7-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="54de7-121">Properties</span></span>
| <span data-ttu-id="54de7-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="54de7-122">Property</span></span>     | <span data-ttu-id="54de7-123">Тип</span><span class="sxs-lookup"><span data-stu-id="54de7-123">Type</span></span>        | <span data-ttu-id="54de7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="54de7-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="54de7-125">id</span><span class="sxs-lookup"><span data-stu-id="54de7-125">id</span></span>|<span data-ttu-id="54de7-126">String</span><span class="sxs-lookup"><span data-stu-id="54de7-126">String</span></span>|<span data-ttu-id="54de7-127">Идентификатор printTask.</span><span class="sxs-lookup"><span data-stu-id="54de7-127">The printTask's identifier.</span></span> <span data-ttu-id="54de7-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54de7-128">Read-only.</span></span>|
|<span data-ttu-id="54de7-129">status</span><span class="sxs-lookup"><span data-stu-id="54de7-129">status</span></span>|[<span data-ttu-id="54de7-130">printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="54de7-130">printTaskStatus</span></span>](printtaskstatus.md)|<span data-ttu-id="54de7-131">Текущее состояние выполнения этого printTask.</span><span class="sxs-lookup"><span data-stu-id="54de7-131">The current execution status of this printTask.</span></span> <span data-ttu-id="54de7-132">**Приложение вызовов отвечает за обновление этого состояния по завершению обработки, если соответствующий printJob не был перенаправлен на другой принтер.**</span><span class="sxs-lookup"><span data-stu-id="54de7-132">**The calling application is responsible for updating this status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="54de7-133">Невыполнение отчетов о завершении приведет к блокировке связанного задания печати от печати и в конечном итоге к их удаляемой работе.</span><span class="sxs-lookup"><span data-stu-id="54de7-133">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |
|<span data-ttu-id="54de7-134">parentUrl</span><span class="sxs-lookup"><span data-stu-id="54de7-134">parentUrl</span></span>|<span data-ttu-id="54de7-135">String</span><span class="sxs-lookup"><span data-stu-id="54de7-135">String</span></span>|<span data-ttu-id="54de7-136">URL-адрес для объекта печати, который вызвал эту задачу.</span><span class="sxs-lookup"><span data-stu-id="54de7-136">The URL for the print entity that triggered this task.</span></span> <span data-ttu-id="54de7-137">Например, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span><span class="sxs-lookup"><span data-stu-id="54de7-137">For example, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span></span> <span data-ttu-id="54de7-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54de7-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54de7-139">Связи</span><span class="sxs-lookup"><span data-stu-id="54de7-139">Relationships</span></span>
| <span data-ttu-id="54de7-140">Связь</span><span class="sxs-lookup"><span data-stu-id="54de7-140">Relationship</span></span> | <span data-ttu-id="54de7-141">Тип</span><span class="sxs-lookup"><span data-stu-id="54de7-141">Type</span></span>        | <span data-ttu-id="54de7-142">Описание</span><span class="sxs-lookup"><span data-stu-id="54de7-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="54de7-143">триггер</span><span class="sxs-lookup"><span data-stu-id="54de7-143">trigger</span></span>|[<span data-ttu-id="54de7-144">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="54de7-144">printTaskTrigger</span></span>](printtasktrigger.md)|<span data-ttu-id="54de7-145">PrintTaskTrigger, который вызвал выполнение этой задачи.</span><span class="sxs-lookup"><span data-stu-id="54de7-145">The printTaskTrigger that triggered this task's execution.</span></span> <span data-ttu-id="54de7-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54de7-146">Read-only.</span></span>|
|<span data-ttu-id="54de7-147">определение</span><span class="sxs-lookup"><span data-stu-id="54de7-147">definition</span></span>|[<span data-ttu-id="54de7-148">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="54de7-148">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="54de7-149">PrintTaskDefinition, который использовался для создания этой задачи.</span><span class="sxs-lookup"><span data-stu-id="54de7-149">The printTaskDefinition that was used to create this task.</span></span> <span data-ttu-id="54de7-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54de7-150">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54de7-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54de7-151">JSON representation</span></span>

<span data-ttu-id="54de7-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54de7-152">The following is a JSON representation of the resource.</span></span>

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


