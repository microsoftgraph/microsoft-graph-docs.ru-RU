---
title: Компонент To Do в Microsoft Graph Toolkit
description: Компонент To Do позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи To Do. Он поддерживает любые задачи в Microsoft To-Do.
localization_priority: Normal
author: shweaver-MSFT
ms.openlocfilehash: 1a00d045da55dc14da47770b0e56522590f4b5bc
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659172"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="343e2-104">Компонент To Do в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="343e2-104">To Do component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="343e2-105">Компонент To Do используется, чтобы позволить вошедшему пользователю просматривать, добавлять, удалять, выполнять и/или изменять задачи из Microsoft To Do с помощью API To Do в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="343e2-105">The To Do component is used to enable the signed-in user to view, add, remove, complete, and/or edit tasks from Microsoft To Do using the To Do API in Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="343e2-106">Пример</span><span class="sxs-lookup"><span data-stu-id="343e2-106">Example</span></span>

<span data-ttu-id="343e2-107">В следующем примере отображаются задачи Microsoft To Do вошедшего пользователя с помощью компонента `mgt-todo`.</span><span class="sxs-lookup"><span data-stu-id="343e2-107">The following example displays the signed-in user's Microsoft To Do tasks using the `mgt-todo` component.</span></span> <span data-ttu-id="343e2-108">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="343e2-108">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="343e2-109">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="343e2-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="343e2-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="343e2-110">Properties</span></span>

<span data-ttu-id="343e2-111">Для настройки компонента можно использовать следующие атрибуты и свойства.</span><span class="sxs-lookup"><span data-stu-id="343e2-111">You can use the following attributes and properties to customize the component.</span></span>

| <span data-ttu-id="343e2-112">Атрибут</span><span class="sxs-lookup"><span data-stu-id="343e2-112">Attribute</span></span> | <span data-ttu-id="343e2-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="343e2-113">Property</span></span> | <span data-ttu-id="343e2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="343e2-114">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="343e2-115">read-only</span><span class="sxs-lookup"><span data-stu-id="343e2-115">read-only</span></span> | <span data-ttu-id="343e2-116">readOnly</span><span class="sxs-lookup"><span data-stu-id="343e2-116">readOnly</span></span> | <span data-ttu-id="343e2-117">Логическое значение для настройки интерфейса задачи только для чтения (без добавления или удаления задач).</span><span class="sxs-lookup"><span data-stu-id="343e2-117">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="343e2-118">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="343e2-118">Default is `false`.</span></span> |
| <span data-ttu-id="343e2-119">hide-header</span><span class="sxs-lookup"><span data-stu-id="343e2-119">hide-header</span></span> | <span data-ttu-id="343e2-120">hideHeader</span><span class="sxs-lookup"><span data-stu-id="343e2-120">hideHeader</span></span> | <span data-ttu-id="343e2-121">Логическое значение для отображения или скрытия заголовка компонента.</span><span class="sxs-lookup"><span data-stu-id="343e2-121">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="343e2-122">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="343e2-122">Default is `false`.</span></span> |
| <span data-ttu-id="343e2-123">hide-options</span><span class="sxs-lookup"><span data-stu-id="343e2-123">hide-options</span></span> | <span data-ttu-id="343e2-124">hideOptions</span><span class="sxs-lookup"><span data-stu-id="343e2-124">hideOptions</span></span> | <span data-ttu-id="343e2-125">Логическое значение для отображения или скрытия параметров в задачах.</span><span class="sxs-lookup"><span data-stu-id="343e2-125">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="343e2-126">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="343e2-126">Default is `false`.</span></span>
| <span data-ttu-id="343e2-127">initial-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="343e2-127">initial-id="folder_id"</span></span> | <span data-ttu-id="343e2-128">initialId</span><span class="sxs-lookup"><span data-stu-id="343e2-128">initialId</span></span> | <span data-ttu-id="343e2-129">Строковый идентификатор, чтобы настроить для изначально отображаемой папки указанный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="343e2-129">A string ID to set the initially displayed folder to the provided ID.</span></span> |
| <span data-ttu-id="343e2-130">target-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="343e2-130">target-id="folder_id"</span></span>| <span data-ttu-id="343e2-131">targetId</span><span class="sxs-lookup"><span data-stu-id="343e2-131">targetId</span></span> | <span data-ttu-id="343e2-132">Строковый идентификатор для блокировки интерфейса задач по указанному идентификатору папки.</span><span class="sxs-lookup"><span data-stu-id="343e2-132">A string ID to lock the tasks interface to the provided folder ID.</span></span> |
| <span data-ttu-id="343e2-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="343e2-133">N/A</span></span> | <span data-ttu-id="343e2-134">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="343e2-134">isNewTaskVisible</span></span>  | <span data-ttu-id="343e2-135">Определяет, отображается ли новое представление задач при визуализации.</span><span class="sxs-lookup"><span data-stu-id="343e2-135">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="343e2-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="343e2-136">N/A</span></span> | <span data-ttu-id="343e2-137">taskFilter</span><span class="sxs-lookup"><span data-stu-id="343e2-137">taskFilter</span></span>  | <span data-ttu-id="343e2-138">Необязательная функция для фильтрации задач, демонстрируемых пользователю.</span><span class="sxs-lookup"><span data-stu-id="343e2-138">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="343e2-139">В следующем примере показаны только задачи из папки с идентификатором *12345*, и пользователю не разрешается создавать новые задачи.</span><span class="sxs-lookup"><span data-stu-id="343e2-139">The following example shows only tasks from the folder with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a><span data-ttu-id="343e2-140">Настраиваемые переменные CSS</span><span class="sxs-lookup"><span data-stu-id="343e2-140">Custom CSS variables</span></span>

