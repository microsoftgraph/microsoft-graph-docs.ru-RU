---
title: Тип ресурса Принттаскдефинитион
description: Представляет задачу, которая может быть активирована при возникновении различных событий в рамках универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 970b4169dcf4d94eed01be7a15654daa51760151
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078313"
---
# <a name="printtaskdefinition-resource-type"></a><span data-ttu-id="83c33-103">Тип ресурса Принттаскдефинитион</span><span class="sxs-lookup"><span data-stu-id="83c33-103">printTaskDefinition resource type</span></span>

<span data-ttu-id="83c33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83c33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83c33-105">Представляет абстрактное определение задачи, которое может быть запущено при возникновении различных событий в рамках универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="83c33-105">Represents an abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>

<span data-ttu-id="83c33-106">Дополнительные сведения о том, как использовать этот ресурс для поддержки печати по запросу в универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="83c33-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="83c33-107">Методы</span><span class="sxs-lookup"><span data-stu-id="83c33-107">Methods</span></span>

| <span data-ttu-id="83c33-108">Метод</span><span class="sxs-lookup"><span data-stu-id="83c33-108">Method</span></span>       | <span data-ttu-id="83c33-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="83c33-109">Return Type</span></span> | <span data-ttu-id="83c33-110">Описание</span><span class="sxs-lookup"><span data-stu-id="83c33-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="83c33-111">Список</span><span class="sxs-lookup"><span data-stu-id="83c33-111">List</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="83c33-112">Коллекция [принттаскдефинитион](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="83c33-112">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="83c33-113">Получение полного списка Принттаскдефинитионс, созданных в рамках универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="83c33-113">Get a complete list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="83c33-114">Создание</span><span class="sxs-lookup"><span data-stu-id="83c33-114">Create</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="83c33-115">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="83c33-115">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="83c33-116">Создание нового Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="83c33-116">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="83c33-117">Обновление</span><span class="sxs-lookup"><span data-stu-id="83c33-117">Update</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="83c33-118">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="83c33-118">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="83c33-119">Обновление Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="83c33-119">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="83c33-120">Удаление</span><span class="sxs-lookup"><span data-stu-id="83c33-120">Delete</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="83c33-121">Нет</span><span class="sxs-lookup"><span data-stu-id="83c33-121">None</span></span> | <span data-ttu-id="83c33-122">Удаление объекта Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="83c33-122">Delete a printTaskDefinition.</span></span> |
| [<span data-ttu-id="83c33-123">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="83c33-123">List tasks</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="83c33-124">printTask</span><span class="sxs-lookup"><span data-stu-id="83c33-124">printTask</span></span>](printtask.md) | <span data-ttu-id="83c33-125">Получение списка задач, созданных на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="83c33-125">Get a list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="83c33-126">Список содержит текущие выполняемые задачи и недавно выполненные задачи.</span><span class="sxs-lookup"><span data-stu-id="83c33-126">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="83c33-127">Вывод задачи</span><span class="sxs-lookup"><span data-stu-id="83c33-127">Get task</span></span>](../api/printtask-get.md) | [<span data-ttu-id="83c33-128">printTask</span><span class="sxs-lookup"><span data-stu-id="83c33-128">printTask</span></span>](printtask.md) | <span data-ttu-id="83c33-129">Получает задачу, созданную на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="83c33-129">Gets a task that has been created based on this definition.</span></span> |
| [<span data-ttu-id="83c33-130">Обновление задачи</span><span class="sxs-lookup"><span data-stu-id="83c33-130">Update task</span></span>](../api/printtaskdefinition-update-task.md) | <span data-ttu-id="83c33-131">Нет</span><span class="sxs-lookup"><span data-stu-id="83c33-131">None</span></span> | <span data-ttu-id="83c33-132">Обновление задачи, созданной на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="83c33-132">Update a task that has been created based on this definition.</span></span> <span data-ttu-id="83c33-133">**Приложения, которые регистрируют триггеры задач, несут ответственность за обновление состояния задачи при завершении обработки, если связанный метод printJob не будет перенаправлен на другой принтер.**</span><span class="sxs-lookup"><span data-stu-id="83c33-133">**Applications that register task triggers are responsible for updating task status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="83c33-134">Если не выполнить отчет о завершении, то соответствующее задание печати блокируется для печати и в конечном итоге удалено.</span><span class="sxs-lookup"><span data-stu-id="83c33-134">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="83c33-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="83c33-135">Properties</span></span>
| <span data-ttu-id="83c33-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="83c33-136">Property</span></span>     | <span data-ttu-id="83c33-137">Тип</span><span class="sxs-lookup"><span data-stu-id="83c33-137">Type</span></span>        | <span data-ttu-id="83c33-138">Описание</span><span class="sxs-lookup"><span data-stu-id="83c33-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="83c33-139">id</span><span class="sxs-lookup"><span data-stu-id="83c33-139">id</span></span>|<span data-ttu-id="83c33-140">String</span><span class="sxs-lookup"><span data-stu-id="83c33-140">String</span></span>|<span data-ttu-id="83c33-141">Идентификатор Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="83c33-141">The printTaskDefinition's identifier.</span></span> <span data-ttu-id="83c33-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83c33-142">Read-only.</span></span>|
|<span data-ttu-id="83c33-143">displayName</span><span class="sxs-lookup"><span data-stu-id="83c33-143">displayName</span></span>|<span data-ttu-id="83c33-144">String</span><span class="sxs-lookup"><span data-stu-id="83c33-144">String</span></span>|<span data-ttu-id="83c33-145">Имя Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="83c33-145">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="83c33-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="83c33-146">createdBy</span></span>|[<span data-ttu-id="83c33-147">аппидентити</span><span class="sxs-lookup"><span data-stu-id="83c33-147">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="83c33-148">Приложение, создавшее Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="83c33-148">The application that created the printTaskDefinition.</span></span> <span data-ttu-id="83c33-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83c33-149">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83c33-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="83c33-150">Relationships</span></span>
| <span data-ttu-id="83c33-151">Связь</span><span class="sxs-lookup"><span data-stu-id="83c33-151">Relationship</span></span> | <span data-ttu-id="83c33-152">Тип</span><span class="sxs-lookup"><span data-stu-id="83c33-152">Type</span></span>        | <span data-ttu-id="83c33-153">Описание</span><span class="sxs-lookup"><span data-stu-id="83c33-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="83c33-154">tasks</span><span class="sxs-lookup"><span data-stu-id="83c33-154">tasks</span></span>|<span data-ttu-id="83c33-155">Коллекция [принттаск](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="83c33-155">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="83c33-156">Список задач, созданных на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="83c33-156">A list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="83c33-157">Список содержит текущие выполняемые задачи и недавно выполненные задачи.</span><span class="sxs-lookup"><span data-stu-id="83c33-157">The list includes currently running tasks and recently completed tasks.</span></span> <span data-ttu-id="83c33-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83c33-158">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83c33-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83c33-159">JSON representation</span></span>

<span data-ttu-id="83c33-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83c33-160">The following is a JSON representation of the resource.</span></span>

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

