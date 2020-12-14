---
title: Компонент "Сделать" в microsoft Graph набор средств
description: Компонент "Дел" позволяет пользователю просматривать, добавлять, удалять, выполнять или редактировать задачи дел. Он работает с любыми задачами в Microsoft To-Do.
localization_priority: Normal
author: shweaver-MSFT
ms.openlocfilehash: 1a00d045da55dc14da47770b0e56522590f4b5bc
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659172"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="33974-104">Компонент "Сделать" в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="33974-104">To Do component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="33974-105">Компонент "Дел" используется для просмотра, добавления, удаления, завершения и редактирования задач из Microsoft To Do с помощью API дел в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="33974-105">The To Do component is used to enable the signed-in user to view, add, remove, complete, and/or edit tasks from Microsoft To Do using the To Do API in Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="33974-106">Пример</span><span class="sxs-lookup"><span data-stu-id="33974-106">Example</span></span>

<span data-ttu-id="33974-107">В следующем примере отображаются задачи Microsoft To Do пользователя, выписав его с помощью `mgt-todo` компонента.</span><span class="sxs-lookup"><span data-stu-id="33974-107">The following example displays the signed-in user's Microsoft To Do tasks using the `mgt-todo` component.</span></span> <span data-ttu-id="33974-108">С помощью редактора кода можно [увидеть,](#properties) как свойства изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="33974-108">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="33974-109">Откройте этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="33974-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="33974-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="33974-110">Properties</span></span>

<span data-ttu-id="33974-111">Для настройки компонента можно использовать следующие атрибуты и свойства.</span><span class="sxs-lookup"><span data-stu-id="33974-111">You can use the following attributes and properties to customize the component.</span></span>

| <span data-ttu-id="33974-112">Атрибут</span><span class="sxs-lookup"><span data-stu-id="33974-112">Attribute</span></span> | <span data-ttu-id="33974-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="33974-113">Property</span></span> | <span data-ttu-id="33974-114">Описание</span><span class="sxs-lookup"><span data-stu-id="33974-114">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="33974-115">только для чтения</span><span class="sxs-lookup"><span data-stu-id="33974-115">read-only</span></span> | <span data-ttu-id="33974-116">readOnly</span><span class="sxs-lookup"><span data-stu-id="33974-116">readOnly</span></span> | <span data-ttu-id="33974-117">Boolean, чтобы настроить интерфейс задачи только для чтения (без добавления или удаления задач).</span><span class="sxs-lookup"><span data-stu-id="33974-117">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="33974-118">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="33974-118">Default is `false`.</span></span> |
| <span data-ttu-id="33974-119">hide-header</span><span class="sxs-lookup"><span data-stu-id="33974-119">hide-header</span></span> | <span data-ttu-id="33974-120">hideHeader</span><span class="sxs-lookup"><span data-stu-id="33974-120">hideHeader</span></span> | <span data-ttu-id="33974-121">Boolean для показа или скрытие загона компонента.</span><span class="sxs-lookup"><span data-stu-id="33974-121">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="33974-122">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="33974-122">Default is `false`.</span></span> |
| <span data-ttu-id="33974-123">hide-options</span><span class="sxs-lookup"><span data-stu-id="33974-123">hide-options</span></span> | <span data-ttu-id="33974-124">hideOptions</span><span class="sxs-lookup"><span data-stu-id="33974-124">hideOptions</span></span> | <span data-ttu-id="33974-125">Boolean для показа или скрытие параметров в задачах.</span><span class="sxs-lookup"><span data-stu-id="33974-125">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="33974-126">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="33974-126">Default is `false`.</span></span>
| <span data-ttu-id="33974-127">initial-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="33974-127">initial-id="folder_id"</span></span> | <span data-ttu-id="33974-128">initialId</span><span class="sxs-lookup"><span data-stu-id="33974-128">initialId</span></span> | <span data-ttu-id="33974-129">ИД строки, чтобы установить для первоначально отображаемой папки предоставленный ИД.</span><span class="sxs-lookup"><span data-stu-id="33974-129">A string ID to set the initially displayed folder to the provided ID.</span></span> |
| <span data-ttu-id="33974-130">target-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="33974-130">target-id="folder_id"</span></span>| <span data-ttu-id="33974-131">targetId</span><span class="sxs-lookup"><span data-stu-id="33974-131">targetId</span></span> | <span data-ttu-id="33974-132">Строка СД для блокировки интерфейса задач с предоставленным ИД папки.</span><span class="sxs-lookup"><span data-stu-id="33974-132">A string ID to lock the tasks interface to the provided folder ID.</span></span> |
| <span data-ttu-id="33974-133">Недоступно</span><span class="sxs-lookup"><span data-stu-id="33974-133">N/A</span></span> | <span data-ttu-id="33974-134">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="33974-134">isNewTaskVisible</span></span>  | <span data-ttu-id="33974-135">Определяет, отображается ли новое представление задачи при отрисовки.</span><span class="sxs-lookup"><span data-stu-id="33974-135">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="33974-136">Недоступно</span><span class="sxs-lookup"><span data-stu-id="33974-136">N/A</span></span> | <span data-ttu-id="33974-137">taskFilter</span><span class="sxs-lookup"><span data-stu-id="33974-137">taskFilter</span></span>  | <span data-ttu-id="33974-138">Необязательная функция для фильтрации задач, которые показываются пользователю.</span><span class="sxs-lookup"><span data-stu-id="33974-138">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="33974-139">В следующем примере показаны только задачи из папки с ИД *12345* и не позволяют пользователю создавать новые задачи.</span><span class="sxs-lookup"><span data-stu-id="33974-139">The following example shows only tasks from the folder with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a><span data-ttu-id="33974-140">Настраиваемые переменные CSS</span><span class="sxs-lookup"><span data-stu-id="33974-140">Custom CSS variables</span></span>

