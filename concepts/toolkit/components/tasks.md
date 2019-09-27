---
title: Компонент Tasks в наборе инструментов Microsoft Graph
description: Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи. Она работает с любой из задач в планировщике (Майкрософт) или в Microsoft.
localization_priority: Normal
author: benotter
ms.openlocfilehash: f8366842be9319e8c89d05fa23bc488cde49359a
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275824"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Компонент Tasks в наборе инструментов Microsoft Graph

Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи. Она работает с задачами в планировщике (Майкрософт) или в Microsoft.

## <a name="example"></a>Пример

[Пример жсфиддле](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a>Свойства

| Свойство | Атрибут | Описание |
| -- | -- | -- |
| Данных | Data-Source = "TODO/Planner" | Перечисление для настройки источника данных задач — либо задачи Майкрософт, либо планировщика (Майкрософт). Значение по умолчанию: `planner`. |
| Статического | только для чтения | Логическое значение, указывающее, что интерфейс задачи должен быть доступен только для чтения (Добавление или удаление задач не выполняется). Значение по умолчанию: `false`. |
| хидехеадер | скрыть — заголовок | Логическое значение для отображения или скрытия заголовка компонента. Значение по умолчанию: `false`. |
| инитиалид | Initial-ID = "planner_id/folder_id" | Строковое значение, чтобы задать для первоначально отображаемого планировщика или папки предоставленный идентификатор. |
| инитиалбуккетид | Initial — сегмент — ID = "BUCKET_ID" | Строковый идентификатор для установки начального сегмента (только для источника данных с планировщиком) на предоставленный идентификатор. |
| targetId | Target-ID = "planner_id/folder_id" | Идентификатор строки, чтобы заблокировать интерфейс Tasks до указанного планировщика или идентификатора папки. |
| таржетбуккетид | Target — сегмент — ID = "BUCKET_ID" | Идентификатор строки для блокировки интерфейса Tasks до указанного идентификатора контейнера (только для источника данных планировщика). |

Ниже приведен пример.

````html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
````

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
}
````

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

Для получения источника данных планировщика (Майкрософт) для получения и чтения задач требуются разрешения Group. Read. ALL. Для добавления, обновления или удаления задач требуются разрешения Group. ReadWrite. ALL.

Для источника данных Microsoft TODO необходимо разрешение Tasks. Read для получения и чтения задач. Для добавления, обновления или удаления задач требуется разрешение Tasks. ReadWrite.

## <a name="authentication"></a>Проверка подлинности

Компонент Tasks использует глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md).
