---
title: Компонент To Do в Microsoft Graph Toolkit
description: Компонент To Do позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи To Do. Он поддерживает любые задачи в Microsoft To-Do.
localization_priority: Normal
author: shweaver-MSFT
ms.openlocfilehash: 3eb91bc23f1159e08749b6e6b073939bacca0c5c
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781004"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d7b34-104">Компонент To Do в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="d7b34-104">To Do component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d7b34-105">Компонент To Do используется, чтобы позволить вошедшему пользователю просматривать, добавлять, удалять, выполнять и/или изменять задачи из Microsoft To Do с помощью API To Do в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d7b34-105">The To Do component is used to enable the signed-in user to view, add, remove, complete, and/or edit tasks from Microsoft To Do using the To Do API in Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="d7b34-106">Пример</span><span class="sxs-lookup"><span data-stu-id="d7b34-106">Example</span></span>

<span data-ttu-id="d7b34-107">В следующем примере отображаются задачи Microsoft To Do вошедшего пользователя с помощью компонента `mgt-todo`.</span><span class="sxs-lookup"><span data-stu-id="d7b34-107">The following example displays the signed-in user's Microsoft To Do tasks using the `mgt-todo` component.</span></span> <span data-ttu-id="d7b34-108">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="d7b34-108">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="d7b34-109">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="d7b34-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="d7b34-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7b34-110">Properties</span></span>

<span data-ttu-id="d7b34-111">Для настройки компонента можно использовать следующие атрибуты и свойства.</span><span class="sxs-lookup"><span data-stu-id="d7b34-111">You can use the following attributes and properties to customize the component.</span></span>

| <span data-ttu-id="d7b34-112">Атрибут</span><span class="sxs-lookup"><span data-stu-id="d7b34-112">Attribute</span></span> | <span data-ttu-id="d7b34-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7b34-113">Property</span></span> | <span data-ttu-id="d7b34-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d7b34-114">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="d7b34-115">read-only</span><span class="sxs-lookup"><span data-stu-id="d7b34-115">read-only</span></span> | <span data-ttu-id="d7b34-116">readOnly</span><span class="sxs-lookup"><span data-stu-id="d7b34-116">readOnly</span></span> | <span data-ttu-id="d7b34-117">Логическое значение для настройки интерфейса задачи только для чтения (без добавления или удаления задач).</span><span class="sxs-lookup"><span data-stu-id="d7b34-117">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="d7b34-118">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="d7b34-118">Default is `false`.</span></span> |
| <span data-ttu-id="d7b34-119">hide-header</span><span class="sxs-lookup"><span data-stu-id="d7b34-119">hide-header</span></span> | <span data-ttu-id="d7b34-120">hideHeader</span><span class="sxs-lookup"><span data-stu-id="d7b34-120">hideHeader</span></span> | <span data-ttu-id="d7b34-121">Логическое значение для отображения или скрытия заголовка компонента.</span><span class="sxs-lookup"><span data-stu-id="d7b34-121">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="d7b34-122">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="d7b34-122">Default is `false`.</span></span> |
| <span data-ttu-id="d7b34-123">hide-options</span><span class="sxs-lookup"><span data-stu-id="d7b34-123">hide-options</span></span> | <span data-ttu-id="d7b34-124">hideOptions</span><span class="sxs-lookup"><span data-stu-id="d7b34-124">hideOptions</span></span> | <span data-ttu-id="d7b34-125">Логическое значение для отображения или скрытия параметров в задачах.</span><span class="sxs-lookup"><span data-stu-id="d7b34-125">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="d7b34-126">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="d7b34-126">Default is `false`.</span></span>
| <span data-ttu-id="d7b34-127">initial-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="d7b34-127">initial-id="folder_id"</span></span> | <span data-ttu-id="d7b34-128">initialId</span><span class="sxs-lookup"><span data-stu-id="d7b34-128">initialId</span></span> | <span data-ttu-id="d7b34-129">Строковый идентификатор, чтобы настроить для изначально отображаемой папки указанный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="d7b34-129">A string ID to set the initially displayed folder to the provided ID.</span></span> |
| <span data-ttu-id="d7b34-130">target-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="d7b34-130">target-id="folder_id"</span></span>| <span data-ttu-id="d7b34-131">targetId</span><span class="sxs-lookup"><span data-stu-id="d7b34-131">targetId</span></span> | <span data-ttu-id="d7b34-132">Строковый идентификатор для блокировки интерфейса задач по указанному идентификатору папки.</span><span class="sxs-lookup"><span data-stu-id="d7b34-132">A string ID to lock the tasks interface to the provided folder ID.</span></span> |
| <span data-ttu-id="d7b34-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d7b34-133">N/A</span></span> | <span data-ttu-id="d7b34-134">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="d7b34-134">isNewTaskVisible</span></span>  | <span data-ttu-id="d7b34-135">Определяет, отображается ли новое представление задач при визуализации.</span><span class="sxs-lookup"><span data-stu-id="d7b34-135">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="d7b34-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d7b34-136">N/A</span></span> | <span data-ttu-id="d7b34-137">taskFilter</span><span class="sxs-lookup"><span data-stu-id="d7b34-137">taskFilter</span></span>  | <span data-ttu-id="d7b34-138">Необязательная функция для фильтрации задач, демонстрируемых пользователю.</span><span class="sxs-lookup"><span data-stu-id="d7b34-138">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="d7b34-139">В следующем примере показаны только задачи из папки с идентификатором *12345*, и пользователю не разрешается создавать новые задачи.</span><span class="sxs-lookup"><span data-stu-id="d7b34-139">The following example shows only tasks from the folder with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a><span data-ttu-id="d7b34-140">Настраиваемые переменные CSS</span><span class="sxs-lookup"><span data-stu-id="d7b34-140">Custom CSS variables</span></span>

