---
title: Компонент задач в microsoft Graph набор средств
description: Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи. Он работает с любыми задачами в Microsoft Planner.
localization_priority: Normal
author: benotter
ms.openlocfilehash: 65fc01d5b2cc5db6f6236bb64b7372522c4d61be
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780990"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Компонент задач в microsoft Graph набор средств

Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи из Microsoft Planner.  

Кроме того, пользователь может назначить одному или нескольким Graph Майкрософт задачу. Дополнительные сведения о назначениях microsoft Graph см. [в материале plannerAssignments.](/graph/api/resources/plannerassignments)

## <a name="example"></a>Пример

В следующем примере отображаются задачи microsoft Planner пользователя, подписанные с помощью `mgt-tasks` компонента. Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[Открыть этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a>Свойства

| Атрибут | Свойство | Описание |
| -- | -- | -- |
| read-only | readOnly | Логическое значение для настройки интерфейса задачи только для чтения (без добавления или удаления задач). Значение по умолчанию: `false`. |
| hide-header | hideHeader | Логическое значение для отображения или скрытия заголовка компонента. Значение по умолчанию: `false`. |
| hide-options | hideOptions | Логическое значение для отображения или скрытия параметров в задачах. Значение по умолчанию: `false`.
| initial-id="planner_id/folder_id" | initialId | A string ID to set the initially displayed planner or folder to the provided ID. |
| initial-bucket-id="bucket_id" | initialBucketId | A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID. |
| target-id="planner_id/folder_id"| targetId | Строковый ID для блокировки интерфейса задач к предоставленной планировщику или папке. |
| target-bucket-id="bucket_id" |targetBucketId  | A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only). |
| group-id | groupId  | A string ID to lock the tasks interface to the group ID. |
| Н/Д | isNewTaskVisible  | Определяет, отображается ли новое представление задач при визуализации. |
| Н/Д | taskFilter  | Необязательная функция для фильтрации задач, демонстрируемых пользователю. |

В следующем примере показаны только задачи от Planner с ID *12345* и не позволяют пользователю создавать новые задачи.

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

В следующем примере показано, как фильтровать задачи, которые имеют только *набор category3.*

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
| taskAdded | Сведения содержат соответствующий объект `task` | Возникает при создании задачи. |
| taskChanged | Сведения содержат соответствующий объект `task` | Возникает при изменении метаданных задачи, например при пометке задачи как завершенной. |
| taskClick | Сведения содержат соответствующий объект `task` | Возникает, когда пользователь щелкает или нажимает задачу. |
| taskRemoved | Сведения содержат соответствующий объект `task` | Возникает, если удалена существующая задача. |

## <a name="templates"></a>Шаблоны

Компонент `tasks` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента. Чтобы указать шаблон, добавьте элемент `<template>` в компонент и установите для параметра `data-type` одно из следующих значений.

| Тип данных     | Контекст данных              | Описание                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| task     | задача: объект задачи планировщика | заменяет всю задачу по умолчанию. |
| task-details | задача: объект задачи планировщика | шаблон заменяет раздел подробностей задачи. |

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

Этот элемент управления использует следующие API и разрешения Microsoft Graph.

| Конфигурация | Разрешение | API |
| ------------- | ---------- | --- |
| `groupId` набор `dataSource` и заме- `TasksSource.planner` | Group.Read.All | [/groups/${group-id}/planner/plans](/graph/api/plannergroup-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http) |
| `targetId` набор `dataSource` и заме- `TasksSource.todo` | Tasks.Read | [/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http) |
| `targetId` установить и `dataSource` установить что-то другое, чем `TasksSource.todo` | Group.Read.All | [/planner/plans/${planId}](/graph/api/plannerplan-get?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http) |
| `dataSource` установлено, что `TasksSource.planner` | Group.Read.All | [/me/planner/plans](/graph/api/planneruser-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http) |
| `dataSource` установлено, что `TasksSource.todo` | Tasks.Read | [/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http) |
| `addTask` установлено `true` и `dataSource` установлено `TasksSource.planner` | Group.ReadWrite.All | [/planner/tasks](/graph/api/planner-post-tasks?view=graph-rest-1.0&tabs=http) |
| `addTask` установлено `true` и `dataSource` установлено `TasksSource.todo` | Tasks.ReadWrite | [/me/outlook/taskFolders/${parentFolderId}/tasks](/graph/api/outlookuser-post-tasks?view=graph-rest-beta&tabs=csharp) |

Для источника данных Microsoft Planner для получения и чтения требуется разрешение Groups.Read.All. Добавление, обновление или удаление задач требует разрешения Groups.ReadWrite.All.

## <a name="authentication"></a>Проверка подлинности

В компоненте задач используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).

## <a name="cache"></a>Кэш

Компонент `mgt-tasks` не кэшет данных.
