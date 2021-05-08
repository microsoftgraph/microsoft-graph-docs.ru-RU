---
title: Компонент задач в microsoft Graph набор средств
description: Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи. Он работает с любыми задачами в Microsoft Planner.
localization_priority: Normal
author: benotter
ms.openlocfilehash: d07db8f1a261f1cff96175a25665f08eff615d67
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266803"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="25626-104">Компонент задач в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="25626-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="25626-105">Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи из Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="25626-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks from Microsoft Planner.</span></span>  

<span data-ttu-id="25626-106">Кроме того, пользователь может назначить одной или нескольким пользователям Microsoft Graph задачу.</span><span class="sxs-lookup"><span data-stu-id="25626-106">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="25626-107">Дополнительные сведения о назначениях Microsoft Graph см. в [материале plannerAssignments.](/graph/api/resources/plannerassignments)</span><span class="sxs-lookup"><span data-stu-id="25626-107">For more details about Microsoft Graph assignments, see [plannerAssignments](/graph/api/resources/plannerassignments).</span></span>

## <a name="example"></a><span data-ttu-id="25626-108">Пример</span><span class="sxs-lookup"><span data-stu-id="25626-108">Example</span></span>

<span data-ttu-id="25626-109">В следующем примере отображаются задачи microsoft Planner пользователя, подписанные с помощью `mgt-tasks` компонента.</span><span class="sxs-lookup"><span data-stu-id="25626-109">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="25626-110">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="25626-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="25626-111">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="25626-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="25626-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="25626-112">Properties</span></span>

| <span data-ttu-id="25626-113">Атрибут</span><span class="sxs-lookup"><span data-stu-id="25626-113">Attribute</span></span> | <span data-ttu-id="25626-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="25626-114">Property</span></span> | <span data-ttu-id="25626-115">Описание</span><span class="sxs-lookup"><span data-stu-id="25626-115">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="25626-116">read-only</span><span class="sxs-lookup"><span data-stu-id="25626-116">read-only</span></span> | <span data-ttu-id="25626-117">readOnly</span><span class="sxs-lookup"><span data-stu-id="25626-117">readOnly</span></span> | <span data-ttu-id="25626-118">Логическое значение для настройки интерфейса задачи только для чтения (без добавления или удаления задач).</span><span class="sxs-lookup"><span data-stu-id="25626-118">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="25626-119">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="25626-119">Default is `false`.</span></span> |
| <span data-ttu-id="25626-120">hide-header</span><span class="sxs-lookup"><span data-stu-id="25626-120">hide-header</span></span> | <span data-ttu-id="25626-121">hideHeader</span><span class="sxs-lookup"><span data-stu-id="25626-121">hideHeader</span></span> | <span data-ttu-id="25626-122">Логическое значение для отображения или скрытия заголовка компонента.</span><span class="sxs-lookup"><span data-stu-id="25626-122">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="25626-123">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="25626-123">Default is `false`.</span></span> |
| <span data-ttu-id="25626-124">hide-options</span><span class="sxs-lookup"><span data-stu-id="25626-124">hide-options</span></span> | <span data-ttu-id="25626-125">hideOptions</span><span class="sxs-lookup"><span data-stu-id="25626-125">hideOptions</span></span> | <span data-ttu-id="25626-126">Логическое значение для отображения или скрытия параметров в задачах.</span><span class="sxs-lookup"><span data-stu-id="25626-126">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="25626-127">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="25626-127">Default is `false`.</span></span>
| <span data-ttu-id="25626-128">initial-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="25626-128">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="25626-129">initialId</span><span class="sxs-lookup"><span data-stu-id="25626-129">initialId</span></span> | <span data-ttu-id="25626-130">A string ID to set the initially displayed planner or folder to the provided ID.</span><span class="sxs-lookup"><span data-stu-id="25626-130">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="25626-131">initial-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="25626-131">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="25626-132">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="25626-132">initialBucketId</span></span> | <span data-ttu-id="25626-133">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span><span class="sxs-lookup"><span data-stu-id="25626-133">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="25626-134">target-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="25626-134">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="25626-135">targetId</span><span class="sxs-lookup"><span data-stu-id="25626-135">targetId</span></span> | <span data-ttu-id="25626-136">Строковый ID для блокировки интерфейса задач к предоставленной планировщику или папке.</span><span class="sxs-lookup"><span data-stu-id="25626-136">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="25626-137">target-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="25626-137">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="25626-138">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="25626-138">targetBucketId</span></span>  | <span data-ttu-id="25626-139">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span><span class="sxs-lookup"><span data-stu-id="25626-139">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="25626-140">group-id</span><span class="sxs-lookup"><span data-stu-id="25626-140">group-id</span></span> | <span data-ttu-id="25626-141">groupId</span><span class="sxs-lookup"><span data-stu-id="25626-141">groupId</span></span>  | <span data-ttu-id="25626-142">A string ID to lock the tasks interface to the group ID.</span><span class="sxs-lookup"><span data-stu-id="25626-142">A string ID to lock the tasks interface to the group ID.</span></span> |
| <span data-ttu-id="25626-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="25626-143">N/A</span></span> | <span data-ttu-id="25626-144">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="25626-144">isNewTaskVisible</span></span>  | <span data-ttu-id="25626-145">Определяет, отображается ли новое представление задач при визуализации.</span><span class="sxs-lookup"><span data-stu-id="25626-145">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="25626-146">Н/Д</span><span class="sxs-lookup"><span data-stu-id="25626-146">N/A</span></span> | <span data-ttu-id="25626-147">taskFilter</span><span class="sxs-lookup"><span data-stu-id="25626-147">taskFilter</span></span>  | <span data-ttu-id="25626-148">Необязательная функция для фильтрации задач, демонстрируемых пользователю.</span><span class="sxs-lookup"><span data-stu-id="25626-148">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="25626-149">В следующем примере показаны только задачи от Planner с ID *12345* и не позволяют пользователю создавать новые задачи.</span><span class="sxs-lookup"><span data-stu-id="25626-149">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="25626-150">В следующем примере показано, как фильтровать задачи, которые имеют только *набор category3.*</span><span class="sxs-lookup"><span data-stu-id="25626-150">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="25626-151">Настраиваемые переменные CSS</span><span class="sxs-lookup"><span data-stu-id="25626-151">Custom CSS variables</span></span>

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