<span data-ttu-id="343e2-141">Компонент `mgt-todo` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="343e2-141">The `mgt-todo` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="343e2-142">Дополнительные сведения см. в статье [Компоненты стиля](https://docs.microsoft.com/graph/toolkit/style.md).</span><span class="sxs-lookup"><span data-stu-id="343e2-142">To learn more, see [styling components](https://docs.microsoft.com/graph/toolkit/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="343e2-143">События</span><span class="sxs-lookup"><span data-stu-id="343e2-143">Events</span></span>

<span data-ttu-id="343e2-144">Из компонента инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="343e2-144">The following events are fired from the component.</span></span>

| <span data-ttu-id="343e2-145">Событие</span><span class="sxs-lookup"><span data-stu-id="343e2-145">Event</span></span> | <span data-ttu-id="343e2-146">Сведения</span><span class="sxs-lookup"><span data-stu-id="343e2-146">Detail</span></span> | <span data-ttu-id="343e2-147">Описание</span><span class="sxs-lookup"><span data-stu-id="343e2-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="343e2-148">taskAdded</span><span class="sxs-lookup"><span data-stu-id="343e2-148">taskAdded</span></span> | <span data-ttu-id="343e2-149">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="343e2-149">The detail contains the respective `task` object</span></span> | <span data-ttu-id="343e2-150">Возникает при создании задачи.</span><span class="sxs-lookup"><span data-stu-id="343e2-150">Fires when a new task has been created.</span></span> |
| <span data-ttu-id="343e2-151">taskChanged</span><span class="sxs-lookup"><span data-stu-id="343e2-151">taskChanged</span></span> | <span data-ttu-id="343e2-152">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="343e2-152">The detail contains the respective `task` object</span></span> | <span data-ttu-id="343e2-153">Возникает при изменении метаданных задачи, например при пометке задачи как завершенной.</span><span class="sxs-lookup"><span data-stu-id="343e2-153">Fires when task metadata has been changed, such as marking completed.</span></span> |
| <span data-ttu-id="343e2-154">taskClick</span><span class="sxs-lookup"><span data-stu-id="343e2-154">taskClick</span></span> | <span data-ttu-id="343e2-155">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="343e2-155">The detail contains the respective `task` object</span></span> | <span data-ttu-id="343e2-156">Возникает, когда пользователь щелкает или нажимает задачу.</span><span class="sxs-lookup"><span data-stu-id="343e2-156">Fires when the user clicks or taps on a task.</span></span> |
| <span data-ttu-id="343e2-157">taskRemoved</span><span class="sxs-lookup"><span data-stu-id="343e2-157">taskRemoved</span></span> | <span data-ttu-id="343e2-158">Сведения содержат соответствующий объект `task`</span><span class="sxs-lookup"><span data-stu-id="343e2-158">The detail contains the respective `task` object</span></span> | <span data-ttu-id="343e2-159">Возникает, если удалена существующая задача.</span><span class="sxs-lookup"><span data-stu-id="343e2-159">Fires when an existing task has been deleted.</span></span> |

## <a name="templates"></a><span data-ttu-id="343e2-160">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="343e2-160">Templates</span></span>

<span data-ttu-id="343e2-161">Компонент `tasks` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="343e2-161">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="343e2-162">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="343e2-162">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="343e2-163">Тип данных</span><span class="sxs-lookup"><span data-stu-id="343e2-163">Data type</span></span>     | <span data-ttu-id="343e2-164">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="343e2-164">Data context</span></span>              | <span data-ttu-id="343e2-165">Описание</span><span class="sxs-lookup"><span data-stu-id="343e2-165">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="343e2-166">task</span><span class="sxs-lookup"><span data-stu-id="343e2-166">task</span></span>     | <span data-ttu-id="343e2-167">задача: объект задачи To-Do</span><span class="sxs-lookup"><span data-stu-id="343e2-167">task: a to-do task object</span></span> | <span data-ttu-id="343e2-168">Заменяет всю стандартную задачу.</span><span class="sxs-lookup"><span data-stu-id="343e2-168">Replaces the whole default task.</span></span> |
| <span data-ttu-id="343e2-169">task-details</span><span class="sxs-lookup"><span data-stu-id="343e2-169">task-details</span></span> | <span data-ttu-id="343e2-170">задача: объект задачи To-Do</span><span class="sxs-lookup"><span data-stu-id="343e2-170">task: a to-do task object</span></span> | <span data-ttu-id="343e2-171">Шаблон заменит раздел сведений задачи.</span><span class="sxs-lookup"><span data-stu-id="343e2-171">Template replaces the details section of the task.</span></span> |

<span data-ttu-id="343e2-172">В следующем примере определяется шаблон для компонента задач.</span><span class="sxs-lookup"><span data-stu-id="343e2-172">The following example defines a template for the tasks component.</span></span>

```html
<mgt-todo>
    <template data-type="task-details">
        <div>
            Importance Level: {{task.importance}}
        </div>
    </template>
</mgt-todo>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="343e2-173">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="343e2-173">Microsoft Graph permissions</span></span>

<span data-ttu-id="343e2-174">Этот элемент управления использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="343e2-174">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="343e2-175">Ресурс</span><span class="sxs-lookup"><span data-stu-id="343e2-175">Resource</span></span> | <span data-ttu-id="343e2-176">Разрешение</span><span class="sxs-lookup"><span data-stu-id="343e2-176">Permission</span></span> |
| - | - |
| [<span data-ttu-id="343e2-177">/me/todo/lists/</span><span class="sxs-lookup"><span data-stu-id="343e2-177">/me/todo/lists/</span></span>](/graph/api/todo-list-lists) | <span data-ttu-id="343e2-178">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="343e2-178">Tasks.ReadWrite</span></span> |
| [<span data-ttu-id="343e2-179">/me/todo/lists/{todoTaskListId}/tasks</span><span class="sxs-lookup"><span data-stu-id="343e2-179">/me/todo/lists/{todoTaskListId}/tasks</span></span>](/graph/api/todotasklist-list-tasks) | <span data-ttu-id="343e2-180">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="343e2-180">Tasks.ReadWrite</span></span> |
| [<span data-ttu-id="343e2-181">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span><span class="sxs-lookup"><span data-stu-id="343e2-181">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span></span>](/graph/api/todotask-get) | <span data-ttu-id="343e2-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="343e2-182">Tasks.ReadWrite</span></span> |

## <a name="authentication"></a><span data-ttu-id="343e2-183">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="343e2-183">Authentication</span></span>

<span data-ttu-id="343e2-184">В компоненте задач используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="343e2-184">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>
