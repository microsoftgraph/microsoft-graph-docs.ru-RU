---
title: Компонент To Do в Microsoft Graph Toolkit
description: Компонент To Do позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи To Do. Он поддерживает любые задачи в Microsoft To-Do.
localization_priority: Normal
author: shweaver-MSFT
ms.openlocfilehash: 94bdbf1777a4ebe6c60d91c227c805c2edf53809
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334726"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="28e05-104">Компонент To Do в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="28e05-104">To Do component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="28e05-105">Компонент To Do используется, чтобы позволить вошедшему пользователю просматривать, добавлять, удалять, выполнять и/или изменять задачи из Microsoft To Do с помощью API To Do в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="28e05-105">The To Do component is used to enable the signed-in user to view, add, remove, complete, and/or edit tasks from Microsoft To Do using the To Do API in Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="28e05-106">Пример</span><span class="sxs-lookup"><span data-stu-id="28e05-106">Example</span></span>

<span data-ttu-id="28e05-107">В следующем примере отображаются задачи Microsoft To Do вошедшего пользователя с помощью компонента `mgt-todo`.</span><span class="sxs-lookup"><span data-stu-id="28e05-107">The following example displays the signed-in user's Microsoft To Do tasks using the `mgt-todo` component.</span></span> <span data-ttu-id="28e05-108">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="28e05-108">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="28e05-109">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="28e05-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="28e05-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="28e05-110">Properties</span></span>

<span data-ttu-id="28e05-111">Для настройки компонента можно использовать следующие атрибуты и свойства.</span><span class="sxs-lookup"><span data-stu-id="28e05-111">You can use the following attributes and properties to customize the component.</span></span>

| <span data-ttu-id="28e05-112">Атрибут</span><span class="sxs-lookup"><span data-stu-id="28e05-112">Attribute</span></span> | <span data-ttu-id="28e05-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="28e05-113">Property</span></span> | <span data-ttu-id="28e05-114">Описание</span><span class="sxs-lookup"><span data-stu-id="28e05-114">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="28e05-115">read-only</span><span class="sxs-lookup"><span data-stu-id="28e05-115">read-only</span></span> | <span data-ttu-id="28e05-116">readOnly</span><span class="sxs-lookup"><span data-stu-id="28e05-116">readOnly</span></span> | <span data-ttu-id="28e05-117">Логическое значение для настройки интерфейса задачи только для чтения (без добавления или удаления задач).</span><span class="sxs-lookup"><span data-stu-id="28e05-117">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="28e05-118">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="28e05-118">Default is `false`.</span></span> |
| <span data-ttu-id="28e05-119">hide-header</span><span class="sxs-lookup"><span data-stu-id="28e05-119">hide-header</span></span> | <span data-ttu-id="28e05-120">hideHeader</span><span class="sxs-lookup"><span data-stu-id="28e05-120">hideHeader</span></span> | <span data-ttu-id="28e05-121">Логическое значение для отображения или скрытия заголовка компонента.</span><span class="sxs-lookup"><span data-stu-id="28e05-121">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="28e05-122">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="28e05-122">Default is `false`.</span></span> |
| <span data-ttu-id="28e05-123">hide-options</span><span class="sxs-lookup"><span data-stu-id="28e05-123">hide-options</span></span> | <span data-ttu-id="28e05-124">hideOptions</span><span class="sxs-lookup"><span data-stu-id="28e05-124">hideOptions</span></span> | <span data-ttu-id="28e05-125">Логическое значение для отображения или скрытия параметров в задачах.</span><span class="sxs-lookup"><span data-stu-id="28e05-125">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="28e05-126">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="28e05-126">Default is `false`.</span></span>
| <span data-ttu-id="28e05-127">initial-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="28e05-127">initial-id="folder_id"</span></span> | <span data-ttu-id="28e05-128">initialId</span><span class="sxs-lookup"><span data-stu-id="28e05-128">initialId</span></span> | <span data-ttu-id="28e05-129">Строковый идентификатор, чтобы настроить для изначально отображаемой папки указанный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="28e05-129">A string ID to set the initially displayed folder to the provided ID.</span></span> |
| <span data-ttu-id="28e05-130">target-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="28e05-130">target-id="folder_id"</span></span>| <span data-ttu-id="28e05-131">targetId</span><span class="sxs-lookup"><span data-stu-id="28e05-131">targetId</span></span> | <span data-ttu-id="28e05-132">Строковый идентификатор для блокировки интерфейса задач по указанному идентификатору папки.</span><span class="sxs-lookup"><span data-stu-id="28e05-132">A string ID to lock the tasks interface to the provided folder ID.</span></span> |
| <span data-ttu-id="28e05-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="28e05-133">N/A</span></span> | <span data-ttu-id="28e05-134">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="28e05-134">isNewTaskVisible</span></span>  | <span data-ttu-id="28e05-135">Определяет, отображается ли новое представление задач при визуализации.</span><span class="sxs-lookup"><span data-stu-id="28e05-135">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="28e05-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="28e05-136">N/A</span></span> | <span data-ttu-id="28e05-137">taskFilter</span><span class="sxs-lookup"><span data-stu-id="28e05-137">taskFilter</span></span>  | <span data-ttu-id="28e05-138">Необязательная функция для фильтрации задач, демонстрируемых пользователю.</span><span class="sxs-lookup"><span data-stu-id="28e05-138">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="28e05-139">В следующем примере показаны только задачи из папки с идентификатором *12345*, и пользователю не разрешается создавать новые задачи.</span><span class="sxs-lookup"><span data-stu-id="28e05-139">The following example shows only tasks from the folder with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a><span data-ttu-id="28e05-140">Настраиваемые переменные CSS</span><span class="sxs-lookup"><span data-stu-id="28e05-140">Custom CSS variables</span></span>

