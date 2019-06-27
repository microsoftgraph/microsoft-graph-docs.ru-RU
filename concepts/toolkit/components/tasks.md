---
title: Компонент Tasks в наборе инструментов Microsoft Graph
description: Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи. Она работает с любой из задач в планировщике (Майкрософт) или в Microsoft.
localization_priority: Normal
author: benotter
ms.openlocfilehash: 3c2017acd7fe054c71a609c8d908e119e12a590b
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243080"
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
| `dataSource` | `data-source="todo/planner"` | Задает источник данных для задач — либо задача Майкрософт, либо планировщик Microsoft. Значение по умолчанию: `planner`. |
| `readOnly` | `read-only` | Задает для интерфейса задачи права только на чтение (Добавление или удаление задач не выполняется). Значение по умолчанию: `false`. |
| `initialId` | `initial-id="planner_id/folder_id"` | Задает для первоначального отображения планировщик или папку предоставленный идентификатор. |
| `initialBucketId` | `initial-bucket-id="bucket_id"` | Задает предоставленный идентификатор в исходном сегменте (только для источника данных с планировщиком). |
| `targetId` | `target-id="planner_id/folder_id"` | Блокирует интерфейс Tasks до указанного планировщика или идентификатора папки. |
| `targetBucketId` | `target-bucket-id="bucket_id"` | Блокирует интерфейс Tasks до указанного идентификатора контейнера (только для источника данных планировщика). |

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

| Ресурс | Разрешение или область |
| - | - |
| /ме/Планнер/Планс | `Group.Read.All` |
| /Планнер/Планс/$ {ID} | `Group.Read.All`, `Group.ReadWrite.All` |
| /Планнер/таскс | `Group.ReadWrite.All` |
| /Ме/Аутлук/таскграупс | `Tasks.Read` |
| /Ме/Аутлук/таскфолдерс | `Tasks.Read`, `Tasks.ReadWrite` |
| /ме/Аутлук/таскс | `Tasks.ReadWrite` |

Для получения источника данных планировщика (Майкрософт) для получения и чтения задач требуются разрешения Group. Read. ALL. Для добавления, обновления или удаления задач требуются разрешения Group. ReadWrite. ALL.

Для источника данных Microsoft TODO необходимо разрешение Tasks. Read для получения и чтения задач. Для добавления, обновления или удаления задач требуется разрешение Tasks. ReadWrite.

## <a name="authentication"></a>Проверка подлинности

Компонент Tasks использует глобальный поставщик проверки подлинности, описанный в [документации по проверке](./../providers.md)подлинности.
