---
title: Компонент задач в microsoft Graph набор средств
description: Компонент "Задачи" позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи. Он работает с любыми задачами в Планировщике (Майкрософт).
localization_priority: Normal
author: benotter
ms.openlocfilehash: 5364491caae4edc9cd3f022937bcd6d809aa924f
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659216"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="37af8-104">Компонент задач в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="37af8-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="37af8-105">Компонент "Задачи" позволяет пользователю просматривать, добавлять, удалять, выполнять или редактировать задачи из Планировщика (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="37af8-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks from Microsoft Planner.</span></span>  

<span data-ttu-id="37af8-106">Кроме того, пользователь может назначить задачу одному или нескольким пользователям Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="37af8-106">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="37af8-107">Дополнительные сведения о назначениях Microsoft Graph см. в [записях plannerAssignments.](/graph/api/resources/plannerassignments)</span><span class="sxs-lookup"><span data-stu-id="37af8-107">For more details about Microsoft Graph assignments, see [plannerAssignments](/graph/api/resources/plannerassignments).</span></span>

## <a name="example"></a><span data-ttu-id="37af8-108">Пример</span><span class="sxs-lookup"><span data-stu-id="37af8-108">Example</span></span>

<span data-ttu-id="37af8-109">В следующем примере отображаются задачи, которые пользователь, вописав в планировщик Microsoft, использует `mgt-tasks` компонент.</span><span class="sxs-lookup"><span data-stu-id="37af8-109">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="37af8-110">С помощью редактора кода можно [увидеть,](#properties) как свойства изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="37af8-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="37af8-111">Откройте этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="37af8-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="37af8-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="37af8-112">Properties</span></span>

| <span data-ttu-id="37af8-113">Атрибут</span><span class="sxs-lookup"><span data-stu-id="37af8-113">Attribute</span></span> | <span data-ttu-id="37af8-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="37af8-114">Property</span></span> | <span data-ttu-id="37af8-115">Описание</span><span class="sxs-lookup"><span data-stu-id="37af8-115">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="37af8-116">только для чтения</span><span class="sxs-lookup"><span data-stu-id="37af8-116">read-only</span></span> | <span data-ttu-id="37af8-117">readOnly</span><span class="sxs-lookup"><span data-stu-id="37af8-117">readOnly</span></span> | <span data-ttu-id="37af8-118">Boolean, чтобы настроить интерфейс задачи только для чтения (без добавления или удаления задач).</span><span class="sxs-lookup"><span data-stu-id="37af8-118">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="37af8-119">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="37af8-119">Default is `false`.</span></span> |
| <span data-ttu-id="37af8-120">hide-header</span><span class="sxs-lookup"><span data-stu-id="37af8-120">hide-header</span></span> | <span data-ttu-id="37af8-121">hideHeader</span><span class="sxs-lookup"><span data-stu-id="37af8-121">hideHeader</span></span> | <span data-ttu-id="37af8-122">Boolean для показа или скрытие загона компонента.</span><span class="sxs-lookup"><span data-stu-id="37af8-122">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="37af8-123">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="37af8-123">Default is `false`.</span></span> |
| <span data-ttu-id="37af8-124">hide-options</span><span class="sxs-lookup"><span data-stu-id="37af8-124">hide-options</span></span> | <span data-ttu-id="37af8-125">hideOptions</span><span class="sxs-lookup"><span data-stu-id="37af8-125">hideOptions</span></span> | <span data-ttu-id="37af8-126">Boolean для показа или скрытие параметров в задачах.</span><span class="sxs-lookup"><span data-stu-id="37af8-126">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="37af8-127">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="37af8-127">Default is `false`.</span></span>
| <span data-ttu-id="37af8-128">initial-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="37af8-128">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="37af8-129">initialId</span><span class="sxs-lookup"><span data-stu-id="37af8-129">initialId</span></span> | <span data-ttu-id="37af8-130">Строковый ИД для первоначально отображаемого планировщика или папки в качестве предоставленного.</span><span class="sxs-lookup"><span data-stu-id="37af8-130">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="37af8-131">initial-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="37af8-131">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="37af8-132">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="37af8-132">initialBucketId</span></span> | <span data-ttu-id="37af8-133">Строковый ИД, чтобы установить для изначально отображаемого сегмента (Data-Source Только Планировщик) предоставленный ИД.</span><span class="sxs-lookup"><span data-stu-id="37af8-133">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="37af8-134">target-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="37af8-134">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="37af8-135">targetId</span><span class="sxs-lookup"><span data-stu-id="37af8-135">targetId</span></span> | <span data-ttu-id="37af8-136">Строковый ИД для блокировки интерфейса задач предоставленным планировщиком или идом папки.</span><span class="sxs-lookup"><span data-stu-id="37af8-136">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="37af8-137">target-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="37af8-137">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="37af8-138">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="37af8-138">targetBucketId</span></span>  | <span data-ttu-id="37af8-139">Строковый ИД для блокировки интерфейса задач с предоставленным идом сегмента (только Data-Source Планировщика).</span><span class="sxs-lookup"><span data-stu-id="37af8-139">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="37af8-140">group-id</span><span class="sxs-lookup"><span data-stu-id="37af8-140">group-id</span></span> | <span data-ttu-id="37af8-141">groupId</span><span class="sxs-lookup"><span data-stu-id="37af8-141">groupId</span></span>  | <span data-ttu-id="37af8-142">ИД строки для блокировки интерфейса задач с помощью ИД группы.</span><span class="sxs-lookup"><span data-stu-id="37af8-142">A string ID to lock the tasks interface to the group ID.</span></span> |
| <span data-ttu-id="37af8-143">Недоступно</span><span class="sxs-lookup"><span data-stu-id="37af8-143">N/A</span></span> | <span data-ttu-id="37af8-144">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="37af8-144">isNewTaskVisible</span></span>  | <span data-ttu-id="37af8-145">Определяет, отображается ли новое представление задачи при отрисовки.</span><span class="sxs-lookup"><span data-stu-id="37af8-145">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="37af8-146">Недоступно</span><span class="sxs-lookup"><span data-stu-id="37af8-146">N/A</span></span> | <span data-ttu-id="37af8-147">taskFilter</span><span class="sxs-lookup"><span data-stu-id="37af8-147">taskFilter</span></span>  | <span data-ttu-id="37af8-148">Необязательная функция для фильтрации задач, которые показываются пользователю.</span><span class="sxs-lookup"><span data-stu-id="37af8-148">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="37af8-149">В следующем примере показаны только задачи из Планировщика с ИД *12345* и не позволяют пользователю создавать новые задачи.</span><span class="sxs-lookup"><span data-stu-id="37af8-149">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="37af8-150">В следующем примере показано, как фильтровать задачи, для которые заданной только *категория 3.*</span><span class="sxs-lookup"><span data-stu-id="37af8-150">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="37af8-151">Настраиваемые переменные CSS</span><span class="sxs-lookup"><span data-stu-id="37af8-151">Custom CSS variables</span></span>

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

## <a name="events"></a><span data-ttu-id="37af8-152">События</span><span class="sxs-lookup"><span data-stu-id="37af8-152">Events</span></span>
| <span data-ttu-id="37af8-153">Событие</span><span class="sxs-lookup"><span data-stu-id="37af8-153">Event</span></span> | <span data-ttu-id="37af8-154">Сведения</span><span class="sxs-lookup"><span data-stu-id="37af8-154">Detail</span></span> | <span data-ttu-id="37af8-155">Описание</span><span class="sxs-lookup"><span data-stu-id="37af8-155">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="37af8-156">taskAdded</span><span class="sxs-lookup"><span data-stu-id="37af8-156">taskAdded</span></span> | <span data-ttu-id="37af8-157">Сведения содержат соответствующий `task` объект</span><span class="sxs-lookup"><span data-stu-id="37af8-157">The detail contains the respective `task` object</span></span> | <span data-ttu-id="37af8-158">Создается, когда создается новая задача.</span><span class="sxs-lookup"><span data-stu-id="37af8-158">Fires when a new task has been created.</span></span> |
| <span data-ttu-id="37af8-159">taskChanged</span><span class="sxs-lookup"><span data-stu-id="37af8-159">taskChanged</span></span> | <span data-ttu-id="37af8-160">Сведения содержат соответствующий `task` объект</span><span class="sxs-lookup"><span data-stu-id="37af8-160">The detail contains the respective `task` object</span></span> | <span data-ttu-id="37af8-161">Происходит, когда метаданные задачи были изменены, например после пометки.</span><span class="sxs-lookup"><span data-stu-id="37af8-161">Fires when task metadata has been changed, such as marking completed.</span></span> |
| <span data-ttu-id="37af8-162">taskClick</span><span class="sxs-lookup"><span data-stu-id="37af8-162">taskClick</span></span> | <span data-ttu-id="37af8-163">Сведения содержат соответствующий `task` объект</span><span class="sxs-lookup"><span data-stu-id="37af8-163">The detail contains the respective `task` object</span></span> | <span data-ttu-id="37af8-164">Происходит, когда пользователь щелкает или нажимает на задачу.</span><span class="sxs-lookup"><span data-stu-id="37af8-164">Fires when the user clicks or taps on a task.</span></span> |
| <span data-ttu-id="37af8-165">taskRemoved</span><span class="sxs-lookup"><span data-stu-id="37af8-165">taskRemoved</span></span> | <span data-ttu-id="37af8-166">Сведения содержат соответствующий `task` объект</span><span class="sxs-lookup"><span data-stu-id="37af8-166">The detail contains the respective `task` object</span></span> | <span data-ttu-id="37af8-167">Происходит при удалении существующей задачи.</span><span class="sxs-lookup"><span data-stu-id="37af8-167">Fires when an existing task has been deleted.</span></span> |

## <a name="templates"></a><span data-ttu-id="37af8-168">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="37af8-168">Templates</span></span>

<span data-ttu-id="37af8-169">Компонент `tasks` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые позволяют заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="37af8-169">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="37af8-170">Чтобы указать шаблон, включив элемент в компонент и заключив в него одно `<template>` `data-type` из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="37af8-170">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="37af8-171">Тип данных</span><span class="sxs-lookup"><span data-stu-id="37af8-171">Data type</span></span>     | <span data-ttu-id="37af8-172">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="37af8-172">Data context</span></span>              | <span data-ttu-id="37af8-173">Описание</span><span class="sxs-lookup"><span data-stu-id="37af8-173">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="37af8-174">task</span><span class="sxs-lookup"><span data-stu-id="37af8-174">task</span></span>     | <span data-ttu-id="37af8-175">task: объект задачи планировщика</span><span class="sxs-lookup"><span data-stu-id="37af8-175">task: a planner task object</span></span> | <span data-ttu-id="37af8-176">заменяет всю задачу по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="37af8-176">replaces the whole default task.</span></span> |
| <span data-ttu-id="37af8-177">task-details</span><span class="sxs-lookup"><span data-stu-id="37af8-177">task-details</span></span> | <span data-ttu-id="37af8-178">task: объект задачи планировщика</span><span class="sxs-lookup"><span data-stu-id="37af8-178">task: a planner task object</span></span> | <span data-ttu-id="37af8-179">шаблон заменяет раздел сведений о задаче.</span><span class="sxs-lookup"><span data-stu-id="37af8-179">template replaces the details section of the task.</span></span> |

<span data-ttu-id="37af8-180">В следующем примере определяется шаблон для компонента задач.</span><span class="sxs-lookup"><span data-stu-id="37af8-180">The following example defines a template for the tasks component.</span></span>

```html
    <mgt-tasks>
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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="37af8-181">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="37af8-181">Microsoft Graph permissions</span></span>

<span data-ttu-id="37af8-182">Этот контроль использует следующие API Microsoft Graph и разрешения.</span><span class="sxs-lookup"><span data-stu-id="37af8-182">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="37af8-183">Ресурс</span><span class="sxs-lookup"><span data-stu-id="37af8-183">Resource</span></span> | <span data-ttu-id="37af8-184">Разрешение</span><span class="sxs-lookup"><span data-stu-id="37af8-184">Permission</span></span> |
| - | - |
| <span data-ttu-id="37af8-185">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="37af8-185">/me/planner/plans</span></span> | <span data-ttu-id="37af8-186">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="37af8-186">Group.Read.All</span></span> |
| <span data-ttu-id="37af8-187">/planner/plans/${id}</span><span class="sxs-lookup"><span data-stu-id="37af8-187">/planner/plans/${id}</span></span> | <span data-ttu-id="37af8-188">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37af8-188">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="37af8-189">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="37af8-189">/planner/tasks</span></span> | <span data-ttu-id="37af8-190">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37af8-190">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="37af8-191">/groups/${group-id}/planner/plans</span><span class="sxs-lookup"><span data-stu-id="37af8-191">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="37af8-192">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37af8-192">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="37af8-193">Для источника данных Планировщика (Майкрософт) для получения и чтения задач требуется разрешение Groups.Read.All.</span><span class="sxs-lookup"><span data-stu-id="37af8-193">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="37af8-194">Для добавления, обновления или удаления задач требуется разрешение Groups.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="37af8-194">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="37af8-195">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="37af8-195">Authentication</span></span>

<span data-ttu-id="37af8-196">Компонент задач использует глобального поставщика проверки подлинности, описанного в [документации по проверке подлинности.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="37af8-196">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>