---
title: Компонент задач в microsoft Graph набор средств
description: Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи. Он работает с любыми задачами в Microsoft Planner.
localization_priority: Normal
author: benotter
ms.openlocfilehash: 3b3476751798dd5569218ec6acc6d09a91112fe6
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082036"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="fdc80-104">Компонент задач в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="fdc80-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="fdc80-105">Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи из Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="fdc80-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks from Microsoft Planner.</span></span>  

<span data-ttu-id="fdc80-106">Кроме того, пользователь может назначить одному или нескольким Graph Майкрософт задачу.</span><span class="sxs-lookup"><span data-stu-id="fdc80-106">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="fdc80-107">Дополнительные сведения о назначениях microsoft Graph см. [в материале plannerAssignments.](/graph/api/resources/plannerassignments)</span><span class="sxs-lookup"><span data-stu-id="fdc80-107">For more details about Microsoft Graph assignments, see [plannerAssignments](/graph/api/resources/plannerassignments).</span></span>

## <a name="example"></a><span data-ttu-id="fdc80-108">Пример</span><span class="sxs-lookup"><span data-stu-id="fdc80-108">Example</span></span>

<span data-ttu-id="fdc80-109">В следующем примере отображаются задачи microsoft Planner пользователя, подписанные с помощью `mgt-tasks` компонента.</span><span class="sxs-lookup"><span data-stu-id="fdc80-109">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="fdc80-110">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="fdc80-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="fdc80-111">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="fdc80-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="fdc80-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdc80-112">Properties</span></span>