<span data-ttu-id="28e05-141">Компонент `mgt-todo` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="28e05-141">The `mgt-todo` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="28e05-142">Дополнительные сведения см. в статье [Компоненты стиля](https://docs.microsoft.com/graph/toolkit/style.md).</span><span class="sxs-lookup"><span data-stu-id="28e05-142">To learn more, see [styling components](https://docs.microsoft.com/graph/toolkit/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="28e05-143">События</span><span class="sxs-lookup"><span data-stu-id="28e05-143">Events</span></span>

<span data-ttu-id="28e05-144">Из компонента инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="28e05-144">The following events are fired from the component.</span></span>

<span data-ttu-id="28e05-145">Событие</span><span class="sxs-lookup"><span data-stu-id="28e05-145">Event</span></span> | <span data-ttu-id="28e05-146">Когда он излучается</span><span class="sxs-lookup"><span data-stu-id="28e05-146">When is it emitted</span></span> | <span data-ttu-id="28e05-147">Настраиваемые данные</span><span class="sxs-lookup"><span data-stu-id="28e05-147">Custom data</span></span> | <span data-ttu-id="28e05-148">Отмена</span><span class="sxs-lookup"><span data-stu-id="28e05-148">Cancelable</span></span> | <span data-ttu-id="28e05-149">Пузыри</span><span class="sxs-lookup"><span data-stu-id="28e05-149">Bubbles</span></span> | <span data-ttu-id="28e05-150">Работает с настраиваемой шаблонной</span><span class="sxs-lookup"><span data-stu-id="28e05-150">Works with custom template</span></span>
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`taskClick` | <span data-ttu-id="28e05-151">Пожары, когда пользователь щелкает или нажимает на задачу</span><span class="sxs-lookup"><span data-stu-id="28e05-151">Fires when the user clicks or taps on a task</span></span> | <span data-ttu-id="28e05-152">Выбранная [задача](https://github.com/microsoftgraph/microsoft-graph-toolkit/blob/66a5bbb6591e6260e95dbc00c0d06bcbe8dcef38/packages/mgt-components/src/components/mgt-todo/graph.todo.ts#L41)</span><span class="sxs-lookup"><span data-stu-id="28e05-152">Selected [task](https://github.com/microsoftgraph/microsoft-graph-toolkit/blob/66a5bbb6591e6260e95dbc00c0d06bcbe8dcef38/packages/mgt-components/src/components/mgt-todo/graph.todo.ts#L41)</span></span> | <span data-ttu-id="28e05-153">Нет</span><span class="sxs-lookup"><span data-stu-id="28e05-153">No</span></span> | <span data-ttu-id="28e05-154">Нет</span><span class="sxs-lookup"><span data-stu-id="28e05-154">No</span></span> | <span data-ttu-id="28e05-155">Нет</span><span class="sxs-lookup"><span data-stu-id="28e05-155">No</span></span>

<span data-ttu-id="28e05-156">Дополнительные сведения об обработке событий см. в [этой работе.](../customize-components/events.md)</span><span class="sxs-lookup"><span data-stu-id="28e05-156">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="28e05-157">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="28e05-157">Templates</span></span>

<span data-ttu-id="28e05-158">Компонент `tasks` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="28e05-158">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="28e05-159">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="28e05-159">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="28e05-160">Тип данных</span><span class="sxs-lookup"><span data-stu-id="28e05-160">Data type</span></span>     | <span data-ttu-id="28e05-161">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="28e05-161">Data context</span></span>              | <span data-ttu-id="28e05-162">Описание</span><span class="sxs-lookup"><span data-stu-id="28e05-162">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="28e05-163">task</span><span class="sxs-lookup"><span data-stu-id="28e05-163">task</span></span>     | <span data-ttu-id="28e05-164">задача: объект задачи To-Do</span><span class="sxs-lookup"><span data-stu-id="28e05-164">task: a to-do task object</span></span> | <span data-ttu-id="28e05-165">Заменяет всю стандартную задачу.</span><span class="sxs-lookup"><span data-stu-id="28e05-165">Replaces the whole default task.</span></span> |
| <span data-ttu-id="28e05-166">task-details</span><span class="sxs-lookup"><span data-stu-id="28e05-166">task-details</span></span> | <span data-ttu-id="28e05-167">задача: объект задачи To-Do</span><span class="sxs-lookup"><span data-stu-id="28e05-167">task: a to-do task object</span></span> | <span data-ttu-id="28e05-168">Шаблон заменит раздел сведений задачи.</span><span class="sxs-lookup"><span data-stu-id="28e05-168">Template replaces the details section of the task.</span></span> |

<span data-ttu-id="28e05-169">В следующем примере определяется шаблон для компонента задач.</span><span class="sxs-lookup"><span data-stu-id="28e05-169">The following example defines a template for the tasks component.</span></span>

```html
<mgt-todo>
    <template data-type="task-details">
        <div>
            Importance Level: {{task.importance}}
        </div>
    </template>
</mgt-todo>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="28e05-170">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="28e05-170">Microsoft Graph permissions</span></span>

<span data-ttu-id="28e05-171">Этот элемент управления использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="28e05-171">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="28e05-172">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="28e05-172">Configuration</span></span> | <span data-ttu-id="28e05-173">Разрешение</span><span class="sxs-lookup"><span data-stu-id="28e05-173">Permission</span></span> | <span data-ttu-id="28e05-174">API</span><span class="sxs-lookup"><span data-stu-id="28e05-174">API</span></span> |
| ------------- | ---------- | --- |
| <span data-ttu-id="28e05-175">`targetId` set</span><span class="sxs-lookup"><span data-stu-id="28e05-175">`targetId` set</span></span> | <span data-ttu-id="28e05-176">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="28e05-176">Tasks.Read</span></span> | <span data-ttu-id="28e05-177">[/me/todo/lists/${listId}](/graph/api/todotasklist-get?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span><span class="sxs-lookup"><span data-stu-id="28e05-177">[/me/todo/lists/${listId}](/graph/api/todotasklist-get?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span></span> |
| <span data-ttu-id="28e05-178">`targetId` не установлено</span><span class="sxs-lookup"><span data-stu-id="28e05-178">`targetId` not set</span></span> | <span data-ttu-id="28e05-179">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="28e05-179">Tasks.Read</span></span> | <span data-ttu-id="28e05-180">[/me/todo/lists](/graph/api/todo-list-lists?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span><span class="sxs-lookup"><span data-stu-id="28e05-180">[/me/todo/lists](/graph/api/todo-list-lists?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span></span> |
| <span data-ttu-id="28e05-181">создание, обновление или удаление задачи</span><span class="sxs-lookup"><span data-stu-id="28e05-181">create, update or delete task</span></span> | <span data-ttu-id="28e05-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28e05-182">Tasks.ReadWrite</span></span> | [<span data-ttu-id="28e05-183">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span><span class="sxs-lookup"><span data-stu-id="28e05-183">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span></span>](/graph/api/todotask-get) |

## <a name="authentication"></a><span data-ttu-id="28e05-184">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="28e05-184">Authentication</span></span>

<span data-ttu-id="28e05-185">В компоненте задач используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="28e05-185">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="28e05-186">Кэш</span><span class="sxs-lookup"><span data-stu-id="28e05-186">Cache</span></span>

<span data-ttu-id="28e05-187">Компонент `mgt-todo` не кэшет данных.</span><span class="sxs-lookup"><span data-stu-id="28e05-187">The `mgt-todo` component doesn't cache any data.</span></span>