<span data-ttu-id="33974-141">Компонент `mgt-todo` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="33974-141">The `mgt-todo` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="33974-142">Дополнительные узнать см. [в компонентах стиля.](https://docs.microsoft.com/graph/toolkit/style.md)</span><span class="sxs-lookup"><span data-stu-id="33974-142">To learn more, see [styling components](https://docs.microsoft.com/graph/toolkit/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="33974-143">События</span><span class="sxs-lookup"><span data-stu-id="33974-143">Events</span></span>

<span data-ttu-id="33974-144">Из компонента и происходят следующие события.</span><span class="sxs-lookup"><span data-stu-id="33974-144">The following events are fired from the component.</span></span>

| <span data-ttu-id="33974-145">Событие</span><span class="sxs-lookup"><span data-stu-id="33974-145">Event</span></span> | <span data-ttu-id="33974-146">Сведения</span><span class="sxs-lookup"><span data-stu-id="33974-146">Detail</span></span> | <span data-ttu-id="33974-147">Описание</span><span class="sxs-lookup"><span data-stu-id="33974-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="33974-148">taskAdded</span><span class="sxs-lookup"><span data-stu-id="33974-148">taskAdded</span></span> | <span data-ttu-id="33974-149">Сведения содержат соответствующий `task` объект</span><span class="sxs-lookup"><span data-stu-id="33974-149">The detail contains the respective `task` object</span></span> | <span data-ttu-id="33974-150">Создается, когда создается новая задача.</span><span class="sxs-lookup"><span data-stu-id="33974-150">Fires when a new task has been created.</span></span> |
| <span data-ttu-id="33974-151">taskChanged</span><span class="sxs-lookup"><span data-stu-id="33974-151">taskChanged</span></span> | <span data-ttu-id="33974-152">Сведения содержат соответствующий `task` объект</span><span class="sxs-lookup"><span data-stu-id="33974-152">The detail contains the respective `task` object</span></span> | <span data-ttu-id="33974-153">Происходит, когда метаданные задачи были изменены, например после пометки.</span><span class="sxs-lookup"><span data-stu-id="33974-153">Fires when task metadata has been changed, such as marking completed.</span></span> |
| <span data-ttu-id="33974-154">taskClick</span><span class="sxs-lookup"><span data-stu-id="33974-154">taskClick</span></span> | <span data-ttu-id="33974-155">Сведения содержат соответствующий `task` объект</span><span class="sxs-lookup"><span data-stu-id="33974-155">The detail contains the respective `task` object</span></span> | <span data-ttu-id="33974-156">Происходит, когда пользователь щелкает задачу или нажимает на нее.</span><span class="sxs-lookup"><span data-stu-id="33974-156">Fires when the user clicks or taps on a task.</span></span> |
| <span data-ttu-id="33974-157">taskRemoved</span><span class="sxs-lookup"><span data-stu-id="33974-157">taskRemoved</span></span> | <span data-ttu-id="33974-158">Сведения содержат соответствующий `task` объект</span><span class="sxs-lookup"><span data-stu-id="33974-158">The detail contains the respective `task` object</span></span> | <span data-ttu-id="33974-159">Происходит при удалении существующей задачи.</span><span class="sxs-lookup"><span data-stu-id="33974-159">Fires when an existing task has been deleted.</span></span> |

## <a name="templates"></a><span data-ttu-id="33974-160">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="33974-160">Templates</span></span>

<span data-ttu-id="33974-161">Компонент `tasks` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые позволяют заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="33974-161">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="33974-162">Чтобы указать шаблон, включив элемент в `<template>` компонент, закажите одно из `data-type` следующих значений.</span><span class="sxs-lookup"><span data-stu-id="33974-162">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="33974-163">Тип данных</span><span class="sxs-lookup"><span data-stu-id="33974-163">Data type</span></span>     | <span data-ttu-id="33974-164">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="33974-164">Data context</span></span>              | <span data-ttu-id="33974-165">Описание</span><span class="sxs-lookup"><span data-stu-id="33974-165">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="33974-166">task</span><span class="sxs-lookup"><span data-stu-id="33974-166">task</span></span>     | <span data-ttu-id="33974-167">task: объект задачи для задач</span><span class="sxs-lookup"><span data-stu-id="33974-167">task: a to-do task object</span></span> | <span data-ttu-id="33974-168">Заменяет всю задачу по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33974-168">Replaces the whole default task.</span></span> |
| <span data-ttu-id="33974-169">task-details</span><span class="sxs-lookup"><span data-stu-id="33974-169">task-details</span></span> | <span data-ttu-id="33974-170">task: объект задачи для задач</span><span class="sxs-lookup"><span data-stu-id="33974-170">task: a to-do task object</span></span> | <span data-ttu-id="33974-171">Шаблон заменяет раздел сведений о задаче.</span><span class="sxs-lookup"><span data-stu-id="33974-171">Template replaces the details section of the task.</span></span> |

<span data-ttu-id="33974-172">В следующем примере определяется шаблон для компонента задач.</span><span class="sxs-lookup"><span data-stu-id="33974-172">The following example defines a template for the tasks component.</span></span>

```html
<mgt-todo>
    <template data-type="task-details">
        <div>
            Importance Level: {{task.importance}}
        </div>
    </template>
</mgt-todo>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="33974-173">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="33974-173">Microsoft Graph permissions</span></span>

<span data-ttu-id="33974-174">Этот контроль использует следующие API Microsoft Graph и разрешения.</span><span class="sxs-lookup"><span data-stu-id="33974-174">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="33974-175">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33974-175">Resource</span></span> | <span data-ttu-id="33974-176">Разрешение</span><span class="sxs-lookup"><span data-stu-id="33974-176">Permission</span></span> |
| - | - |
| [<span data-ttu-id="33974-177">/me/todo/lists/</span><span class="sxs-lookup"><span data-stu-id="33974-177">/me/todo/lists/</span></span>](/graph/api/todo-list-lists) | <span data-ttu-id="33974-178">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33974-178">Tasks.ReadWrite</span></span> |
| [<span data-ttu-id="33974-179">/me/todo/lists/{todoTaskListId}/tasks</span><span class="sxs-lookup"><span data-stu-id="33974-179">/me/todo/lists/{todoTaskListId}/tasks</span></span>](/graph/api/todotasklist-list-tasks) | <span data-ttu-id="33974-180">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33974-180">Tasks.ReadWrite</span></span> |
| [<span data-ttu-id="33974-181">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span><span class="sxs-lookup"><span data-stu-id="33974-181">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span></span>](/graph/api/todotask-get) | <span data-ttu-id="33974-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33974-182">Tasks.ReadWrite</span></span> |

## <a name="authentication"></a><span data-ttu-id="33974-183">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="33974-183">Authentication</span></span>

<span data-ttu-id="33974-184">Компонент задач использует глобального поставщика проверки подлинности, описанного в [документации по проверке подлинности.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="33974-184">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>