| <span data-ttu-id="fdc80-113">Атрибут</span><span class="sxs-lookup"><span data-stu-id="fdc80-113">Attribute</span></span> | <span data-ttu-id="fdc80-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdc80-114">Property</span></span> | <span data-ttu-id="fdc80-115">Описание</span><span class="sxs-lookup"><span data-stu-id="fdc80-115">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="fdc80-116">read-only</span><span class="sxs-lookup"><span data-stu-id="fdc80-116">read-only</span></span> | <span data-ttu-id="fdc80-117">readOnly</span><span class="sxs-lookup"><span data-stu-id="fdc80-117">readOnly</span></span> | <span data-ttu-id="fdc80-118">Логическое значение для настройки интерфейса задачи только для чтения (без добавления или удаления задач).</span><span class="sxs-lookup"><span data-stu-id="fdc80-118">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="fdc80-119">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="fdc80-119">Default is `false`.</span></span> |
| <span data-ttu-id="fdc80-120">hide-header</span><span class="sxs-lookup"><span data-stu-id="fdc80-120">hide-header</span></span> | <span data-ttu-id="fdc80-121">hideHeader</span><span class="sxs-lookup"><span data-stu-id="fdc80-121">hideHeader</span></span> | <span data-ttu-id="fdc80-122">Логическое значение для отображения или скрытия заголовка компонента.</span><span class="sxs-lookup"><span data-stu-id="fdc80-122">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="fdc80-123">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="fdc80-123">Default is `false`.</span></span> |
| <span data-ttu-id="fdc80-124">hide-options</span><span class="sxs-lookup"><span data-stu-id="fdc80-124">hide-options</span></span> | <span data-ttu-id="fdc80-125">hideOptions</span><span class="sxs-lookup"><span data-stu-id="fdc80-125">hideOptions</span></span> | <span data-ttu-id="fdc80-126">Логическое значение для отображения или скрытия параметров в задачах.</span><span class="sxs-lookup"><span data-stu-id="fdc80-126">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="fdc80-127">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="fdc80-127">Default is `false`.</span></span>
| <span data-ttu-id="fdc80-128">initial-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="fdc80-128">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="fdc80-129">initialId</span><span class="sxs-lookup"><span data-stu-id="fdc80-129">initialId</span></span> | <span data-ttu-id="fdc80-130">A string ID to set the initially displayed planner or folder to the provided ID.</span><span class="sxs-lookup"><span data-stu-id="fdc80-130">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="fdc80-131">initial-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="fdc80-131">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="fdc80-132">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="fdc80-132">initialBucketId</span></span> | <span data-ttu-id="fdc80-133">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span><span class="sxs-lookup"><span data-stu-id="fdc80-133">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="fdc80-134">target-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="fdc80-134">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="fdc80-135">targetId</span><span class="sxs-lookup"><span data-stu-id="fdc80-135">targetId</span></span> | <span data-ttu-id="fdc80-136">Строковый ID для блокировки интерфейса задач к предоставленной планировщику или папке.</span><span class="sxs-lookup"><span data-stu-id="fdc80-136">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="fdc80-137">target-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="fdc80-137">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="fdc80-138">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="fdc80-138">targetBucketId</span></span>  | <span data-ttu-id="fdc80-139">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span><span class="sxs-lookup"><span data-stu-id="fdc80-139">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="fdc80-140">group-id</span><span class="sxs-lookup"><span data-stu-id="fdc80-140">group-id</span></span> | <span data-ttu-id="fdc80-141">groupId</span><span class="sxs-lookup"><span data-stu-id="fdc80-141">groupId</span></span>  | <span data-ttu-id="fdc80-142">A string ID to lock the tasks interface to the group ID.</span><span class="sxs-lookup"><span data-stu-id="fdc80-142">A string ID to lock the tasks interface to the group ID.</span></span> |
| <span data-ttu-id="fdc80-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fdc80-143">N/A</span></span> | <span data-ttu-id="fdc80-144">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="fdc80-144">isNewTaskVisible</span></span>  | <span data-ttu-id="fdc80-145">Определяет, отображается ли новое представление задач при визуализации.</span><span class="sxs-lookup"><span data-stu-id="fdc80-145">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="fdc80-146">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fdc80-146">N/A</span></span> | <span data-ttu-id="fdc80-147">taskFilter</span><span class="sxs-lookup"><span data-stu-id="fdc80-147">taskFilter</span></span>  | <span data-ttu-id="fdc80-148">Необязательная функция для фильтрации задач, демонстрируемых пользователю.</span><span class="sxs-lookup"><span data-stu-id="fdc80-148">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="fdc80-149">В следующем примере показаны только задачи от Planner с ID *12345* и не позволяют пользователю создавать новые задачи.</span><span class="sxs-lookup"><span data-stu-id="fdc80-149">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="fdc80-150">В следующем примере показано, как фильтровать задачи, которые имеют только *набор category3.*</span><span class="sxs-lookup"><span data-stu-id="fdc80-150">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="fdc80-151">Настраиваемые переменные CSS</span><span class="sxs-lookup"><span data-stu-id="fdc80-151">Custom CSS variables</span></span>

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

## <a name="events"></a><span data-ttu-id="fdc80-152">События</span><span class="sxs-lookup"><span data-stu-id="fdc80-152">Events</span></span>

| <span data-ttu-id="fdc80-153">Событие</span><span class="sxs-lookup"><span data-stu-id="fdc80-153">Event</span></span> | <span data-ttu-id="fdc80-154">Сведения</span><span class="sxs-lookup"><span data-stu-id="fdc80-154">Detail</span></span> | <span data-ttu-id="fdc80-155">Описание</span><span class="sxs-lookup"><span data-stu-id="fdc80-155">Description</span></span> |
| --- | --- | --- |
| `taskAdded` | <span data-ttu-id="fdc80-156">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="fdc80-156">The detail contains the respective `task` object</span></span> | <span data-ttu-id="fdc80-157">Возникает при создании задачи.</span><span class="sxs-lookup"><span data-stu-id="fdc80-157">Fires when a new task has been created.</span></span> |
| `taskChanged` | <span data-ttu-id="fdc80-158">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="fdc80-158">The detail contains the respective `task` object</span></span> | <span data-ttu-id="fdc80-159">Возникает при изменении метаданных задачи, например при пометке задачи как завершенной.</span><span class="sxs-lookup"><span data-stu-id="fdc80-159">Fires when task metadata has been changed, such as marking completed.</span></span> |
| `taskClick` | <span data-ttu-id="fdc80-160">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="fdc80-160">The detail contains the respective `task` object</span></span> | <span data-ttu-id="fdc80-161">Возникает, когда пользователь щелкает или нажимает задачу.</span><span class="sxs-lookup"><span data-stu-id="fdc80-161">Fires when the user clicks or taps on a task.</span></span> |
| `taskRemoved` | <span data-ttu-id="fdc80-162">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="fdc80-162">The detail contains the respective `task` object</span></span> | <span data-ttu-id="fdc80-163">Возникает, если удалена существующая задача.</span><span class="sxs-lookup"><span data-stu-id="fdc80-163">Fires when an existing task has been deleted.</span></span> |

