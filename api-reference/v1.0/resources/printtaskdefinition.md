---
title: тип ресурса printTaskDefinition
description: Представляет задачу, которая может быть вызвана при различных событиях, происходящих в универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9a8a8c78d1e165dfe0f9417c5aa052f9f0b2383b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518104"
---
# <a name="printtaskdefinition-resource-type"></a><span data-ttu-id="7942a-103">тип ресурса printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="7942a-103">printTaskDefinition resource type</span></span>

<span data-ttu-id="7942a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7942a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="7942a-105">Представляет абстрактное определение задачи, которая может быть вызвана при различных событиях, происходящих в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="7942a-105">Represents an abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>

<span data-ttu-id="7942a-106">Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="7942a-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

<span data-ttu-id="7942a-107">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="7942a-107">This resource supports:</span></span>
* <span data-ttu-id="7942a-108">[Подписка на изменение уведомлений.](/graph/universal-print-webhook-notifications)</span><span class="sxs-lookup"><span data-stu-id="7942a-108">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="7942a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="7942a-109">Methods</span></span>
| <span data-ttu-id="7942a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="7942a-110">Method</span></span>       | <span data-ttu-id="7942a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7942a-111">Return Type</span></span> | <span data-ttu-id="7942a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7942a-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7942a-113">Список</span><span class="sxs-lookup"><span data-stu-id="7942a-113">List</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="7942a-114">[printTaskDefinition collection](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7942a-114">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="7942a-115">Получите полный список отпечатковTaskDefinitions, созданных в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="7942a-115">Get a complete list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="7942a-116">Создание</span><span class="sxs-lookup"><span data-stu-id="7942a-116">Create</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="7942a-117">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="7942a-117">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="7942a-118">Создайте новый шрифтTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="7942a-118">Create a new printTaskDefinition.</span></span> |
| <span data-ttu-id="7942a-119">[обновление](../api/print-update-taskdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7942a-119">[Update](../api/print-update-taskdefinition.md)</span></span> | [<span data-ttu-id="7942a-120">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="7942a-120">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="7942a-121">Обновление печатиTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="7942a-121">Update a printTaskDefinition.</span></span> |
| <span data-ttu-id="7942a-122">[удаление](../api/print-delete-taskdefinition.md);</span><span class="sxs-lookup"><span data-stu-id="7942a-122">[Delete](../api/print-delete-taskdefinition.md)</span></span> | <span data-ttu-id="7942a-123">Нет</span><span class="sxs-lookup"><span data-stu-id="7942a-123">None</span></span> | <span data-ttu-id="7942a-124">Удаление печатиTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="7942a-124">Delete a printTaskDefinition.</span></span> |
| [<span data-ttu-id="7942a-125">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="7942a-125">List tasks</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="7942a-126">printTask</span><span class="sxs-lookup"><span data-stu-id="7942a-126">printTask</span></span>](printtask.md) | <span data-ttu-id="7942a-127">Получите список задач, созданных на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="7942a-127">Get a list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="7942a-128">Список включает в себя выполнение текущих задач и недавно завершенных задач.</span><span class="sxs-lookup"><span data-stu-id="7942a-128">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="7942a-129">Вывод задачи</span><span class="sxs-lookup"><span data-stu-id="7942a-129">Get task</span></span>](../api/printtask-get.md) | [<span data-ttu-id="7942a-130">printTask</span><span class="sxs-lookup"><span data-stu-id="7942a-130">printTask</span></span>](printtask.md) | <span data-ttu-id="7942a-131">Получает задачу, созданную на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="7942a-131">Gets a task that has been created based on this definition.</span></span> |
| [<span data-ttu-id="7942a-132">Обновление задачи</span><span class="sxs-lookup"><span data-stu-id="7942a-132">Update task</span></span>](../api/printtaskdefinition-update-task.md) | [<span data-ttu-id="7942a-133">printTask</span><span class="sxs-lookup"><span data-stu-id="7942a-133">printTask</span></span>](printtask.md) | <span data-ttu-id="7942a-134">Обновление задачи, созданной на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="7942a-134">Update a task that has been created based on this definition.</span></span> <span data-ttu-id="7942a-135">**Приложения, которые регистрируют триггеры задач, отвечают за обновление состояния задачи по завершению обработки, если соответствующий printJob не был перенаправлен на другой принтер.**</span><span class="sxs-lookup"><span data-stu-id="7942a-135">**Applications that register task triggers are responsible for updating task status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="7942a-136">Невыполнение отчетов о завершении приведет к блокировке связанного задания печати от печати и в конечном итоге к их удаляемой работе.</span><span class="sxs-lookup"><span data-stu-id="7942a-136">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="7942a-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="7942a-137">Properties</span></span>
|<span data-ttu-id="7942a-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="7942a-138">Property</span></span>|<span data-ttu-id="7942a-139">Тип</span><span class="sxs-lookup"><span data-stu-id="7942a-139">Type</span></span>|<span data-ttu-id="7942a-140">Описание</span><span class="sxs-lookup"><span data-stu-id="7942a-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7942a-141">id</span><span class="sxs-lookup"><span data-stu-id="7942a-141">id</span></span>|<span data-ttu-id="7942a-142">Строка</span><span class="sxs-lookup"><span data-stu-id="7942a-142">String</span></span>|<span data-ttu-id="7942a-143">Идентификатор printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="7942a-143">The printTaskDefinition's identifier.</span></span> <span data-ttu-id="7942a-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7942a-144">Read-only.</span></span>|
|<span data-ttu-id="7942a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7942a-145">displayName</span></span>|<span data-ttu-id="7942a-146">Строка</span><span class="sxs-lookup"><span data-stu-id="7942a-146">String</span></span>|<span data-ttu-id="7942a-147">Имя печатиTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="7942a-147">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="7942a-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="7942a-148">createdBy</span></span>|[<span data-ttu-id="7942a-149">appIdentity</span><span class="sxs-lookup"><span data-stu-id="7942a-149">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="7942a-150">Приложение, создав печатьTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="7942a-150">The application that created the printTaskDefinition.</span></span> <span data-ttu-id="7942a-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7942a-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7942a-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="7942a-152">Relationships</span></span>
|<span data-ttu-id="7942a-153">Связь</span><span class="sxs-lookup"><span data-stu-id="7942a-153">Relationship</span></span>|<span data-ttu-id="7942a-154">Тип</span><span class="sxs-lookup"><span data-stu-id="7942a-154">Type</span></span>|<span data-ttu-id="7942a-155">Описание</span><span class="sxs-lookup"><span data-stu-id="7942a-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7942a-156">tasks</span><span class="sxs-lookup"><span data-stu-id="7942a-156">tasks</span></span>|<span data-ttu-id="7942a-157">[printTask](printtask.md) collection</span><span class="sxs-lookup"><span data-stu-id="7942a-157">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="7942a-158">Список задач, созданных на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="7942a-158">A list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="7942a-159">Список включает в себя выполнение текущих задач и недавно завершенных задач.</span><span class="sxs-lookup"><span data-stu-id="7942a-159">The list includes currently running tasks and recently completed tasks.</span></span> <span data-ttu-id="7942a-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7942a-160">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7942a-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7942a-161">JSON representation</span></span>
<span data-ttu-id="7942a-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7942a-162">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.appIdentity"
  }
}
```