<span data-ttu-id="d7b34-141">Компонент `mgt-todo` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="d7b34-141">The `mgt-todo` component defines the following CSS custom properties.</span></span>

````css
mgt-todo {
  --tasks-background-color
  --tasks-header-padding
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

  --task-margin
  --task-background
  --task-border
  --task-header-color
  --task-header-margin

  --task-new-margin
  --task-new-border
  --task-new-input-margin
  --task-new-input-padding
  --task-new-input-font-size
  --task-new-select-border

  --task-new-add-button-background
  --task-new-add-button-disabled-background
  --task-new-cancel-button-color

  --task-complete-background
  --task-complete-border

  --task-icon-alignment: flex-start (default) | center | flex-end
  --task-icon-background
  --task-icon-background-completed
  --task-icon-border
  --task-icon-border-completed
  --task-icon-border-radius
  --task-icon-color
  --task-icon-color-completed
}
````

<span data-ttu-id="d7b34-142">Дополнительные сведения см. в статье [Компоненты стиля](https://docs.microsoft.com/graph/toolkit/style.md).</span><span class="sxs-lookup"><span data-stu-id="d7b34-142">To learn more, see [styling components](https://docs.microsoft.com/graph/toolkit/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="d7b34-143">События</span><span class="sxs-lookup"><span data-stu-id="d7b34-143">Events</span></span>

<span data-ttu-id="d7b34-144">Из компонента инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="d7b34-144">The following events are fired from the component.</span></span>

| <span data-ttu-id="d7b34-145">Событие</span><span class="sxs-lookup"><span data-stu-id="d7b34-145">Event</span></span> | <span data-ttu-id="d7b34-146">Сведения</span><span class="sxs-lookup"><span data-stu-id="d7b34-146">Detail</span></span> | <span data-ttu-id="d7b34-147">Описание</span><span class="sxs-lookup"><span data-stu-id="d7b34-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="d7b34-148">taskAdded</span><span class="sxs-lookup"><span data-stu-id="d7b34-148">taskAdded</span></span> | <span data-ttu-id="d7b34-149">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="d7b34-149">The detail contains the respective `task` object</span></span> | <span data-ttu-id="d7b34-150">Возникает при создании задачи.</span><span class="sxs-lookup"><span data-stu-id="d7b34-150">Fires when a new task has been created.</span></span> |
| <span data-ttu-id="d7b34-151">taskChanged</span><span class="sxs-lookup"><span data-stu-id="d7b34-151">taskChanged</span></span> | <span data-ttu-id="d7b34-152">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="d7b34-152">The detail contains the respective `task` object</span></span> | <span data-ttu-id="d7b34-153">Возникает при изменении метаданных задачи, например при пометке задачи как завершенной.</span><span class="sxs-lookup"><span data-stu-id="d7b34-153">Fires when task metadata has been changed, such as marking completed.</span></span> |
| <span data-ttu-id="d7b34-154">taskClick</span><span class="sxs-lookup"><span data-stu-id="d7b34-154">taskClick</span></span> | <span data-ttu-id="d7b34-155">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="d7b34-155">The detail contains the respective `task` object</span></span> | <span data-ttu-id="d7b34-156">Возникает, когда пользователь щелкает или нажимает задачу.</span><span class="sxs-lookup"><span data-stu-id="d7b34-156">Fires when the user clicks or taps on a task.</span></span> |
| <span data-ttu-id="d7b34-157">taskRemoved</span><span class="sxs-lookup"><span data-stu-id="d7b34-157">taskRemoved</span></span> | <span data-ttu-id="d7b34-158">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="d7b34-158">The detail contains the respective `task` object</span></span> | <span data-ttu-id="d7b34-159">Возникает, если удалена существующая задача.</span><span class="sxs-lookup"><span data-stu-id="d7b34-159">Fires when an existing task has been deleted.</span></span> |

## <a name="templates"></a><span data-ttu-id="d7b34-160">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="d7b34-160">Templates</span></span>

<span data-ttu-id="d7b34-161">Компонент `tasks` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="d7b34-161">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="d7b34-162">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="d7b34-162">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="d7b34-163">Тип данных</span><span class="sxs-lookup"><span data-stu-id="d7b34-163">Data type</span></span>     | <span data-ttu-id="d7b34-164">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="d7b34-164">Data context</span></span>              | <span data-ttu-id="d7b34-165">Описание</span><span class="sxs-lookup"><span data-stu-id="d7b34-165">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="d7b34-166">task</span><span class="sxs-lookup"><span data-stu-id="d7b34-166">task</span></span>     | <span data-ttu-id="d7b34-167">задача: объект задачи To-Do</span><span class="sxs-lookup"><span data-stu-id="d7b34-167">task: a to-do task object</span></span> | <span data-ttu-id="d7b34-168">Заменяет всю стандартную задачу.</span><span class="sxs-lookup"><span data-stu-id="d7b34-168">Replaces the whole default task.</span></span> |
| <span data-ttu-id="d7b34-169">task-details</span><span class="sxs-lookup"><span data-stu-id="d7b34-169">task-details</span></span> | <span data-ttu-id="d7b34-170">задача: объект задачи To-Do</span><span class="sxs-lookup"><span data-stu-id="d7b34-170">task: a to-do task object</span></span> | <span data-ttu-id="d7b34-171">Шаблон заменит раздел сведений задачи.</span><span class="sxs-lookup"><span data-stu-id="d7b34-171">Template replaces the details section of the task.</span></span> |

<span data-ttu-id="d7b34-172">В следующем примере определяется шаблон для компонента задач.</span><span class="sxs-lookup"><span data-stu-id="d7b34-172">The following example defines a template for the tasks component.</span></span>

```html
<mgt-todo>
    <template data-type="task-details">
        <div>
            Importance Level: {{task.importance}}
        </div>
    </template>
</mgt-todo>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="d7b34-173">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d7b34-173">Microsoft Graph permissions</span></span>

<span data-ttu-id="d7b34-174">Этот элемент управления использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d7b34-174">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="d7b34-175">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="d7b34-175">Configuration</span></span> | <span data-ttu-id="d7b34-176">Разрешение</span><span class="sxs-lookup"><span data-stu-id="d7b34-176">Permission</span></span> | <span data-ttu-id="d7b34-177">API</span><span class="sxs-lookup"><span data-stu-id="d7b34-177">API</span></span> |
| ------------- | ---------- | --- |
| <span data-ttu-id="d7b34-178">`targetId` set</span><span class="sxs-lookup"><span data-stu-id="d7b34-178">`targetId` set</span></span> | <span data-ttu-id="d7b34-179">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d7b34-179">Tasks.Read</span></span> | <span data-ttu-id="d7b34-180">[/me/todo/lists/${listId}](/graph/api/todotasklist-get?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span><span class="sxs-lookup"><span data-stu-id="d7b34-180">[/me/todo/lists/${listId}](/graph/api/todotasklist-get?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span></span> |
| <span data-ttu-id="d7b34-181">`targetId` не установлено</span><span class="sxs-lookup"><span data-stu-id="d7b34-181">`targetId` not set</span></span> | <span data-ttu-id="d7b34-182">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d7b34-182">Tasks.Read</span></span> | <span data-ttu-id="d7b34-183">[/me/todo/lists](/graph/api/todo-list-lists?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span><span class="sxs-lookup"><span data-stu-id="d7b34-183">[/me/todo/lists](/graph/api/todo-list-lists?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span></span> |
| <span data-ttu-id="d7b34-184">создание, обновление или удаление задачи</span><span class="sxs-lookup"><span data-stu-id="d7b34-184">create, update or delete task</span></span> | <span data-ttu-id="d7b34-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7b34-185">Tasks.ReadWrite</span></span> | [<span data-ttu-id="d7b34-186">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span><span class="sxs-lookup"><span data-stu-id="d7b34-186">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span></span>](/graph/api/todotask-get) |

## <a name="authentication"></a><span data-ttu-id="d7b34-187">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="d7b34-187">Authentication</span></span>

<span data-ttu-id="d7b34-188">В компоненте задач используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="d7b34-188">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="d7b34-189">Кэш</span><span class="sxs-lookup"><span data-stu-id="d7b34-189">Cache</span></span>

<span data-ttu-id="d7b34-190">Компонент `mgt-todo` не кэшет данных.</span><span class="sxs-lookup"><span data-stu-id="d7b34-190">The `mgt-todo` component doesn't cache any data.</span></span>
