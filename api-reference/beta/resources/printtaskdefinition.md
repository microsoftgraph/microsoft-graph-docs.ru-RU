---
title: Тип ресурса printTaskDefinition
description: Представляет задачу, которую можно запускать при различных событиях в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: bbffceb08be336cd816d80f03236078b39348339
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934865"
---
# <a name="printtaskdefinition-resource-type"></a><span data-ttu-id="632e1-103">Тип ресурса printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="632e1-103">printTaskDefinition resource type</span></span>

<span data-ttu-id="632e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="632e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="632e1-105">Представляет абстрактное определение задачи, которое может запускаться при различных событиях в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="632e1-105">Represents an abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>

<span data-ttu-id="632e1-106">Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати с потягивом в универсальную печать, см. в подстройки "Расширение универсальной печати [для поддержки печати потягив".](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="632e1-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

<span data-ttu-id="632e1-107">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="632e1-107">This resource supports:</span></span>
* <span data-ttu-id="632e1-108">[Подписка на уведомления об изменениях.](/graph/universal-print-webhook-notifications)</span><span class="sxs-lookup"><span data-stu-id="632e1-108">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="632e1-109">Методы</span><span class="sxs-lookup"><span data-stu-id="632e1-109">Methods</span></span>

| <span data-ttu-id="632e1-110">Метод</span><span class="sxs-lookup"><span data-stu-id="632e1-110">Method</span></span>       | <span data-ttu-id="632e1-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="632e1-111">Return Type</span></span> | <span data-ttu-id="632e1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="632e1-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="632e1-113">Список</span><span class="sxs-lookup"><span data-stu-id="632e1-113">List</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="632e1-114">[Коллекция printTaskDefinition](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="632e1-114">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="632e1-115">Получите полный список printTaskDefinitions, созданных в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="632e1-115">Get a complete list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="632e1-116">Создание</span><span class="sxs-lookup"><span data-stu-id="632e1-116">Create</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="632e1-117">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="632e1-117">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="632e1-118">Создайте новый printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="632e1-118">Create a new printTaskDefinition.</span></span> |
| <span data-ttu-id="632e1-119">[обновление](../api/print-update-taskdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="632e1-119">[Update](../api/print-update-taskdefinition.md)</span></span> | [<span data-ttu-id="632e1-120">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="632e1-120">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="632e1-121">Обновление printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="632e1-121">Update a printTaskDefinition.</span></span> |
| <span data-ttu-id="632e1-122">[удаление](../api/print-delete-taskdefinition.md);</span><span class="sxs-lookup"><span data-stu-id="632e1-122">[Delete](../api/print-delete-taskdefinition.md)</span></span> | <span data-ttu-id="632e1-123">Нет</span><span class="sxs-lookup"><span data-stu-id="632e1-123">None</span></span> | <span data-ttu-id="632e1-124">Удаление printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="632e1-124">Delete a printTaskDefinition.</span></span> |
| [<span data-ttu-id="632e1-125">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="632e1-125">List tasks</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="632e1-126">printTask</span><span class="sxs-lookup"><span data-stu-id="632e1-126">printTask</span></span>](printtask.md) | <span data-ttu-id="632e1-127">Получите список задач, созданных на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="632e1-127">Get a list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="632e1-128">Список включает в себя задачи, которые в настоящее время запущены, и недавно завершенные задачи.</span><span class="sxs-lookup"><span data-stu-id="632e1-128">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="632e1-129">Вывод задачи</span><span class="sxs-lookup"><span data-stu-id="632e1-129">Get task</span></span>](../api/printtask-get.md) | [<span data-ttu-id="632e1-130">printTask</span><span class="sxs-lookup"><span data-stu-id="632e1-130">printTask</span></span>](printtask.md) | <span data-ttu-id="632e1-131">Получает задачу, созданную на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="632e1-131">Gets a task that has been created based on this definition.</span></span> |
| [<span data-ttu-id="632e1-132">Обновление задачи</span><span class="sxs-lookup"><span data-stu-id="632e1-132">Update task</span></span>](../api/printtaskdefinition-update-task.md) | <span data-ttu-id="632e1-133">Нет</span><span class="sxs-lookup"><span data-stu-id="632e1-133">None</span></span> | <span data-ttu-id="632e1-134">Обновление задачи, созданной на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="632e1-134">Update a task that has been created based on this definition.</span></span> <span data-ttu-id="632e1-135">**Приложения, регистрющие триггеры задач, отвечают за обновление состояния задачи после завершения обработки, если связанная задача printJob не была перенаправлена на другой принтер.**</span><span class="sxs-lookup"><span data-stu-id="632e1-135">**Applications that register task triggers are responsible for updating task status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="632e1-136">Если не сообщить о завершении, связанное задание печати будет заблокировано и удалено.</span><span class="sxs-lookup"><span data-stu-id="632e1-136">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="632e1-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="632e1-137">Properties</span></span>
| <span data-ttu-id="632e1-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="632e1-138">Property</span></span>     | <span data-ttu-id="632e1-139">Тип</span><span class="sxs-lookup"><span data-stu-id="632e1-139">Type</span></span>        | <span data-ttu-id="632e1-140">Описание</span><span class="sxs-lookup"><span data-stu-id="632e1-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="632e1-141">id</span><span class="sxs-lookup"><span data-stu-id="632e1-141">id</span></span>|<span data-ttu-id="632e1-142">String</span><span class="sxs-lookup"><span data-stu-id="632e1-142">String</span></span>|<span data-ttu-id="632e1-143">Идентификатор printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="632e1-143">The printTaskDefinition's identifier.</span></span> <span data-ttu-id="632e1-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="632e1-144">Read-only.</span></span>|
|<span data-ttu-id="632e1-145">displayName</span><span class="sxs-lookup"><span data-stu-id="632e1-145">displayName</span></span>|<span data-ttu-id="632e1-146">String</span><span class="sxs-lookup"><span data-stu-id="632e1-146">String</span></span>|<span data-ttu-id="632e1-147">Имя printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="632e1-147">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="632e1-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="632e1-148">createdBy</span></span>|[<span data-ttu-id="632e1-149">appIdentity</span><span class="sxs-lookup"><span data-stu-id="632e1-149">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="632e1-150">Приложение, созда которое создало printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="632e1-150">The application that created the printTaskDefinition.</span></span> <span data-ttu-id="632e1-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="632e1-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="632e1-152">Связи</span><span class="sxs-lookup"><span data-stu-id="632e1-152">Relationships</span></span>
| <span data-ttu-id="632e1-153">Связь</span><span class="sxs-lookup"><span data-stu-id="632e1-153">Relationship</span></span> | <span data-ttu-id="632e1-154">Тип</span><span class="sxs-lookup"><span data-stu-id="632e1-154">Type</span></span>        | <span data-ttu-id="632e1-155">Описание</span><span class="sxs-lookup"><span data-stu-id="632e1-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="632e1-156">tasks</span><span class="sxs-lookup"><span data-stu-id="632e1-156">tasks</span></span>|<span data-ttu-id="632e1-157">[Коллекция printTask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="632e1-157">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="632e1-158">Список задач, созданных на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="632e1-158">A list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="632e1-159">Список включает в себя задачи, которые в настоящее время запущены, и недавно завершенные задачи.</span><span class="sxs-lookup"><span data-stu-id="632e1-159">The list includes currently running tasks and recently completed tasks.</span></span> <span data-ttu-id="632e1-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="632e1-160">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="632e1-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="632e1-161">JSON representation</span></span>

<span data-ttu-id="632e1-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="632e1-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {"@odata.type": "microsoft.graph.appIdentity"},
  "tasks": [{"@odata.type": "microsoft.graph.printTask"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

