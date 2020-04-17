---
title: Компонент Tasks в наборе инструментов Microsoft Graph
description: Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи. Она работает с любой из задач в планировщике (Майкрософт) или в Microsoft.
localization_priority: Normal
author: benotter
ms.openlocfilehash: cfd248ca7cb240cd724b8df863383b308121db4b
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144277"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Компонент Tasks в наборе инструментов Microsoft Graph

Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи. Она работает с задачами в планировщике (Майкрософт) или в Microsoft.  

Кроме того, пользователь может назначить одну или несколько пользователей Microsoft Graph для задачи. Более подробную информацию о назначениях Microsoft Graph можно узнать в разделе [планнерассигнментс](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).

## <a name="example"></a>Пример

В следующем примере отображаются задачи планировщика Microsoft, вошедшего в систему, с `mgt-tasks` помощью компонента. С помощью редактора кода можно увидеть, как [Свойства](#properties) изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[Откройте этот пример в меню упр. dev.](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a>Свойства

| Атрибут | Свойство | Описание |
| -- | -- | -- |
| Data-Source = "TODO/Planner" | Данных | Перечисление для настройки источника данных задач — либо задачи Майкрософт, либо планировщика (Майкрософт). Значение по умолчанию: `planner`. |
| только для чтения | Статического | Логическое значение, указывающее, что интерфейс задачи должен быть доступен только для чтения (Добавление или удаление задач не выполняется). Значение по умолчанию: `false`. |
| скрыть — заголовок | хидехеадер | Логическое значение для отображения или скрытия заголовка компонента. Значение по умолчанию: `false`. |
| Параметры скрытия | хидеоптионс | Логическое значение для отображения или скрытия параметров в разделе "задачи". Значение по умолчанию: `false`.
| Initial-ID = "planner_id/folder_id" | инитиалид | Строковое значение, чтобы задать для первоначально отображаемого планировщика или папки предоставленный идентификатор. |
| Initial — сегмент — ID = "bucket_id" | инитиалбуккетид | Строковый идентификатор для установки начального сегмента (только для источника данных с планировщиком) на предоставленный идентификатор. |
| Target-ID = "planner_id/folder_id"| targetId | Идентификатор строки, чтобы заблокировать интерфейс Tasks до указанного планировщика или идентификатора папки. |
| Target — сегмент — ID = "bucket_id" |таржетбуккетид  | Идентификатор строки для блокировки интерфейса Tasks до указанного идентификатора контейнера (только для источника данных планировщика). |
| Идентификатор группы | groupId  | Строковый идентификатор для блокировки интерфейса Tasks до идентификатора группы (только для источника данных планировщика). |
| Недоступно | исневтасквисибле  | Определяет, отображается ли новое представление задач во время отображения. |
| Недоступно | таскфилтер  | Необязательная функция для фильтрации задач, которые отображаются для пользователя. |

В следующем примере показаны задачи планировщика с ИДЕНТИФИКАТОРом *12345* , которые не позволяют пользователю создавать новые задачи.

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

В приведенном ниже примере показано, как фильтровать задачи, для которых только задано значение *Category3* .

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
| тасккликк | Сведения содержит соответствующий `task` объект | Возникает, когда пользователь щелкает или нажимает задачу. |

## <a name="templates"></a>Шаблоны

`tasks` Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента. Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений:

| Тип данных     | Контекст данных              | Описание                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| task     | Задача: планировщик или объект задачи "задача" | заменяет всю задачу по умолчанию. |
| Задача — сведения | Задача: планировщик или объект задачи "задача" | шаблон заменяет раздел сведений о задаче. |

В следующем примере определяется шаблон для компонента Tasks.

```html
    <mgt-tasks data-source="todo">
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

Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.

| Ресурс | Разрешение |
| - | - |
| /ме/планнер/планс | Group.Read.All |
| /Планнер/Планс/$ {ID} | Group.Read.All, Group.ReadWrite.All |
| /планнер/таскс | Group.ReadWrite.All |
| /ме/аутлук/таскграупс | Tasks.Read |
| /ме/аутлук/таскфолдерс | Tasks. Read, Tasks. ReadWrite |
| /ме/аутлук/таскс | Tasks.ReadWrite |
| /граупс/$ {Group – ID}/Планнер/Планс | Group.Read.All, Group.ReadWrite.All |

Для получения источника данных планировщика (Майкрософт) для получения и чтения задач требуются разрешения Group. Read. ALL. Для добавления, обновления или удаления задач требуются разрешения Group. ReadWrite. ALL.

Для источника данных Microsoft TODO необходимо разрешение Tasks. Read для получения и чтения задач. Для добавления, обновления или удаления задач требуется разрешение Tasks. ReadWrite.

## <a name="authentication"></a>Проверка подлинности

Компонент Tasks использует глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md).
