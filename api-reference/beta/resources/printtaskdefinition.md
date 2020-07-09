---
title: Тип ресурса Принттаскдефинитион
description: Представляет задачу, которая может быть активирована при возникновении различных событий в рамках универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 013d2756455abebc0f20bbe5a1d186a0a4d65648
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091699"
---
# <a name="printtaskdefinition-resource-type"></a><span data-ttu-id="128a7-103">Тип ресурса Принттаскдефинитион</span><span class="sxs-lookup"><span data-stu-id="128a7-103">printTaskDefinition resource type</span></span>

<span data-ttu-id="128a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="128a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="128a7-105">Представляет абстрактное определение задачи, которое может быть запущено при возникновении различных событий в рамках универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="128a7-105">Represents an abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>

<span data-ttu-id="128a7-106">Дополнительные сведения о том, как использовать этот ресурс для поддержки печати по запросу в универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="128a7-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="128a7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="128a7-107">Methods</span></span>

| <span data-ttu-id="128a7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="128a7-108">Method</span></span>       | <span data-ttu-id="128a7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="128a7-109">Return Type</span></span> | <span data-ttu-id="128a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="128a7-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="128a7-111">Список</span><span class="sxs-lookup"><span data-stu-id="128a7-111">List</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="128a7-112">Коллекция [принттаскдефинитион](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="128a7-112">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="128a7-113">Получение полного списка Принттаскдефинитионс, созданных в рамках универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="128a7-113">Get a complete list of printTaskDefinitions created within Universal Print.</span></span> |
| <span data-ttu-id="128a7-114">[Создание](../api/print-post-taskdefinitions.md);</span><span class="sxs-lookup"><span data-stu-id="128a7-114">[Create](../api/print-post-taskdefinitions.md)</span></span> | [<span data-ttu-id="128a7-115">принттаскдефинитион</span><span class="sxs-lookup"><span data-stu-id="128a7-115">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="128a7-116">Создание нового Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="128a7-116">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="128a7-117">Update</span><span class="sxs-lookup"><span data-stu-id="128a7-117">Update</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="128a7-118">принттаскдефинитион</span><span class="sxs-lookup"><span data-stu-id="128a7-118">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="128a7-119">Обновление Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="128a7-119">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="128a7-120">Delete</span><span class="sxs-lookup"><span data-stu-id="128a7-120">Delete</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="128a7-121">Нет</span><span class="sxs-lookup"><span data-stu-id="128a7-121">None</span></span> | <span data-ttu-id="128a7-122">Удаление объекта Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="128a7-122">Delete a printTaskDefinition.</span></span> |
| [<span data-ttu-id="128a7-123">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="128a7-123">List tasks</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="128a7-124">принттаск</span><span class="sxs-lookup"><span data-stu-id="128a7-124">printTask</span></span>](printtask.md) | <span data-ttu-id="128a7-125">Получение списка задач, созданных на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="128a7-125">Get a list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="128a7-126">Список содержит текущие выполняемые задачи и недавно выполненные задачи.</span><span class="sxs-lookup"><span data-stu-id="128a7-126">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="128a7-127">Вывод задачи</span><span class="sxs-lookup"><span data-stu-id="128a7-127">Get task</span></span>](../api/printtask-get.md) | [<span data-ttu-id="128a7-128">принттаск</span><span class="sxs-lookup"><span data-stu-id="128a7-128">printTask</span></span>](printtask.md) | <span data-ttu-id="128a7-129">Получает задачу, созданную на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="128a7-129">Gets a task that has been created based on this definition.</span></span> |
| [<span data-ttu-id="128a7-130">Обновление задачи</span><span class="sxs-lookup"><span data-stu-id="128a7-130">Update task</span></span>](../api/printtaskdefinition-update-task.md) | <span data-ttu-id="128a7-131">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="128a7-131">None</span></span> | <span data-ttu-id="128a7-132">Обновление задачи, созданной на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="128a7-132">Update a task that has been created based on this definition.</span></span> <span data-ttu-id="128a7-133">**Приложения, которые регистрируют триггеры задач, несут ответственность за обновление состояния задачи при завершении обработки, если связанный метод printJob не будет перенаправлен на другой принтер.**</span><span class="sxs-lookup"><span data-stu-id="128a7-133">**Applications that register task triggers are responsible for updating task status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="128a7-134">Если не выполнить отчет о завершении, то соответствующее задание печати блокируется для печати и в конечном итоге удалено.</span><span class="sxs-lookup"><span data-stu-id="128a7-134">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="128a7-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="128a7-135">Properties</span></span>
| <span data-ttu-id="128a7-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="128a7-136">Property</span></span>     | <span data-ttu-id="128a7-137">Тип</span><span class="sxs-lookup"><span data-stu-id="128a7-137">Type</span></span>        | <span data-ttu-id="128a7-138">Описание</span><span class="sxs-lookup"><span data-stu-id="128a7-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="128a7-139">id</span><span class="sxs-lookup"><span data-stu-id="128a7-139">id</span></span>|<span data-ttu-id="128a7-140">String</span><span class="sxs-lookup"><span data-stu-id="128a7-140">String</span></span>|<span data-ttu-id="128a7-141">Идентификатор Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="128a7-141">The printTaskDefinition's identifier.</span></span> <span data-ttu-id="128a7-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="128a7-142">Read-only.</span></span>|
|<span data-ttu-id="128a7-143">displayName</span><span class="sxs-lookup"><span data-stu-id="128a7-143">displayName</span></span>|<span data-ttu-id="128a7-144">Строка</span><span class="sxs-lookup"><span data-stu-id="128a7-144">String</span></span>|<span data-ttu-id="128a7-145">Имя Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="128a7-145">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="128a7-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="128a7-146">createdBy</span></span>|[<span data-ttu-id="128a7-147">аппидентити</span><span class="sxs-lookup"><span data-stu-id="128a7-147">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="128a7-148">Приложение, создавшее Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="128a7-148">The application that created the printTaskDefinition.</span></span> <span data-ttu-id="128a7-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="128a7-149">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="128a7-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="128a7-150">Relationships</span></span>
| <span data-ttu-id="128a7-151">Связь</span><span class="sxs-lookup"><span data-stu-id="128a7-151">Relationship</span></span> | <span data-ttu-id="128a7-152">Тип</span><span class="sxs-lookup"><span data-stu-id="128a7-152">Type</span></span>        | <span data-ttu-id="128a7-153">Описание</span><span class="sxs-lookup"><span data-stu-id="128a7-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="128a7-154">tasks</span><span class="sxs-lookup"><span data-stu-id="128a7-154">tasks</span></span>|<span data-ttu-id="128a7-155">Коллекция [принттаск](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="128a7-155">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="128a7-156">Список задач, созданных на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="128a7-156">A list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="128a7-157">Список содержит текущие выполняемые задачи и недавно выполненные задачи.</span><span class="sxs-lookup"><span data-stu-id="128a7-157">The list includes currently running tasks and recently completed tasks.</span></span> <span data-ttu-id="128a7-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="128a7-158">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="128a7-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="128a7-159">JSON representation</span></span>

<span data-ttu-id="128a7-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="128a7-160">The following is a JSON representation of the resource.</span></span>

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