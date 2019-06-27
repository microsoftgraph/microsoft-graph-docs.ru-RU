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
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="3705a-104">Компонент Tasks в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3705a-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="3705a-105">Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи.</span><span class="sxs-lookup"><span data-stu-id="3705a-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="3705a-106">Она работает с задачами в планировщике (Майкрософт) или в Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3705a-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>

## <a name="example"></a><span data-ttu-id="3705a-107">Пример</span><span class="sxs-lookup"><span data-stu-id="3705a-107">Example</span></span>

[<span data-ttu-id="3705a-108">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="3705a-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a><span data-ttu-id="3705a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3705a-109">Properties</span></span>

| <span data-ttu-id="3705a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3705a-110">Property</span></span> | <span data-ttu-id="3705a-111">Атрибут</span><span class="sxs-lookup"><span data-stu-id="3705a-111">Attribute</span></span> | <span data-ttu-id="3705a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3705a-112">Description</span></span> |
| -- | -- | -- |
| `dataSource` | `data-source="todo/planner"` | <span data-ttu-id="3705a-113">Задает источник данных для задач — либо задача Майкрософт, либо планировщик Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3705a-113">Sets the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="3705a-114">Значение по умолчанию: `planner`.</span><span class="sxs-lookup"><span data-stu-id="3705a-114">Default is `planner`.</span></span> |
| `readOnly` | `read-only` | <span data-ttu-id="3705a-115">Задает для интерфейса задачи права только на чтение (Добавление или удаление задач не выполняется).</span><span class="sxs-lookup"><span data-stu-id="3705a-115">Sets the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="3705a-116">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="3705a-116">Default is `false`.</span></span> |
| `initialId` | `initial-id="planner_id/folder_id"` | <span data-ttu-id="3705a-117">Задает для первоначального отображения планировщик или папку предоставленный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="3705a-117">Sets the initially displayed planner or folder to the provided ID.</span></span> |
| `initialBucketId` | `initial-bucket-id="bucket_id"` | <span data-ttu-id="3705a-118">Задает предоставленный идентификатор в исходном сегменте (только для источника данных с планировщиком).</span><span class="sxs-lookup"><span data-stu-id="3705a-118">Sets the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| `targetId` | `target-id="planner_id/folder_id"` | <span data-ttu-id="3705a-119">Блокирует интерфейс Tasks до указанного планировщика или идентификатора папки.</span><span class="sxs-lookup"><span data-stu-id="3705a-119">Locks the tasks interface to the provided planner or folder ID.</span></span> |
| `targetBucketId` | `target-bucket-id="bucket_id"` | <span data-ttu-id="3705a-120">Блокирует интерфейс Tasks до указанного идентификатора контейнера (только для источника данных планировщика).</span><span class="sxs-lookup"><span data-stu-id="3705a-120">Locks the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |

<span data-ttu-id="3705a-121">Ниже приведен пример.</span><span class="sxs-lookup"><span data-stu-id="3705a-121">The following is an example.</span></span>

````html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
````

## <a name="custom-css-variables"></a><span data-ttu-id="3705a-122">Настраиваемые переменные CSS</span><span class="sxs-lookup"><span data-stu-id="3705a-122">Custom CSS variables</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="3705a-123">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3705a-123">Microsoft Graph permissions</span></span>

<span data-ttu-id="3705a-124">Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3705a-124">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="3705a-125">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3705a-125">Resource</span></span> | <span data-ttu-id="3705a-126">Разрешение или область</span><span class="sxs-lookup"><span data-stu-id="3705a-126">Permission/scope</span></span> |
| - | - |
| <span data-ttu-id="3705a-127">/ме/Планнер/Планс</span><span class="sxs-lookup"><span data-stu-id="3705a-127">/me/planner/plans</span></span> | `Group.Read.All` |
| <span data-ttu-id="3705a-128">/Планнер/Планс/$ {ID}</span><span class="sxs-lookup"><span data-stu-id="3705a-128">/planner/plans/${id}</span></span> | <span data-ttu-id="3705a-129">`Group.Read.All`, `Group.ReadWrite.All`</span><span class="sxs-lookup"><span data-stu-id="3705a-129"></span></span> |
| <span data-ttu-id="3705a-130">/Планнер/таскс</span><span class="sxs-lookup"><span data-stu-id="3705a-130">/planner/tasks</span></span> | `Group.ReadWrite.All` |
| <span data-ttu-id="3705a-131">/Ме/Аутлук/таскграупс</span><span class="sxs-lookup"><span data-stu-id="3705a-131">/me/outlook/taskGroups</span></span> | `Tasks.Read` |
| <span data-ttu-id="3705a-132">/Ме/Аутлук/таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="3705a-132">/me/outlook/taskFolders</span></span> | <span data-ttu-id="3705a-133">`Tasks.Read`, `Tasks.ReadWrite`</span><span class="sxs-lookup"><span data-stu-id="3705a-133"></span></span> |
| <span data-ttu-id="3705a-134">/ме/Аутлук/таскс</span><span class="sxs-lookup"><span data-stu-id="3705a-134">/me/outlook/tasks</span></span> | `Tasks.ReadWrite` |

<span data-ttu-id="3705a-135">Для получения источника данных планировщика (Майкрософт) для получения и чтения задач требуются разрешения Group. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="3705a-135">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="3705a-136">Для добавления, обновления или удаления задач требуются разрешения Group. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="3705a-136">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="3705a-137">Для источника данных Microsoft TODO необходимо разрешение Tasks. Read для получения и чтения задач.</span><span class="sxs-lookup"><span data-stu-id="3705a-137">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="3705a-138">Для добавления, обновления или удаления задач требуется разрешение Tasks. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="3705a-138">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="3705a-139">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="3705a-139">Authentication</span></span>

<span data-ttu-id="3705a-140">Компонент Tasks использует глобальный поставщик проверки подлинности, описанный в [документации по проверке](./../providers.md)подлинности.</span><span class="sxs-lookup"><span data-stu-id="3705a-140">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
