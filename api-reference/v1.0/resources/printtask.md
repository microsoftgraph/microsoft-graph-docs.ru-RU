---
title: тип ресурса printTask
description: Представляет задачу, выполненную или выполненную в результате события универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2026706ec46a2408d20231add8203d2f5a622c96
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517452"
---
# <a name="printtask-resource-type"></a><span data-ttu-id="5496a-103">тип ресурса printTask</span><span class="sxs-lookup"><span data-stu-id="5496a-103">printTask resource type</span></span>

<span data-ttu-id="5496a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5496a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="5496a-105">Представляет задачу, выполненную или выполненную в результате события универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="5496a-105">Represents a task that is executing or has been executed as a result of a Universal Print event.</span></span>

<span data-ttu-id="5496a-106">Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="5496a-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="5496a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5496a-107">Methods</span></span>
|<span data-ttu-id="5496a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5496a-108">Method</span></span>|<span data-ttu-id="5496a-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="5496a-109">Return type</span></span>|<span data-ttu-id="5496a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5496a-110">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="5496a-111">Список (от printTaskDefintion)</span><span class="sxs-lookup"><span data-stu-id="5496a-111">List (from printTaskDefintion)</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="5496a-112">printTask</span><span class="sxs-lookup"><span data-stu-id="5496a-112">printTask</span></span>](printtask.md) | <span data-ttu-id="5496a-113">Получите список задач, созданных на основе определенного шрифтаTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="5496a-113">Get a list of tasks that have been created based on a particular printTaskDefinition.</span></span> <span data-ttu-id="5496a-114">Список включает в себя выполнение текущих задач и недавно завершенных задач.</span><span class="sxs-lookup"><span data-stu-id="5496a-114">The list includes currently running tasks and recently completed tasks.</span></span> |
| <span data-ttu-id="5496a-115">[получение](../api/printtask-get.md);</span><span class="sxs-lookup"><span data-stu-id="5496a-115">[Get](../api/printtask-get.md)</span></span> | [<span data-ttu-id="5496a-116">printTask</span><span class="sxs-lookup"><span data-stu-id="5496a-116">printTask</span></span>](printtask.md) | <span data-ttu-id="5496a-117">Сведения о задаче печати.</span><span class="sxs-lookup"><span data-stu-id="5496a-117">Get details about a print task.</span></span> |
| <span data-ttu-id="5496a-118">[обновление](../api/printtaskdefinition-update-task.md).</span><span class="sxs-lookup"><span data-stu-id="5496a-118">[Update](../api/printtaskdefinition-update-task.md)</span></span> | [<span data-ttu-id="5496a-119">printTask</span><span class="sxs-lookup"><span data-stu-id="5496a-119">printTask</span></span>](printtask.md) | <span data-ttu-id="5496a-120">Обновляет задачу печати.</span><span class="sxs-lookup"><span data-stu-id="5496a-120">Updates a print task.</span></span> |

## <a name="properties"></a><span data-ttu-id="5496a-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="5496a-121">Properties</span></span>
|<span data-ttu-id="5496a-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="5496a-122">Property</span></span>|<span data-ttu-id="5496a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5496a-123">Type</span></span>|<span data-ttu-id="5496a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5496a-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5496a-125">id</span><span class="sxs-lookup"><span data-stu-id="5496a-125">id</span></span>|<span data-ttu-id="5496a-126">Строка</span><span class="sxs-lookup"><span data-stu-id="5496a-126">String</span></span>|<span data-ttu-id="5496a-127">Идентификатор printTask.</span><span class="sxs-lookup"><span data-stu-id="5496a-127">The printTask's identifier.</span></span> <span data-ttu-id="5496a-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5496a-128">Read-only.</span></span>|
|<span data-ttu-id="5496a-129">status</span><span class="sxs-lookup"><span data-stu-id="5496a-129">status</span></span>|[<span data-ttu-id="5496a-130">printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="5496a-130">printTaskStatus</span></span>](printtaskstatus.md)|<span data-ttu-id="5496a-131">Текущее состояние выполнения этого printTask.</span><span class="sxs-lookup"><span data-stu-id="5496a-131">The current execution status of this printTask.</span></span> <span data-ttu-id="5496a-132">**Приложение вызовов отвечает за обновление этого состояния по завершению обработки, если соответствующий printJob не был перенаправлен на другой принтер.**</span><span class="sxs-lookup"><span data-stu-id="5496a-132">**The calling application is responsible for updating this status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="5496a-133">Невыполнение отчетов о завершении приведет к блокировке связанного задания печати от печати и в конечном итоге к их удаляемой работе.</span><span class="sxs-lookup"><span data-stu-id="5496a-133">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |
|<span data-ttu-id="5496a-134">parentUrl</span><span class="sxs-lookup"><span data-stu-id="5496a-134">parentUrl</span></span>|<span data-ttu-id="5496a-135">Строка</span><span class="sxs-lookup"><span data-stu-id="5496a-135">String</span></span>|<span data-ttu-id="5496a-136">URL-адрес для объекта печати, который вызвал эту задачу.</span><span class="sxs-lookup"><span data-stu-id="5496a-136">The URL for the print entity that triggered this task.</span></span> <span data-ttu-id="5496a-137">Например, `https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{jobId}`.</span><span class="sxs-lookup"><span data-stu-id="5496a-137">For example, `https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{jobId}`.</span></span> <span data-ttu-id="5496a-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5496a-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5496a-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="5496a-139">Relationships</span></span>
|<span data-ttu-id="5496a-140">Связь</span><span class="sxs-lookup"><span data-stu-id="5496a-140">Relationship</span></span>|<span data-ttu-id="5496a-141">Тип</span><span class="sxs-lookup"><span data-stu-id="5496a-141">Type</span></span>|<span data-ttu-id="5496a-142">Описание</span><span class="sxs-lookup"><span data-stu-id="5496a-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5496a-143">триггер</span><span class="sxs-lookup"><span data-stu-id="5496a-143">trigger</span></span>|[<span data-ttu-id="5496a-144">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="5496a-144">printTaskTrigger</span></span>](printtasktrigger.md)|<span data-ttu-id="5496a-145">PrintTaskTrigger, который вызвал выполнение этой задачи.</span><span class="sxs-lookup"><span data-stu-id="5496a-145">The printTaskTrigger that triggered this task's execution.</span></span> <span data-ttu-id="5496a-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5496a-146">Read-only.</span></span>|
|<span data-ttu-id="5496a-147">определение</span><span class="sxs-lookup"><span data-stu-id="5496a-147">definition</span></span>|[<span data-ttu-id="5496a-148">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="5496a-148">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="5496a-149">PrintTaskDefinition, который использовался для создания этой задачи.</span><span class="sxs-lookup"><span data-stu-id="5496a-149">The printTaskDefinition that was used to create this task.</span></span> <span data-ttu-id="5496a-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5496a-150">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5496a-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5496a-151">JSON representation</span></span>
<span data-ttu-id="5496a-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5496a-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTask",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTask",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printTaskStatus"
  },
  "parentUrl": "String"
}
```

