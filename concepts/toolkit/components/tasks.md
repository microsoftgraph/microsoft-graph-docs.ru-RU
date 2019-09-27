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
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d9183-104">Компонент Tasks в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d9183-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d9183-105">Компонент Tasks позволяет пользователю просматривать, добавлять, удалять, выполнять или изменять задачи.</span><span class="sxs-lookup"><span data-stu-id="d9183-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="d9183-106">Она работает с задачами в планировщике (Майкрософт) или в Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d9183-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>

## <a name="example"></a><span data-ttu-id="d9183-107">Пример</span><span class="sxs-lookup"><span data-stu-id="d9183-107">Example</span></span>

[<span data-ttu-id="d9183-108">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="d9183-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a><span data-ttu-id="d9183-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9183-109">Properties</span></span>

| <span data-ttu-id="d9183-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9183-110">Property</span></span> | <span data-ttu-id="d9183-111">Атрибут</span><span class="sxs-lookup"><span data-stu-id="d9183-111">Attribute</span></span> | <span data-ttu-id="d9183-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d9183-112">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="d9183-113">Данных</span><span class="sxs-lookup"><span data-stu-id="d9183-113">dataSource</span></span> | <span data-ttu-id="d9183-114">Data-Source = "TODO/Planner"</span><span class="sxs-lookup"><span data-stu-id="d9183-114">data-source="todo/planner"</span></span> | <span data-ttu-id="d9183-115">Перечисление для настройки источника данных задач — либо задачи Майкрософт, либо планировщика (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="d9183-115">An enumeration to configure the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="d9183-116">Значение по умолчанию: `planner`.</span><span class="sxs-lookup"><span data-stu-id="d9183-116">Default is `planner`.</span></span> |
| <span data-ttu-id="d9183-117">Статического</span><span class="sxs-lookup"><span data-stu-id="d9183-117">readOnly</span></span> | <span data-ttu-id="d9183-118">только для чтения</span><span class="sxs-lookup"><span data-stu-id="d9183-118">read-only</span></span> | <span data-ttu-id="d9183-119">Логическое значение, указывающее, что интерфейс задачи должен быть доступен только для чтения (Добавление или удаление задач не выполняется).</span><span class="sxs-lookup"><span data-stu-id="d9183-119">A boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="d9183-120">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="d9183-120">Default is `false`.</span></span> |
| <span data-ttu-id="d9183-121">хидехеадер</span><span class="sxs-lookup"><span data-stu-id="d9183-121">hideHeader</span></span> | <span data-ttu-id="d9183-122">скрыть — заголовок</span><span class="sxs-lookup"><span data-stu-id="d9183-122">hide-header</span></span> | <span data-ttu-id="d9183-123">Логическое значение для отображения или скрытия заголовка компонента.</span><span class="sxs-lookup"><span data-stu-id="d9183-123">A boolean to show or hide the header of the component.</span></span> <span data-ttu-id="d9183-124">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="d9183-124">Default is `false`.</span></span> |
| <span data-ttu-id="d9183-125">инитиалид</span><span class="sxs-lookup"><span data-stu-id="d9183-125">initialId</span></span> | <span data-ttu-id="d9183-126">Initial-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="d9183-126">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="d9183-127">Строковое значение, чтобы задать для первоначально отображаемого планировщика или папки предоставленный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="d9183-127">A string id to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="d9183-128">инитиалбуккетид</span><span class="sxs-lookup"><span data-stu-id="d9183-128">initialBucketId</span></span> | <span data-ttu-id="d9183-129">Initial — сегмент — ID = "BUCKET_ID"</span><span class="sxs-lookup"><span data-stu-id="d9183-129">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="d9183-130">Строковый идентификатор для установки начального сегмента (только для источника данных с планировщиком) на предоставленный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="d9183-130">A string id to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="d9183-131">targetId</span><span class="sxs-lookup"><span data-stu-id="d9183-131">targetId</span></span> | <span data-ttu-id="d9183-132">Target-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="d9183-132">target-id="planner_id/folder_id"</span></span> | <span data-ttu-id="d9183-133">Идентификатор строки, чтобы заблокировать интерфейс Tasks до указанного планировщика или идентификатора папки.</span><span class="sxs-lookup"><span data-stu-id="d9183-133">A string id to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="d9183-134">таржетбуккетид</span><span class="sxs-lookup"><span data-stu-id="d9183-134">targetBucketId</span></span> | <span data-ttu-id="d9183-135">Target — сегмент — ID = "BUCKET_ID"</span><span class="sxs-lookup"><span data-stu-id="d9183-135">target-bucket-id="bucket_id"</span></span> | <span data-ttu-id="d9183-136">Идентификатор строки для блокировки интерфейса Tasks до указанного идентификатора контейнера (только для источника данных планировщика).</span><span class="sxs-lookup"><span data-stu-id="d9183-136">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |

<span data-ttu-id="d9183-137">Ниже приведен пример.</span><span class="sxs-lookup"><span data-stu-id="d9183-137">The following is an example.</span></span>

````html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
````

## <a name="custom-css-variables"></a><span data-ttu-id="d9183-138">Настраиваемые переменные CSS</span><span class="sxs-lookup"><span data-stu-id="d9183-138">Custom CSS variables</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="d9183-139">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d9183-139">Microsoft Graph permissions</span></span>

<span data-ttu-id="d9183-140">Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d9183-140">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="d9183-141">Ресурс</span><span class="sxs-lookup"><span data-stu-id="d9183-141">Resource</span></span> | <span data-ttu-id="d9183-142">Разрешение</span><span class="sxs-lookup"><span data-stu-id="d9183-142">Permission</span></span> |
| - | - |
| <span data-ttu-id="d9183-143">/ме/планнер/планс</span><span class="sxs-lookup"><span data-stu-id="d9183-143">/me/planner/plans</span></span> | <span data-ttu-id="d9183-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9183-144">Group.Read.All</span></span> |
| <span data-ttu-id="d9183-145">/Планнер/Планс/$ {ID}</span><span class="sxs-lookup"><span data-stu-id="d9183-145">/planner/plans/${id}</span></span> | <span data-ttu-id="d9183-146">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9183-146">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d9183-147">/планнер/таскс</span><span class="sxs-lookup"><span data-stu-id="d9183-147">/planner/tasks</span></span> | <span data-ttu-id="d9183-148">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9183-148">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d9183-149">/ме/аутлук/таскграупс</span><span class="sxs-lookup"><span data-stu-id="d9183-149">/me/outlook/taskGroups</span></span> | <span data-ttu-id="d9183-150">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d9183-150">Tasks.Read</span></span> |
| <span data-ttu-id="d9183-151">/ме/аутлук/таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="d9183-151">/me/outlook/taskFolders</span></span> | <span data-ttu-id="d9183-152">Tasks. Read, Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9183-152">Tasks.Read, Tasks.ReadWrite</span></span> |
| <span data-ttu-id="d9183-153">/ме/аутлук/таскс</span><span class="sxs-lookup"><span data-stu-id="d9183-153">/me/outlook/tasks</span></span> | <span data-ttu-id="d9183-154">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9183-154">Tasks.ReadWrite</span></span> |

<span data-ttu-id="d9183-155">Для получения источника данных планировщика (Майкрософт) для получения и чтения задач требуются разрешения Group. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="d9183-155">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="d9183-156">Для добавления, обновления или удаления задач требуются разрешения Group. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="d9183-156">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="d9183-157">Для источника данных Microsoft TODO необходимо разрешение Tasks. Read для получения и чтения задач.</span><span class="sxs-lookup"><span data-stu-id="d9183-157">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="d9183-158">Для добавления, обновления или удаления задач требуется разрешение Tasks. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="d9183-158">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="d9183-159">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="d9183-159">Authentication</span></span>

<span data-ttu-id="d9183-160">Компонент Tasks использует глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="d9183-160">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
