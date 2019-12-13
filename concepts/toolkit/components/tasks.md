---
title: Компонент Tasks в наборе инструментов Microsoft Graph
description: Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи. Она работает с любой из задач в планировщике (Майкрософт) или в Microsoft.
localization_priority: Normal
author: benotter
ms.openlocfilehash: 19faf3dec1c61680250cacf3cfaf5837b8bc4cee
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955850"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="67027-104">Компонент Tasks в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="67027-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="67027-105">Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи.</span><span class="sxs-lookup"><span data-stu-id="67027-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="67027-106">Она работает с задачами в планировщике (Майкрософт) или в Microsoft.</span><span class="sxs-lookup"><span data-stu-id="67027-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>  

<span data-ttu-id="67027-107">Кроме того, пользователь может назначить одну или несколько пользователей Microsoft Graph для задачи.</span><span class="sxs-lookup"><span data-stu-id="67027-107">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="67027-108">Более подробную информацию о назначениях Microsoft Graph можно узнать в разделе [планнерассигнментс](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="67027-108">For more details about Microsoft Graph assignments, see [plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span></span>

## <a name="example"></a><span data-ttu-id="67027-109">Пример</span><span class="sxs-lookup"><span data-stu-id="67027-109">Example</span></span>

[<span data-ttu-id="67027-110">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="67027-110">jsfiddle example</span></span>](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a><span data-ttu-id="67027-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="67027-111">Properties</span></span>

| <span data-ttu-id="67027-112">Атрибут</span><span class="sxs-lookup"><span data-stu-id="67027-112">Attribute</span></span> | <span data-ttu-id="67027-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="67027-113">Property</span></span> | <span data-ttu-id="67027-114">Описание</span><span class="sxs-lookup"><span data-stu-id="67027-114">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="67027-115">Data-Source = "TODO/Planner"</span><span class="sxs-lookup"><span data-stu-id="67027-115">data-source="todo/planner"</span></span> | <span data-ttu-id="67027-116">Данных</span><span class="sxs-lookup"><span data-stu-id="67027-116">dataSource</span></span> | <span data-ttu-id="67027-117">Перечисление для настройки источника данных задач — либо задачи Майкрософт, либо планировщика (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="67027-117">An enumeration to configure the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="67027-118">Значение по умолчанию: `planner`.</span><span class="sxs-lookup"><span data-stu-id="67027-118">Default is `planner`.</span></span> |
| <span data-ttu-id="67027-119">только для чтения</span><span class="sxs-lookup"><span data-stu-id="67027-119">read-only</span></span> | <span data-ttu-id="67027-120">Статического</span><span class="sxs-lookup"><span data-stu-id="67027-120">readOnly</span></span> | <span data-ttu-id="67027-121">Логическое значение, указывающее, что интерфейс задачи должен быть доступен только для чтения (Добавление или удаление задач не выполняется).</span><span class="sxs-lookup"><span data-stu-id="67027-121">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="67027-122">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="67027-122">Default is `false`.</span></span> |
| <span data-ttu-id="67027-123">скрыть — заголовок</span><span class="sxs-lookup"><span data-stu-id="67027-123">hide-header</span></span> | <span data-ttu-id="67027-124">хидехеадер</span><span class="sxs-lookup"><span data-stu-id="67027-124">hideHeader</span></span> | <span data-ttu-id="67027-125">Логическое значение для отображения или скрытия заголовка компонента.</span><span class="sxs-lookup"><span data-stu-id="67027-125">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="67027-126">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="67027-126">Default is `false`.</span></span> |
| <span data-ttu-id="67027-127">Initial-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="67027-127">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="67027-128">инитиалид</span><span class="sxs-lookup"><span data-stu-id="67027-128">initialId</span></span> | <span data-ttu-id="67027-129">Строковое значение, чтобы задать для первоначально отображаемого планировщика или папки предоставленный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="67027-129">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="67027-130">Initial — сегмент — ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="67027-130">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="67027-131">инитиалбуккетид</span><span class="sxs-lookup"><span data-stu-id="67027-131">initialBucketId</span></span> | <span data-ttu-id="67027-132">Строковый идентификатор для установки начального сегмента (только для источника данных с планировщиком) на предоставленный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="67027-132">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="67027-133">Target-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="67027-133">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="67027-134">targetId</span><span class="sxs-lookup"><span data-stu-id="67027-134">targetId</span></span> | <span data-ttu-id="67027-135">Идентификатор строки, чтобы заблокировать интерфейс Tasks до указанного планировщика или идентификатора папки.</span><span class="sxs-lookup"><span data-stu-id="67027-135">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="67027-136">Target — сегмент — ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="67027-136">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="67027-137">таржетбуккетид</span><span class="sxs-lookup"><span data-stu-id="67027-137">targetBucketId</span></span>  | <span data-ttu-id="67027-138">Идентификатор строки для блокировки интерфейса Tasks до указанного идентификатора контейнера (только для источника данных планировщика).</span><span class="sxs-lookup"><span data-stu-id="67027-138">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="67027-139">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="67027-139">group-id</span></span> | <span data-ttu-id="67027-140">groupId</span><span class="sxs-lookup"><span data-stu-id="67027-140">groupId</span></span>  | <span data-ttu-id="67027-141">Строковый идентификатор для блокировки интерфейса Tasks до идентификатора группы (только для источника данных планировщика).</span><span class="sxs-lookup"><span data-stu-id="67027-141">A string ID to lock the tasks interface to the group ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="67027-142">Н/Д</span><span class="sxs-lookup"><span data-stu-id="67027-142">N/A</span></span> | <span data-ttu-id="67027-143">исневтасквисибле</span><span class="sxs-lookup"><span data-stu-id="67027-143">isNewTaskVisible</span></span>  | <span data-ttu-id="67027-144">Определяет, отображается ли новое представление задач во время отображения.</span><span class="sxs-lookup"><span data-stu-id="67027-144">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="67027-145">Н/Д</span><span class="sxs-lookup"><span data-stu-id="67027-145">N/A</span></span> | <span data-ttu-id="67027-146">таскфилтер</span><span class="sxs-lookup"><span data-stu-id="67027-146">taskFilter</span></span>  | <span data-ttu-id="67027-147">Необязательная функция для фильтрации задач, которые отображаются для пользователя.</span><span class="sxs-lookup"><span data-stu-id="67027-147">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="67027-148">В следующем примере показаны задачи планировщика с ИДЕНТИФИКАТОРом *12345* , которые не позволяют пользователю создавать новые задачи.</span><span class="sxs-lookup"><span data-stu-id="67027-148">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="67027-149">В приведенном ниже примере показано, как фильтровать задачи, для которых только задано значение *Category3* .</span><span class="sxs-lookup"><span data-stu-id="67027-149">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="67027-150">Настраиваемые переменные CSS</span><span class="sxs-lookup"><span data-stu-id="67027-150">Custom CSS variables</span></span>

````css
mgt-tasks {
--tasks-header-padding
--tasks-header-margin 

--tasks-title-padding
--tasks-plan-title-font-size
--tasks-plan-title-padding

--tasks-new-button-width
--tasks-new-button-height
--tasks-new-button-color
--tasks-new-button-background
--tasks-new-button-border
--tasks-new-button-hover-background
--tasks-new-button-active-background

--tasks-new-task-name-margin

--task-margin
--task-box-shadow
--task-background
--task-border

--task-header-color
--task-header-margin

--task-detail-icon-margin

--task-new-margin
--task-new-border
--task-new-line-margin
--tasks-new-line-border
--task-new-input-margin
--task-new-input-padding
--task-new-input-font-size
--task-new-input-active-border
--task-new-select-border

--task-new-add-button-background
--task-new-add-button-disabled-background
--task-new-cancel-button-color

--task-complete-background
--task-complete-border
--task-complete-header-color
--task-complete-detail-color
--task-complete-detail-icon-color
}
````

## <a name="events"></a><span data-ttu-id="67027-151">События</span><span class="sxs-lookup"><span data-stu-id="67027-151">Events</span></span>
| <span data-ttu-id="67027-152">Событие</span><span class="sxs-lookup"><span data-stu-id="67027-152">Event</span></span> | <span data-ttu-id="67027-153">Detail (Сведения)</span><span class="sxs-lookup"><span data-stu-id="67027-153">Detail</span></span> | <span data-ttu-id="67027-154">Описание</span><span class="sxs-lookup"><span data-stu-id="67027-154">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="67027-155">тасккликк</span><span class="sxs-lookup"><span data-stu-id="67027-155">taskClick</span></span> | <span data-ttu-id="67027-156">Сведения содержит соответствующий `task` объект</span><span class="sxs-lookup"><span data-stu-id="67027-156">The detail contains the respective `task` object</span></span> | <span data-ttu-id="67027-157">Возникает, когда пользователь щелкает или нажимает задачу.</span><span class="sxs-lookup"><span data-stu-id="67027-157">Fired when the user clicks or taps on a task.</span></span> |

## <a name="templates"></a><span data-ttu-id="67027-158">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="67027-158">Templates</span></span>

<span data-ttu-id="67027-159">`tasks` Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="67027-159">The `tasks` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="67027-160">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="67027-160">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="67027-161">Тип данных</span><span class="sxs-lookup"><span data-stu-id="67027-161">Data type</span></span>     | <span data-ttu-id="67027-162">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="67027-162">Data context</span></span>              | <span data-ttu-id="67027-163">Описание</span><span class="sxs-lookup"><span data-stu-id="67027-163">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="67027-164">task</span><span class="sxs-lookup"><span data-stu-id="67027-164">task</span></span>     | <span data-ttu-id="67027-165">Задача: планировщик или объект задачи "задача"</span><span class="sxs-lookup"><span data-stu-id="67027-165">task: a planner or to-do task object</span></span> | <span data-ttu-id="67027-166">заменяет всю задачу по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="67027-166">replaces the whole default task.</span></span> |
| <span data-ttu-id="67027-167">Задача — сведения</span><span class="sxs-lookup"><span data-stu-id="67027-167">task-details</span></span> | <span data-ttu-id="67027-168">Задача: планировщик или объект задачи "задача"</span><span class="sxs-lookup"><span data-stu-id="67027-168">task: a planner or to-do task object</span></span> | <span data-ttu-id="67027-169">шаблон заменяет раздел сведений о задаче.</span><span class="sxs-lookup"><span data-stu-id="67027-169">template replaces the details section of the task.</span></span> |

<span data-ttu-id="67027-170">В следующем примере определяется шаблон для компонента Tasks.</span><span class="sxs-lookup"><span data-stu-id="67027-170">The following example defines a template for the tasks component.</span></span>

```html
    <mgt-tasks data-source="todo">
      <template data-type="task-details">
        <div>
          Owner: {{task.owner}}
        </div>
        <div>
          Importance Level: {{task.importance}}
        </div>
      </template>
    </mgt-tasks>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="67027-171">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="67027-171">Microsoft Graph permissions</span></span>

<span data-ttu-id="67027-172">Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="67027-172">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="67027-173">Resource</span><span class="sxs-lookup"><span data-stu-id="67027-173">Resource</span></span> | <span data-ttu-id="67027-174">Разрешение</span><span class="sxs-lookup"><span data-stu-id="67027-174">Permission</span></span> |
| - | - |
| <span data-ttu-id="67027-175">/ме/планнер/планс</span><span class="sxs-lookup"><span data-stu-id="67027-175">/me/planner/plans</span></span> | <span data-ttu-id="67027-176">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="67027-176">Group.Read.All</span></span> |
| <span data-ttu-id="67027-177">/Планнер/Планс/$ {ID}</span><span class="sxs-lookup"><span data-stu-id="67027-177">/planner/plans/${id}</span></span> | <span data-ttu-id="67027-178">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67027-178">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="67027-179">/планнер/таскс</span><span class="sxs-lookup"><span data-stu-id="67027-179">/planner/tasks</span></span> | <span data-ttu-id="67027-180">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67027-180">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="67027-181">/ме/аутлук/таскграупс</span><span class="sxs-lookup"><span data-stu-id="67027-181">/me/outlook/taskGroups</span></span> | <span data-ttu-id="67027-182">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="67027-182">Tasks.Read</span></span> |
| <span data-ttu-id="67027-183">/ме/аутлук/таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="67027-183">/me/outlook/taskFolders</span></span> | <span data-ttu-id="67027-184">Tasks. Read, Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67027-184">Tasks.Read, Tasks.ReadWrite</span></span> |
| <span data-ttu-id="67027-185">/ме/аутлук/таскс</span><span class="sxs-lookup"><span data-stu-id="67027-185">/me/outlook/tasks</span></span> | <span data-ttu-id="67027-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67027-186">Tasks.ReadWrite</span></span> |
| <span data-ttu-id="67027-187">/граупс/$ {Group – ID}/Планнер/Планс</span><span class="sxs-lookup"><span data-stu-id="67027-187">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="67027-188">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67027-188">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="67027-189">Для получения источника данных планировщика (Майкрософт) для получения и чтения задач требуются разрешения Group. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="67027-189">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="67027-190">Для добавления, обновления или удаления задач требуются разрешения Group. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="67027-190">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="67027-191">Для источника данных Microsoft TODO необходимо разрешение Tasks. Read для получения и чтения задач.</span><span class="sxs-lookup"><span data-stu-id="67027-191">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="67027-192">Для добавления, обновления или удаления задач требуется разрешение Tasks. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="67027-192">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="67027-193">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="67027-193">Authentication</span></span>

<span data-ttu-id="67027-194">Компонент Tasks использует глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="67027-194">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