<span data-ttu-id="fdc80-164">Дополнительные сведения об обработке событий см. в [этой работе.](../customize-components/events.md)</span><span class="sxs-lookup"><span data-stu-id="fdc80-164">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="fdc80-165">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="fdc80-165">Templates</span></span>

<span data-ttu-id="fdc80-166">Компонент `tasks` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="fdc80-166">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="fdc80-167">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и установите для параметра `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="fdc80-167">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="fdc80-168">Тип данных</span><span class="sxs-lookup"><span data-stu-id="fdc80-168">Data type</span></span>     | <span data-ttu-id="fdc80-169">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="fdc80-169">Data context</span></span>              | <span data-ttu-id="fdc80-170">Описание</span><span class="sxs-lookup"><span data-stu-id="fdc80-170">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="fdc80-171">task</span><span class="sxs-lookup"><span data-stu-id="fdc80-171">task</span></span>     | <span data-ttu-id="fdc80-172">задача: объект задачи планировщика</span><span class="sxs-lookup"><span data-stu-id="fdc80-172">task: a planner task object</span></span> | <span data-ttu-id="fdc80-173">заменяет всю задачу по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fdc80-173">replaces the whole default task.</span></span> |
| <span data-ttu-id="fdc80-174">task-details</span><span class="sxs-lookup"><span data-stu-id="fdc80-174">task-details</span></span> | <span data-ttu-id="fdc80-175">задача: объект задачи планировщика</span><span class="sxs-lookup"><span data-stu-id="fdc80-175">task: a planner task object</span></span> | <span data-ttu-id="fdc80-176">шаблон заменяет раздел подробностей задачи.</span><span class="sxs-lookup"><span data-stu-id="fdc80-176">template replaces the details section of the task.</span></span> |

<span data-ttu-id="fdc80-177">В следующем примере определяется шаблон для компонента задач.</span><span class="sxs-lookup"><span data-stu-id="fdc80-177">The following example defines a template for the tasks component.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="fdc80-178">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fdc80-178">Microsoft Graph permissions</span></span>

<span data-ttu-id="fdc80-179">Этот элемент управления использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fdc80-179">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="fdc80-180">Настройка</span><span class="sxs-lookup"><span data-stu-id="fdc80-180">Configuration</span></span> | <span data-ttu-id="fdc80-181">Разрешение</span><span class="sxs-lookup"><span data-stu-id="fdc80-181">Permission</span></span> | <span data-ttu-id="fdc80-182">API</span><span class="sxs-lookup"><span data-stu-id="fdc80-182">API</span></span> |
| ------------- | ---------- | --- |
| <span data-ttu-id="fdc80-183">`groupId` набор `dataSource` и заме- `TasksSource.planner`</span><span class="sxs-lookup"><span data-stu-id="fdc80-183">`groupId` set and `dataSource` set to `TasksSource.planner`</span></span> | <span data-ttu-id="fdc80-184">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdc80-184">Group.Read.All</span></span> | <span data-ttu-id="fdc80-185">[/groups/${group-id}/planner/plans](/graph/api/plannergroup-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="fdc80-185">[/groups/${group-id}/planner/plans](/graph/api/plannergroup-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span></span> |
| <span data-ttu-id="fdc80-186">`targetId` набор `dataSource` и заме- `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="fdc80-186">`targetId` set and `dataSource` set to `TasksSource.todo`</span></span> | <span data-ttu-id="fdc80-187">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fdc80-187">Tasks.Read</span></span> | <span data-ttu-id="fdc80-188">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="fdc80-188">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span></span> |
| <span data-ttu-id="fdc80-189">`targetId` установить и `dataSource` установить что-то другое, чем `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="fdc80-189">`targetId` set and `dataSource` set to something else than `TasksSource.todo`</span></span> | <span data-ttu-id="fdc80-190">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdc80-190">Group.Read.All</span></span> | <span data-ttu-id="fdc80-191">[/planner/plans/${planId}](/graph/api/plannerplan-get?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="fdc80-191">[/planner/plans/${planId}](/graph/api/plannerplan-get?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span></span> |
| <span data-ttu-id="fdc80-192">`dataSource` установлено, что `TasksSource.planner`</span><span class="sxs-lookup"><span data-stu-id="fdc80-192">`dataSource` set to `TasksSource.planner`</span></span> | <span data-ttu-id="fdc80-193">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdc80-193">Group.Read.All</span></span> | <span data-ttu-id="fdc80-194">[/me/planner/plans](/graph/api/planneruser-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="fdc80-194">[/me/planner/plans](/graph/api/planneruser-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span></span> |
| <span data-ttu-id="fdc80-195">`dataSource` установлено, что `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="fdc80-195">`dataSource` set to `TasksSource.todo`</span></span> | <span data-ttu-id="fdc80-196">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fdc80-196">Tasks.Read</span></span> | <span data-ttu-id="fdc80-197">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="fdc80-197">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span></span> |
| <span data-ttu-id="fdc80-198">`addTask` установлено `true` и `dataSource` установлено `TasksSource.planner`</span><span class="sxs-lookup"><span data-stu-id="fdc80-198">`addTask` set to `true` and `dataSource` set to `TasksSource.planner`</span></span> | <span data-ttu-id="fdc80-199">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdc80-199">Group.ReadWrite.All</span></span> | [<span data-ttu-id="fdc80-200">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="fdc80-200">/planner/tasks</span></span>](/graph/api/planner-post-tasks?view=graph-rest-1.0&tabs=http) |
| <span data-ttu-id="fdc80-201">`addTask` установлено `true` и `dataSource` установлено `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="fdc80-201">`addTask` set to `true` and `dataSource` set to `TasksSource.todo`</span></span> | <span data-ttu-id="fdc80-202">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdc80-202">Tasks.ReadWrite</span></span> | [<span data-ttu-id="fdc80-203">/me/outlook/taskFolders/${parentFolderId}/tasks</span><span class="sxs-lookup"><span data-stu-id="fdc80-203">/me/outlook/taskFolders/${parentFolderId}/tasks</span></span>](/graph/api/outlookuser-post-tasks?view=graph-rest-beta&tabs=csharp) |

<span data-ttu-id="fdc80-204">Для источника данных Microsoft Planner для получения и чтения требуется разрешение Groups.Read.All.</span><span class="sxs-lookup"><span data-stu-id="fdc80-204">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="fdc80-205">Добавление, обновление или удаление задач требует разрешения Groups.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="fdc80-205">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="fdc80-206">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="fdc80-206">Authentication</span></span>

<span data-ttu-id="fdc80-207">В компоненте задач используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="fdc80-207">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="fdc80-208">Кэш</span><span class="sxs-lookup"><span data-stu-id="fdc80-208">Cache</span></span>

<span data-ttu-id="fdc80-209">Компонент `mgt-tasks` не кэшет данных.</span><span class="sxs-lookup"><span data-stu-id="fdc80-209">The `mgt-tasks` component doesn't cache any data.</span></span>
