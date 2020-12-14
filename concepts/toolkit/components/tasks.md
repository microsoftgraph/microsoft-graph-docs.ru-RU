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
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Компонент задач в microsoft Graph набор средств

Компонент "Задачи" позволяет пользователю просматривать, добавлять, удалять, выполнять или редактировать задачи из Планировщика (Майкрософт).  

Кроме того, пользователь может назначить задачу одному или нескольким пользователям Microsoft Graph. Дополнительные сведения о назначениях Microsoft Graph см. в [записях plannerAssignments.](/graph/api/resources/plannerassignments)

## <a name="example"></a>Пример

В следующем примере отображаются задачи, которые пользователь, вописав в планировщик Microsoft, использует `mgt-tasks` компонент. С помощью редактора кода можно [увидеть,](#properties) как свойства изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[Откройте этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a>Свойства

| Атрибут | Свойство | Описание |
| -- | -- | -- |
| только для чтения | readOnly | Boolean, чтобы настроить интерфейс задачи только для чтения (без добавления или удаления задач). Значение по умолчанию: `false`. |
| hide-header | hideHeader | Boolean для показа или скрытие загона компонента. Значение по умолчанию: `false`. |
| hide-options | hideOptions | Boolean для показа или скрытие параметров в задачах. Значение по умолчанию: `false`.
| initial-id="planner_id/folder_id" | initialId | Строковый ИД для первоначально отображаемого планировщика или папки в качестве предоставленного. |
| initial-bucket-id="bucket_id" | initialBucketId | Строковый ИД, чтобы установить для изначально отображаемого сегмента (Data-Source Только Планировщик) предоставленный ИД. |
| target-id="planner_id/folder_id"| targetId | Строковый ИД для блокировки интерфейса задач предоставленным планировщиком или идом папки. |
| target-bucket-id="bucket_id" |targetBucketId  | Строковый ИД для блокировки интерфейса задач с предоставленным идом сегмента (только Data-Source Планировщика). |
| group-id | groupId  | ИД строки для блокировки интерфейса задач с помощью ИД группы. |
| Недоступно | isNewTaskVisible  | Определяет, отображается ли новое представление задачи при отрисовки. |
| Недоступно | taskFilter  | Необязательная функция для фильтрации задач, которые показываются пользователю. |

В следующем примере показаны только задачи из Планировщика с ИД *12345* и не позволяют пользователю создавать новые задачи.

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

В следующем примере показано, как фильтровать задачи, для которые заданной только *категория 3.*

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a>Настраиваемые переменные CSS

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

## <a name="events"></a>События
| Событие | Сведения | Описание |
| --- | --- | --- |
| taskAdded | Сведения содержат соответствующий `task` объект | Создается, когда создается новая задача. |
| taskChanged | Сведения содержат соответствующий `task` объект | Происходит, когда метаданные задачи были изменены, например после пометки. |
| taskClick | Сведения содержат соответствующий `task` объект | Происходит, когда пользователь щелкает задачу или нажимает на нее. |
| taskRemoved | Сведения содержат соответствующий `task` объект | Происходит при удалении существующей задачи. |

## <a name="templates"></a>Шаблоны

Компонент `tasks` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые позволяют заменить определенные части компонента. Чтобы указать шаблон, включив элемент в компонент и заключив в него одно `<template>` `data-type` из следующих значений:

| Тип данных     | Контекст данных              | Описание                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| task     | task: объект задачи планировщика | заменяет всю задачу по умолчанию. |
| task-details | task: объект задачи планировщика | шаблон заменяет раздел сведений о задаче. |

В следующем примере определяется шаблон для компонента задач.

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

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот контроль использует следующие API Microsoft Graph и разрешения.

| Ресурс | Разрешение |
| - | - |
| /me/planner/plans | Group.Read.All |
| /planner/plans/${id} | Group.Read.All, Group.ReadWrite.All |
| /planner/tasks | Group.ReadWrite.All |
| /groups/${group-id}/planner/plans | Group.Read.All, Group.ReadWrite.All |

Для источника данных Планировщика (Майкрософт) для получения и чтения задач требуется разрешение Groups.Read.All. Для добавления, обновления или удаления задач требуется разрешение Groups.ReadWrite.All.

## <a name="authentication"></a>Проверка подлинности

Компонент задач использует глобального поставщика проверки подлинности, описанного в [документации по проверке подлинности.](../providers/providers.md)