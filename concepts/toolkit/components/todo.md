---
title: Компонент To Do в Microsoft Graph Toolkit
description: Компонент To Do позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи To Do. Он поддерживает любые задачи в Microsoft To-Do.
localization_priority: Normal
author: shweaver-MSFT
ms.openlocfilehash: 1d2f1fd83626c1fcaaf2356605347581f247f6da
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266789"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a>Компонент To Do в Microsoft Graph Toolkit

Компонент To Do используется, чтобы позволить вошедшему пользователю просматривать, добавлять, удалять, выполнять и/или изменять задачи из Microsoft To Do с помощью API To Do в Microsoft Graph.

## <a name="example"></a>Пример

В следующем примере отображаются задачи Microsoft To Do вошедшего пользователя с помощью компонента `mgt-todo`. Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[Открыть этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a>Свойства

Для настройки компонента можно использовать следующие атрибуты и свойства.

| Атрибут | Свойство | Описание |
| -- | -- | -- |
| read-only | readOnly | Логическое значение для настройки интерфейса задачи только для чтения (без добавления или удаления задач). Значение по умолчанию: `false`. |
| hide-header | hideHeader | Логическое значение для отображения или скрытия заголовка компонента. Значение по умолчанию: `false`. |
| hide-options | hideOptions | Логическое значение для отображения или скрытия параметров в задачах. Значение по умолчанию: `false`.
| initial-id="folder_id" | initialId | Строковый идентификатор, чтобы настроить для изначально отображаемой папки указанный идентификатор. |
| target-id="folder_id"| targetId | Строковый идентификатор для блокировки интерфейса задач по указанному идентификатору папки. |
| Н/Д | isNewTaskVisible  | Определяет, отображается ли новое представление задач при визуализации. |
| Н/Д | taskFilter  | Необязательная функция для фильтрации задач, демонстрируемых пользователю. |

В следующем примере показаны только задачи из папки с идентификатором *12345*, и пользователю не разрешается создавать новые задачи.

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

Дополнительные сведения см. в статье [Компоненты стиля](https://docs.microsoft.com/graph/toolkit/style.md).

## <a name="events"></a>События

Из компонента инициируются следующие события.

| Событие | Сведения | Описание |
| --- | --- | --- |
| taskAdded | Сведения содержат соответствующий объект `task` | Возникает при создании задачи. |
| taskChanged | Сведения содержат соответствующий объект `task` | Возникает при изменении метаданных задачи, например при пометке задачи как завершенной. |
| taskClick | Сведения содержат соответствующий объект `task` | Возникает, когда пользователь щелкает или нажимает задачу. |
| taskRemoved | Сведения содержат соответствующий объект `task` | Возникает, если удалена существующая задача. |

## <a name="templates"></a>Шаблоны

Компонент `tasks` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента. Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.

| Тип данных     | Контекст данных              | Описание                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| task     | задача: объект задачи To-Do | Заменяет всю стандартную задачу. |
| task-details | задача: объект задачи To-Do | Шаблон заменит раздел сведений задачи. |

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

Этот элемент управления использует следующие API и разрешения Microsoft Graph.

| Ресурс | Разрешение |
| - | - |
| [/me/todo/lists/](/graph/api/todo-list-lists) | Tasks.ReadWrite |
| [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks) | Tasks.ReadWrite |
| [/me/todo/lists/{todoTaskListId}/tasks/{taskId}](/graph/api/todotask-get) | Tasks.ReadWrite |

## <a name="authentication"></a>Проверка подлинности

В компоненте задач используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).

## <a name="cache"></a>Кэш

Компонент `mgt-todo` не кэшет данных.