## <a name="events"></a><span data-ttu-id="25626-152">События</span><span class="sxs-lookup"><span data-stu-id="25626-152">Events</span></span>
| <span data-ttu-id="25626-153">Событие</span><span class="sxs-lookup"><span data-stu-id="25626-153">Event</span></span> | <span data-ttu-id="25626-154">Сведения</span><span class="sxs-lookup"><span data-stu-id="25626-154">Detail</span></span> | <span data-ttu-id="25626-155">Описание</span><span class="sxs-lookup"><span data-stu-id="25626-155">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="25626-156">taskAdded</span><span class="sxs-lookup"><span data-stu-id="25626-156">taskAdded</span></span> | <span data-ttu-id="25626-157">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="25626-157">The detail contains the respective `task` object</span></span> | <span data-ttu-id="25626-158">Возникает при создании задачи.</span><span class="sxs-lookup"><span data-stu-id="25626-158">Fires when a new task has been created.</span></span> |
| <span data-ttu-id="25626-159">taskChanged</span><span class="sxs-lookup"><span data-stu-id="25626-159">taskChanged</span></span> | <span data-ttu-id="25626-160">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="25626-160">The detail contains the respective `task` object</span></span> | <span data-ttu-id="25626-161">Возникает при изменении метаданных задачи, например при пометке задачи как завершенной.</span><span class="sxs-lookup"><span data-stu-id="25626-161">Fires when task metadata has been changed, such as marking completed.</span></span> |
| <span data-ttu-id="25626-162">taskClick</span><span class="sxs-lookup"><span data-stu-id="25626-162">taskClick</span></span> | <span data-ttu-id="25626-163">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="25626-163">The detail contains the respective `task` object</span></span> | <span data-ttu-id="25626-164">Возникает, когда пользователь щелкает или нажимает задачу.</span><span class="sxs-lookup"><span data-stu-id="25626-164">Fires when the user clicks or taps on a task.</span></span> |
| <span data-ttu-id="25626-165">taskRemoved</span><span class="sxs-lookup"><span data-stu-id="25626-165">taskRemoved</span></span> | <span data-ttu-id="25626-166">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="25626-166">The detail contains the respective `task` object</span></span> | <span data-ttu-id="25626-167">Возникает, если удалена существующая задача.</span><span class="sxs-lookup"><span data-stu-id="25626-167">Fires when an existing task has been deleted.</span></span> |

