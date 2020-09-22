---
title: Использование API Microsoft To Do
description: API Microsoft Graph можно использовать для создания приложения, подключающегося к задачам в Microsoft To Do.
author: avijityadav
localization_priority: Priority
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: 76dc89caeb0a39d9dd0f40c1bcf046ffe9fe3f9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973533"
---
# <a name="use-the-microsoft-to-do-api"></a><span data-ttu-id="6de82-103">Использование API Microsoft To Do</span><span class="sxs-lookup"><span data-stu-id="6de82-103">Use the Microsoft To Do API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6de82-104">Используйте API To Do Microsoft Graph для создания приложения, подключающегося к задачам в клиентах Microsoft To Do.</span><span class="sxs-lookup"><span data-stu-id="6de82-104">Use the Microsoft Graph To Do API to create an app that connects with tasks across Microsoft To Do clients.</span></span> <span data-ttu-id="6de82-105">Создавайте разнообразные возможности с задачами, например следующие:</span><span class="sxs-lookup"><span data-stu-id="6de82-105">Build a variety of experiences with tasks, such as the following:</span></span>

* <span data-ttu-id="6de82-106">Создавайте задачи из рабочего процесса приложения, например из электронной почты или уведомлений, и сохраняйте их в To Do.</span><span class="sxs-lookup"><span data-stu-id="6de82-106">Create tasks from your app’s workflow, for example, from email or notifications, and save them in To Do.</span></span> <span data-ttu-id="6de82-107">Используйте объект [linkedResource](linkedresource.md), чтобы сохранить ссылку, ведущую к вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="6de82-107">Use the [linkedResource](linkedresource.md) entity to store the link back to your app.</span></span>
* <span data-ttu-id="6de82-108">Синхронизируйте существующие задачи приложения с помощью To Do и создайте единое представление задач, чтобы лучше определить приоритеты и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="6de82-108">Sync your app’s existing tasks with To Do and create a single task view for better prioritization and manageability.</span></span>
* <span data-ttu-id="6de82-109">Управляйте задачами To Do в пользовательском бизнес-приложении.</span><span class="sxs-lookup"><span data-stu-id="6de82-109">Manage To Do tasks in a custom business application.</span></span>

<span data-ttu-id="6de82-110">В настоящее время этот API поддерживает только разрешения, делегированные вошедшим пользователем.</span><span class="sxs-lookup"><span data-stu-id="6de82-110">Currently, the API supports only permissions delegated by the signed-in user.</span></span>
 
<span data-ttu-id="6de82-111">Прежде чем приступить к работе с API To Do, ознакомьтесь с ресурсами и их связью между собой.</span><span class="sxs-lookup"><span data-stu-id="6de82-111">Before starting with the To Do API, take a look at the resources and how they relate to one another.</span></span>

![Объекты API To Do](/graph/images/todo-api-entities.png)

## <a name="task-list"></a><span data-ttu-id="6de82-113">Список задач</span><span class="sxs-lookup"><span data-stu-id="6de82-113">Task list</span></span>

<span data-ttu-id="6de82-114">Объект [todoTaskList](./todotasklist.md) представляет логический контейнер ресурсов [todoTask](./todotask.md).</span><span class="sxs-lookup"><span data-stu-id="6de82-114">A [todoTaskList](./todotasklist.md) represents a logical container of [todoTask](./todotask.md) resources.</span></span> <span data-ttu-id="6de82-115">В настоящее время вы можете создавать задачи только в списке задач.</span><span class="sxs-lookup"><span data-stu-id="6de82-115">You can currently create tasks only in a task list.</span></span> <span data-ttu-id="6de82-116">Чтобы [получить все свои списки задач](../api/todotasklist-get.md), выполните следующий HTTP-запрос:</span><span class="sxs-lookup"><span data-stu-id="6de82-116">To [get all your task lists](../api/todotasklist-get.md), make the following HTTP request:</span></span>

``` http
GET /me/todo/lists
```

## <a name="task"></a><span data-ttu-id="6de82-117">Задача</span><span class="sxs-lookup"><span data-stu-id="6de82-117">Task</span></span>

<span data-ttu-id="6de82-118">Объект [todoTask](./todotask.md) представляет задачу, т. е. рабочий или личный элемент, который можно отследить и завершить.</span><span class="sxs-lookup"><span data-stu-id="6de82-118">A [todoTask](./todotask.md) represents a task, i.e. a piece of work or personal item that can be tracked and completed.</span></span> <span data-ttu-id="6de82-119">Чтобы получить свои задачи из списка задач, выполните следующий HTTP-запрос:</span><span class="sxs-lookup"><span data-stu-id="6de82-119">To get your tasks from a task list, make the following HTTP request:</span></span>
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
```

## <a name="linked-resource"></a><span data-ttu-id="6de82-120">Связанный ресурс</span><span class="sxs-lookup"><span data-stu-id="6de82-120">Linked resource</span></span>

<span data-ttu-id="6de82-121">Объект [linkedResource](linkedresource.md) представляет любой элемент из партнерского приложения, связанный с задачей, например такой элемент, как письмо, из которого создана задача.</span><span class="sxs-lookup"><span data-stu-id="6de82-121">A [linkedResource](linkedresource.md) represents any item from a partner application related to the task, e.g. an item like email from where a task was created.</span></span> <span data-ttu-id="6de82-122">Вы можете использовать его для хранения данных и связи с соответствующим элементом в приложении.</span><span class="sxs-lookup"><span data-stu-id="6de82-122">You can use it to store information and the link back to the related item in your app.</span></span> <span data-ttu-id="6de82-123">Чтобы получить связанный ресурс из задачи, выполните следующий HTTP-запрос:</span><span class="sxs-lookup"><span data-stu-id="6de82-123">To get a linked resource from a task, make the following HTTP request:</span></span>
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/linkedresources/{linkedResourceId}
```

## <a name="track-changes-using-delta-query"></a><span data-ttu-id="6de82-124">Отслеживание изменений с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="6de82-124">Track changes using delta query</span></span>

<span data-ttu-id="6de82-125">Для повышения производительности вы можете использовать локальный кэш объектов и периодически синхронизировать локальный кэш с сервером, используя [разностный запрос](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="6de82-125">For performance reasons, you may want to maintain a local cache of objects, and periodically synchronize the local cache with the server, using [delta query](/graph/delta-query-overview).</span></span> 

<span data-ttu-id="6de82-126">Разностный запрос поддерживают следующие ресурсы API To Do:</span><span class="sxs-lookup"><span data-stu-id="6de82-126">The following To Do API resources support delta query:</span></span>
* <span data-ttu-id="6de82-127">Коллекция [todoTask](./todotask.md) в списке задач</span><span class="sxs-lookup"><span data-stu-id="6de82-127">[todoTask](./todotask.md) collection in a task list</span></span>
* [<span data-ttu-id="6de82-128">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="6de82-128">todoTaskList</span></span>](./todotasklist.md)

## <a name="whats-new"></a><span data-ttu-id="6de82-129">Новые возможности</span><span class="sxs-lookup"><span data-stu-id="6de82-129">What's new</span></span>
<span data-ttu-id="6de82-130">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="6de82-130">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

