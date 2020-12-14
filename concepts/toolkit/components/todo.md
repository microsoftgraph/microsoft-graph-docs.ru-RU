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
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a>Компонент "Сделать" в microsoft Graph набор средств

Компонент "Дел" используется для просмотра, добавления, удаления, завершения и редактирования задач из Microsoft To Do с помощью API дел в Microsoft Graph.

## <a name="example"></a>Пример

В следующем примере отображаются задачи Microsoft To Do пользователя, выписав его с помощью `mgt-todo` компонента. С помощью редактора кода можно [увидеть,](#properties) как свойства изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[Откройте этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a>Свойства

Для настройки компонента можно использовать следующие атрибуты и свойства.

| Атрибут | Свойство | Описание |
| -- | -- | -- |
| только для чтения | readOnly | Boolean, чтобы настроить интерфейс задачи только для чтения (без добавления или удаления задач). Значение по умолчанию: `false`. |
| hide-header | hideHeader | Boolean для показа или скрытие загона компонента. Значение по умолчанию: `false`. |
| hide-options | hideOptions | Boolean для показа или скрытие параметров в задачах. Значение по умолчанию: `false`.
| initial-id="folder_id" | initialId | ИД строки, чтобы установить для первоначально отображаемой папки предоставленный ИД. |
| target-id="folder_id"| targetId | Строка СД для блокировки интерфейса задач с предоставленным ИД папки. |
| Недоступно | isNewTaskVisible  | Определяет, отображается ли новое представление задачи при отрисовки. |
| Недоступно | taskFilter  | Необязательная функция для фильтрации задач, которые показываются пользователю. |

В следующем примере показаны только задачи из папки с ИД *12345* и не позволяют пользователю создавать новые задачи.

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a>Настраиваемые переменные CSS

Компонент `mgt-todo` определяет следующие настраиваемые свойства CSS.

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

Дополнительные узнать см. [в компонентах стиля.](https://docs.microsoft.com/graph/toolkit/style.md)

## <a name="events"></a>События

Из компонента и происходят следующие события.

| Событие | Сведения | Описание |
| --- | --- | --- |
| taskAdded | Сведения содержат соответствующий `task` объект | Создается, когда создается новая задача. |
| taskChanged | Сведения содержат соответствующий `task` объект | Происходит, когда метаданные задачи были изменены, например после пометки. |
| taskClick | Сведения содержат соответствующий `task` объект | Происходит, когда пользователь щелкает задачу или нажимает на нее. |
| taskRemoved | Сведения содержат соответствующий `task` объект | Происходит при удалении существующей задачи. |

## <a name="templates"></a>Шаблоны

Компонент `tasks` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые позволяют заменить определенные части компонента. Чтобы указать шаблон, включив элемент в `<template>` компонент, закажите одно из `data-type` следующих значений.

| Тип данных     | Контекст данных              | Описание                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| task     | task: объект задачи для задач | Заменяет всю задачу по умолчанию. |
| task-details | task: объект задачи для задач | Шаблон заменяет раздел сведений о задаче. |

В следующем примере определяется шаблон для компонента задач.

```html
<mgt-todo>
    <template data-type="task-details">
        <div>
            Importance Level: {{task.importance}}
        </div>
    </template>
</mgt-todo>
```

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот контроль использует следующие API Microsoft Graph и разрешения.

| Ресурс | Разрешение |
| - | - |
| [/me/todo/lists/](/graph/api/todo-list-lists) | Tasks.ReadWrite |
| [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks) | Tasks.ReadWrite |
| [/me/todo/lists/{todoTaskListId}/tasks/{taskId}](/graph/api/todotask-get) | Tasks.ReadWrite |

## <a name="authentication"></a>Проверка подлинности

Компонент задач использует глобального поставщика проверки подлинности, описанного в [документации по проверке подлинности.](../providers/providers.md)