## <a name="templates"></a><span data-ttu-id="25626-168">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="25626-168">Templates</span></span>

<span data-ttu-id="25626-169">Компонент `tasks` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="25626-169">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="25626-170">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и установите для параметра `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="25626-170">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="25626-171">Тип данных</span><span class="sxs-lookup"><span data-stu-id="25626-171">Data type</span></span>     | <span data-ttu-id="25626-172">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="25626-172">Data context</span></span>              | <span data-ttu-id="25626-173">Описание</span><span class="sxs-lookup"><span data-stu-id="25626-173">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="25626-174">task</span><span class="sxs-lookup"><span data-stu-id="25626-174">task</span></span>     | <span data-ttu-id="25626-175">задача: объект задачи планировщика</span><span class="sxs-lookup"><span data-stu-id="25626-175">task: a planner task object</span></span> | <span data-ttu-id="25626-176">заменяет всю задачу по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="25626-176">replaces the whole default task.</span></span> |
| <span data-ttu-id="25626-177">task-details</span><span class="sxs-lookup"><span data-stu-id="25626-177">task-details</span></span> | <span data-ttu-id="25626-178">задача: объект задачи планировщика</span><span class="sxs-lookup"><span data-stu-id="25626-178">task: a planner task object</span></span> | <span data-ttu-id="25626-179">шаблон заменяет раздел подробностей задачи.</span><span class="sxs-lookup"><span data-stu-id="25626-179">template replaces the details section of the task.</span></span> |

<span data-ttu-id="25626-180">В следующем примере определяется шаблон для компонента задач.</span><span class="sxs-lookup"><span data-stu-id="25626-180">The following example defines a template for the tasks component.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="25626-181">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="25626-181">Microsoft Graph permissions</span></span>

<span data-ttu-id="25626-182">Этот элемент управления использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="25626-182">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="25626-183">Ресурс</span><span class="sxs-lookup"><span data-stu-id="25626-183">Resource</span></span> | <span data-ttu-id="25626-184">Разрешение</span><span class="sxs-lookup"><span data-stu-id="25626-184">Permission</span></span> |
| - | - |
| <span data-ttu-id="25626-185">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="25626-185">/me/planner/plans</span></span> | <span data-ttu-id="25626-186">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="25626-186">Group.Read.All</span></span> |
| <span data-ttu-id="25626-187">/planner/plans/${id}</span><span class="sxs-lookup"><span data-stu-id="25626-187">/planner/plans/${id}</span></span> | <span data-ttu-id="25626-188">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25626-188">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="25626-189">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="25626-189">/planner/tasks</span></span> | <span data-ttu-id="25626-190">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25626-190">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="25626-191">/groups/${group-id}/planner/plans</span><span class="sxs-lookup"><span data-stu-id="25626-191">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="25626-192">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25626-192">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="25626-193">Для источника данных Microsoft Planner для получения и чтения требуется разрешение Groups.Read.All.</span><span class="sxs-lookup"><span data-stu-id="25626-193">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="25626-194">Добавление, обновление или удаление задач требует разрешения Groups.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="25626-194">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="25626-195">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="25626-195">Authentication</span></span>

<span data-ttu-id="25626-196">В компоненте задач используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="25626-196">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="25626-197">Кэш</span><span class="sxs-lookup"><span data-stu-id="25626-197">Cache</span></span>

<span data-ttu-id="25626-198">Компонент `mgt-tasks` не кэшет данных.</span><span class="sxs-lookup"><span data-stu-id="25626-198">The `mgt-tasks` component doesn't cache any data.</span></span>
