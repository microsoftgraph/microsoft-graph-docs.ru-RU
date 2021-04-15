---
title: тип ресурса printTaskDefinition
description: Представляет задачу, которая может быть вызвана при различных событиях, происходящих в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2495825ec64d73bb440d16e4eae9125f8dbd38eb
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766310"
---
# <a name="printtaskdefinition-resource-type"></a><span data-ttu-id="c2099-103">тип ресурса printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="c2099-103">printTaskDefinition resource type</span></span>

<span data-ttu-id="c2099-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2099-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2099-105">Представляет абстрактное определение задачи, которая может быть вызвана при различных событиях, происходящих в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="c2099-105">Represents an abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>

<span data-ttu-id="c2099-106">Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="c2099-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

<span data-ttu-id="c2099-107">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="c2099-107">This resource supports:</span></span>
* <span data-ttu-id="c2099-108">[Подписка на изменение уведомлений.](/graph/universal-print-webhook-notifications)</span><span class="sxs-lookup"><span data-stu-id="c2099-108">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="c2099-109">Методы</span><span class="sxs-lookup"><span data-stu-id="c2099-109">Methods</span></span>

| <span data-ttu-id="c2099-110">Метод</span><span class="sxs-lookup"><span data-stu-id="c2099-110">Method</span></span>       | <span data-ttu-id="c2099-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c2099-111">Return Type</span></span> | <span data-ttu-id="c2099-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c2099-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c2099-113">Список</span><span class="sxs-lookup"><span data-stu-id="c2099-113">List</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="c2099-114">[printTaskDefinition collection](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c2099-114">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="c2099-115">Получите полный список отпечатковTaskDefinitions, созданных в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="c2099-115">Get a complete list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="c2099-116">Create</span><span class="sxs-lookup"><span data-stu-id="c2099-116">Create</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="c2099-117">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="c2099-117">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="c2099-118">Создайте новый шрифтTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c2099-118">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="c2099-119">Обновление</span><span class="sxs-lookup"><span data-stu-id="c2099-119">Update</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="c2099-120">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="c2099-120">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="c2099-121">Обновление печатиTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c2099-121">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="c2099-122">Delete</span><span class="sxs-lookup"><span data-stu-id="c2099-122">Delete</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="c2099-123">Нет</span><span class="sxs-lookup"><span data-stu-id="c2099-123">None</span></span> | <span data-ttu-id="c2099-124">Удаление печатиTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c2099-124">Delete a printTaskDefinition.</span></span> |
| [<span data-ttu-id="c2099-125">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="c2099-125">List tasks</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="c2099-126">printTask</span><span class="sxs-lookup"><span data-stu-id="c2099-126">printTask</span></span>](printtask.md) | <span data-ttu-id="c2099-127">Получите список задач, созданных на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="c2099-127">Get a list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="c2099-128">Список включает в себя выполнение текущих задач и недавно завершенных задач.</span><span class="sxs-lookup"><span data-stu-id="c2099-128">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="c2099-129">Вывод задачи</span><span class="sxs-lookup"><span data-stu-id="c2099-129">Get task</span></span>](../api/printtask-get.md) | [<span data-ttu-id="c2099-130">printTask</span><span class="sxs-lookup"><span data-stu-id="c2099-130">printTask</span></span>](printtask.md) | <span data-ttu-id="c2099-131">Получает задачу, созданную на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="c2099-131">Gets a task that has been created based on this definition.</span></span> |
| [<span data-ttu-id="c2099-132">Обновление задачи</span><span class="sxs-lookup"><span data-stu-id="c2099-132">Update task</span></span>](../api/printtaskdefinition-update-task.md) | [<span data-ttu-id="c2099-133">printTask</span><span class="sxs-lookup"><span data-stu-id="c2099-133">printTask</span></span>](printtask.md) | <span data-ttu-id="c2099-134">Обновление задачи, созданной на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="c2099-134">Update a task that has been created based on this definition.</span></span> <span data-ttu-id="c2099-135">**Приложения, которые регистрируют триггеры задач, отвечают за обновление состояния задачи по завершению обработки, если соответствующий printJob не был перенаправлен на другой принтер.**</span><span class="sxs-lookup"><span data-stu-id="c2099-135">**Applications that register task triggers are responsible for updating task status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="c2099-136">Невыполнение отчетов о завершении приведет к блокировке связанного задания печати от печати и в конечном итоге к их удаляемой работе.</span><span class="sxs-lookup"><span data-stu-id="c2099-136">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="c2099-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2099-137">Properties</span></span>
| <span data-ttu-id="c2099-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2099-138">Property</span></span>     | <span data-ttu-id="c2099-139">Тип</span><span class="sxs-lookup"><span data-stu-id="c2099-139">Type</span></span>        | <span data-ttu-id="c2099-140">Описание</span><span class="sxs-lookup"><span data-stu-id="c2099-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c2099-141">id</span><span class="sxs-lookup"><span data-stu-id="c2099-141">id</span></span>|<span data-ttu-id="c2099-142">String</span><span class="sxs-lookup"><span data-stu-id="c2099-142">String</span></span>|<span data-ttu-id="c2099-143">Идентификатор printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c2099-143">The printTaskDefinition's identifier.</span></span> <span data-ttu-id="c2099-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2099-144">Read-only.</span></span>|
|<span data-ttu-id="c2099-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c2099-145">displayName</span></span>|<span data-ttu-id="c2099-146">String</span><span class="sxs-lookup"><span data-stu-id="c2099-146">String</span></span>|<span data-ttu-id="c2099-147">Имя печатиTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c2099-147">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="c2099-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="c2099-148">createdBy</span></span>|[<span data-ttu-id="c2099-149">appIdentity</span><span class="sxs-lookup"><span data-stu-id="c2099-149">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="c2099-150">Приложение, создав печатьTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c2099-150">The application that created the printTaskDefinition.</span></span> <span data-ttu-id="c2099-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2099-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2099-152">Связи</span><span class="sxs-lookup"><span data-stu-id="c2099-152">Relationships</span></span>
| <span data-ttu-id="c2099-153">Связь</span><span class="sxs-lookup"><span data-stu-id="c2099-153">Relationship</span></span> | <span data-ttu-id="c2099-154">Тип</span><span class="sxs-lookup"><span data-stu-id="c2099-154">Type</span></span>        | <span data-ttu-id="c2099-155">Описание</span><span class="sxs-lookup"><span data-stu-id="c2099-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c2099-156">tasks</span><span class="sxs-lookup"><span data-stu-id="c2099-156">tasks</span></span>|<span data-ttu-id="c2099-157">[printTask](printtask.md) collection</span><span class="sxs-lookup"><span data-stu-id="c2099-157">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="c2099-158">Список задач, созданных на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="c2099-158">A list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="c2099-159">Список включает в себя выполнение текущих задач и недавно завершенных задач.</span><span class="sxs-lookup"><span data-stu-id="c2099-159">The list includes currently running tasks and recently completed tasks.</span></span> <span data-ttu-id="c2099-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2099-160">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2099-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2099-161">JSON representation</span></span>

<span data-ttu-id="c2099-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2099-162">The following is a JSON representation of the resource.</span></span>

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

