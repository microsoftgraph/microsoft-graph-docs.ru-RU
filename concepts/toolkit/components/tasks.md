---
title: Компонент Tasks в наборе инструментов Microsoft Graph
description: Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи. Она работает с любой из задач в планировщике (Майкрософт) или в Microsoft.
localization_priority: Normal
author: benotter
ms.openlocfilehash: cfd248ca7cb240cd724b8df863383b308121db4b
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144277"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="924e9-104">Компонент Tasks в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="924e9-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="924e9-105">Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи.</span><span class="sxs-lookup"><span data-stu-id="924e9-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="924e9-106">Она работает с задачами в планировщике (Майкрософт) или в Microsoft.</span><span class="sxs-lookup"><span data-stu-id="924e9-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>  

<span data-ttu-id="924e9-107">Кроме того, пользователь может назначить одну или несколько пользователей Microsoft Graph для задачи.</span><span class="sxs-lookup"><span data-stu-id="924e9-107">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="924e9-108">Более подробную информацию о назначениях Microsoft Graph можно узнать в разделе [планнерассигнментс](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="924e9-108">For more details about Microsoft Graph assignments, see [plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span></span>

## <a name="example"></a><span data-ttu-id="924e9-109">Пример</span><span class="sxs-lookup"><span data-stu-id="924e9-109">Example</span></span>

<span data-ttu-id="924e9-110">В следующем примере отображаются задачи планировщика Microsoft, вошедшего в систему, с `mgt-tasks` помощью компонента.</span><span class="sxs-lookup"><span data-stu-id="924e9-110">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="924e9-111">С помощью редактора кода можно увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="924e9-111">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="924e9-112">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="924e9-112">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="924e9-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="924e9-113">Properties</span></span>

| <span data-ttu-id="924e9-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="924e9-114">Attribute</span></span> | <span data-ttu-id="924e9-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="924e9-115">Property</span></span> | <span data-ttu-id="924e9-116">Описание</span><span class="sxs-lookup"><span data-stu-id="924e9-116">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="924e9-117">Data-Source = "TODO/Planner"</span><span class="sxs-lookup"><span data-stu-id="924e9-117">data-source="todo/planner"</span></span> | <span data-ttu-id="924e9-118">Данных</span><span class="sxs-lookup"><span data-stu-id="924e9-118">dataSource</span></span> | <span data-ttu-id="924e9-119">Перечисление для настройки источника данных задач — либо задачи Майкрософт, либо планировщика (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="924e9-119">An enumeration to configure the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="924e9-120">Значение по умолчанию: `planner`.</span><span class="sxs-lookup"><span data-stu-id="924e9-120">Default is `planner`.</span></span> |
| <span data-ttu-id="924e9-121">только для чтения</span><span class="sxs-lookup"><span data-stu-id="924e9-121">read-only</span></span> | <span data-ttu-id="924e9-122">Статического</span><span class="sxs-lookup"><span data-stu-id="924e9-122">readOnly</span></span> | <span data-ttu-id="924e9-123">Логическое значение, указывающее, что интерфейс задачи должен быть доступен только для чтения (Добавление или удаление задач не выполняется).</span><span class="sxs-lookup"><span data-stu-id="924e9-123">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="924e9-124">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="924e9-124">Default is `false`.</span></span> |
| <span data-ttu-id="924e9-125">скрыть — заголовок</span><span class="sxs-lookup"><span data-stu-id="924e9-125">hide-header</span></span> | <span data-ttu-id="924e9-126">хидехеадер</span><span class="sxs-lookup"><span data-stu-id="924e9-126">hideHeader</span></span> | <span data-ttu-id="924e9-127">Логическое значение для отображения или скрытия заголовка компонента.</span><span class="sxs-lookup"><span data-stu-id="924e9-127">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="924e9-128">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="924e9-128">Default is `false`.</span></span> |
| <span data-ttu-id="924e9-129">Параметры скрытия</span><span class="sxs-lookup"><span data-stu-id="924e9-129">hide-options</span></span> | <span data-ttu-id="924e9-130">хидеоптионс</span><span class="sxs-lookup"><span data-stu-id="924e9-130">hideOptions</span></span> | <span data-ttu-id="924e9-131">Логическое значение для отображения или скрытия параметров в разделе "задачи".</span><span class="sxs-lookup"><span data-stu-id="924e9-131">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="924e9-132">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="924e9-132">Default is `false`.</span></span>
| <span data-ttu-id="924e9-133">Initial-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="924e9-133">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="924e9-134">инитиалид</span><span class="sxs-lookup"><span data-stu-id="924e9-134">initialId</span></span> | <span data-ttu-id="924e9-135">Строковое значение, чтобы задать для первоначально отображаемого планировщика или папки предоставленный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="924e9-135">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="924e9-136">Initial — сегмент — ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="924e9-136">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="924e9-137">инитиалбуккетид</span><span class="sxs-lookup"><span data-stu-id="924e9-137">initialBucketId</span></span> | <span data-ttu-id="924e9-138">Строковый идентификатор для установки начального сегмента (только для источника данных с планировщиком) на предоставленный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="924e9-138">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="924e9-139">Target-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="924e9-139">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="924e9-140">targetId</span><span class="sxs-lookup"><span data-stu-id="924e9-140">targetId</span></span> | <span data-ttu-id="924e9-141">Идентификатор строки, чтобы заблокировать интерфейс Tasks до указанного планировщика или идентификатора папки.</span><span class="sxs-lookup"><span data-stu-id="924e9-141">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="924e9-142">Target — сегмент — ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="924e9-142">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="924e9-143">таржетбуккетид</span><span class="sxs-lookup"><span data-stu-id="924e9-143">targetBucketId</span></span>  | <span data-ttu-id="924e9-144">Идентификатор строки для блокировки интерфейса Tasks до указанного идентификатора контейнера (только для источника данных планировщика).</span><span class="sxs-lookup"><span data-stu-id="924e9-144">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="924e9-145">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="924e9-145">group-id</span></span> | <span data-ttu-id="924e9-146">groupId</span><span class="sxs-lookup"><span data-stu-id="924e9-146">groupId</span></span>  | <span data-ttu-id="924e9-147">Строковый идентификатор для блокировки интерфейса Tasks до идентификатора группы (только для источника данных планировщика).</span><span class="sxs-lookup"><span data-stu-id="924e9-147">A string ID to lock the tasks interface to the group ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="924e9-148">Н/Д</span><span class="sxs-lookup"><span data-stu-id="924e9-148">N/A</span></span> | <span data-ttu-id="924e9-149">исневтасквисибле</span><span class="sxs-lookup"><span data-stu-id="924e9-149">isNewTaskVisible</span></span>  | <span data-ttu-id="924e9-150">Определяет, отображается ли новое представление задач во время отображения.</span><span class="sxs-lookup"><span data-stu-id="924e9-150">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="924e9-151">Н/Д</span><span class="sxs-lookup"><span data-stu-id="924e9-151">N/A</span></span> | <span data-ttu-id="924e9-152">таскфилтер</span><span class="sxs-lookup"><span data-stu-id="924e9-152">taskFilter</span></span>  | <span data-ttu-id="924e9-153">Необязательная функция для фильтрации задач, которые отображаются для пользователя.</span><span class="sxs-lookup"><span data-stu-id="924e9-153">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="924e9-154">В следующем примере показаны задачи планировщика с ИДЕНТИФИКАТОРом *12345* , которые не позволяют пользователю создавать новые задачи.</span><span class="sxs-lookup"><span data-stu-id="924e9-154">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="924e9-155">В приведенном ниже примере показано, как фильтровать задачи, для которых только задано значение *Category3* .</span><span class="sxs-lookup"><span data-stu-id="924e9-155">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="924e9-156">Настраиваемые переменные CSS</span><span class="sxs-lookup"><span data-stu-id="924e9-156">Custom CSS variables</span></span>

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

--task-icon-background-completed
--task-icon-background

--task-icon-border-completed
--task-icon-border

--task-icon-color
--task-icon-color-completed

--task-icon-border-radius

--task-icon-alignment: flex-start (default) | center | flex-end
}
````

## <a name="events"></a><span data-ttu-id="924e9-157">Мероприятия</span><span class="sxs-lookup"><span data-stu-id="924e9-157">Events</span></span>
| <span data-ttu-id="924e9-158">Событие</span><span class="sxs-lookup"><span data-stu-id="924e9-158">Event</span></span> | <span data-ttu-id="924e9-159">Detail (Сведения)</span><span class="sxs-lookup"><span data-stu-id="924e9-159">Detail</span></span> | <span data-ttu-id="924e9-160">Описание</span><span class="sxs-lookup"><span data-stu-id="924e9-160">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="924e9-161">тасккликк</span><span class="sxs-lookup"><span data-stu-id="924e9-161">taskClick</span></span> | <span data-ttu-id="924e9-162">Сведения содержит соответствующий `task` объект</span><span class="sxs-lookup"><span data-stu-id="924e9-162">The detail contains the respective `task` object</span></span> | <span data-ttu-id="924e9-163">Возникает, когда пользователь щелкает или нажимает задачу.</span><span class="sxs-lookup"><span data-stu-id="924e9-163">Fired when the user clicks or taps on a task.</span></span> |

## <a name="templates"></a><span data-ttu-id="924e9-164">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="924e9-164">Templates</span></span>

<span data-ttu-id="924e9-165">`tasks` Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="924e9-165">The `tasks` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="924e9-166">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="924e9-166">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="924e9-167">Тип данных</span><span class="sxs-lookup"><span data-stu-id="924e9-167">Data type</span></span>     | <span data-ttu-id="924e9-168">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="924e9-168">Data context</span></span>              | <span data-ttu-id="924e9-169">Описание</span><span class="sxs-lookup"><span data-stu-id="924e9-169">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="924e9-170">task</span><span class="sxs-lookup"><span data-stu-id="924e9-170">task</span></span>     | <span data-ttu-id="924e9-171">Задача: планировщик или объект задачи "задача"</span><span class="sxs-lookup"><span data-stu-id="924e9-171">task: a planner or to-do task object</span></span> | <span data-ttu-id="924e9-172">заменяет всю задачу по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="924e9-172">replaces the whole default task.</span></span> |
| <span data-ttu-id="924e9-173">Задача — сведения</span><span class="sxs-lookup"><span data-stu-id="924e9-173">task-details</span></span> | <span data-ttu-id="924e9-174">Задача: планировщик или объект задачи "задача"</span><span class="sxs-lookup"><span data-stu-id="924e9-174">task: a planner or to-do task object</span></span> | <span data-ttu-id="924e9-175">шаблон заменяет раздел сведений о задаче.</span><span class="sxs-lookup"><span data-stu-id="924e9-175">template replaces the details section of the task.</span></span> |

<span data-ttu-id="924e9-176">В следующем примере определяется шаблон для компонента Tasks.</span><span class="sxs-lookup"><span data-stu-id="924e9-176">The following example defines a template for the tasks component.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="924e9-177">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="924e9-177">Microsoft Graph permissions</span></span>

<span data-ttu-id="924e9-178">Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="924e9-178">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="924e9-179">Ресурс</span><span class="sxs-lookup"><span data-stu-id="924e9-179">Resource</span></span> | <span data-ttu-id="924e9-180">Разрешение</span><span class="sxs-lookup"><span data-stu-id="924e9-180">Permission</span></span> |
| - | - |
| <span data-ttu-id="924e9-181">/ме/планнер/планс</span><span class="sxs-lookup"><span data-stu-id="924e9-181">/me/planner/plans</span></span> | <span data-ttu-id="924e9-182">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="924e9-182">Group.Read.All</span></span> |
| <span data-ttu-id="924e9-183">/Планнер/Планс/$ {ID}</span><span class="sxs-lookup"><span data-stu-id="924e9-183">/planner/plans/${id}</span></span> | <span data-ttu-id="924e9-184">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="924e9-184">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="924e9-185">/планнер/таскс</span><span class="sxs-lookup"><span data-stu-id="924e9-185">/planner/tasks</span></span> | <span data-ttu-id="924e9-186">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="924e9-186">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="924e9-187">/ме/аутлук/таскграупс</span><span class="sxs-lookup"><span data-stu-id="924e9-187">/me/outlook/taskGroups</span></span> | <span data-ttu-id="924e9-188">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="924e9-188">Tasks.Read</span></span> |
| <span data-ttu-id="924e9-189">/ме/аутлук/таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="924e9-189">/me/outlook/taskFolders</span></span> | <span data-ttu-id="924e9-190">Tasks. Read, Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="924e9-190">Tasks.Read, Tasks.ReadWrite</span></span> |
| <span data-ttu-id="924e9-191">/ме/аутлук/таскс</span><span class="sxs-lookup"><span data-stu-id="924e9-191">/me/outlook/tasks</span></span> | <span data-ttu-id="924e9-192">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="924e9-192">Tasks.ReadWrite</span></span> |
| <span data-ttu-id="924e9-193">/граупс/$ {Group – ID}/Планнер/Планс</span><span class="sxs-lookup"><span data-stu-id="924e9-193">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="924e9-194">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="924e9-194">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="924e9-195">Для получения источника данных планировщика (Майкрософт) для получения и чтения задач требуются разрешения Group. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="924e9-195">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="924e9-196">Для добавления, обновления или удаления задач требуются разрешения Group. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="924e9-196">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="924e9-197">Для источника данных Microsoft TODO необходимо разрешение Tasks. Read для получения и чтения задач.</span><span class="sxs-lookup"><span data-stu-id="924e9-197">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="924e9-198">Для добавления, обновления или удаления задач требуется разрешение Tasks. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="924e9-198">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="924e9-199">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="924e9-199">Authentication</span></span>

<span data-ttu-id="924e9-200">Компонент Tasks использует глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="924e9-200">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
