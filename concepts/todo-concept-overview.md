---
title: Обзор API To Do
description: Приложение To Do предоставляет простой способ управления задачами и планирования дня
author: avijityadav
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 34dc63ab14bc6cc1a2c118e6a77f9f6cc597bccc
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796747"
---
# <a name="to-do-api-overview"></a><span data-ttu-id="50742-103">Обзор API To Do</span><span class="sxs-lookup"><span data-stu-id="50742-103">To Do API overview</span></span>
<span data-ttu-id="50742-104">Приложение Microsoft To Do предоставляет пользователям простой способ управления задачами и планирования дня.</span><span class="sxs-lookup"><span data-stu-id="50742-104">Microsoft To Do provides a simple way for people to manage their tasks and plan their day.</span></span> <span data-ttu-id="50742-105">Задачи упорядочиваются в списках задач, доступных в клиентах To Do, Outlook и Teams с любого устройства.</span><span class="sxs-lookup"><span data-stu-id="50742-105">Tasks are organized in task lists, which can be accessed across To Do clients, Outlook and Teams from any device.</span></span>

<span data-ttu-id="50742-106">**Приложение To Do для Windows**</span><span class="sxs-lookup"><span data-stu-id="50742-106">**To Do Windows app**</span></span>

<span data-ttu-id="50742-107">![Снимок экрана: приложение Microsoft To Do для Windows](./images/todo-windows-app.png "Изображение приложения Microsoft To Do для Windows")</span><span class="sxs-lookup"><span data-stu-id="50742-107">![Screenshot of a Microsoft To Do Windows App](./images/todo-windows-app.png "Image of Microsoft To Do Windows App")</span></span>

## <a name="why-integrate-with-to-do"></a><span data-ttu-id="50742-108">Зачем нужна интеграция с To Do?</span><span class="sxs-lookup"><span data-stu-id="50742-108">Why integrate with To Do?</span></span>

### <a name="ease-of-organizing-and-tracking-tasks"></a><span data-ttu-id="50742-109">Простота упорядочения и отслеживания задач</span><span class="sxs-lookup"><span data-stu-id="50742-109">Ease of organizing and tracking tasks</span></span>
<span data-ttu-id="50742-110">Microsoft To Do помогает создать список для любых задач, от рабочих заданий до домашних проектов и покупок.</span><span class="sxs-lookup"><span data-stu-id="50742-110">Microsoft To Do helps you create a list for anything, from work assignments to home projects to groceries.</span></span> <span data-ttu-id="50742-111">Вы можете отслеживать крайние сроки, добавляя напоминания, даты выполнения и заметки.</span><span class="sxs-lookup"><span data-stu-id="50742-111">You can keep track of deadlines by adding reminders, due dates, and notes.</span></span> <span data-ttu-id="50742-112">Вы можете открыть свой список откуда угодно с помощью приложений Microsoft To Do для iOS, Android, Mac, Windows и Интернета.</span><span class="sxs-lookup"><span data-stu-id="50742-112">You can access your lists from anywhere with the Microsoft To Do apps for iOS, Android, Mac, Windows, and the web.</span></span> 

### <a name="integrate-across-microsoft-365"></a><span data-ttu-id="50742-113">Интеграция в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="50742-113">Integrate across Microsoft 365</span></span>
<span data-ttu-id="50742-114">Приложение To Do — единый центр для личных задач в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="50742-114">To Do is the single destination for personal tasks in Microsoft 365.</span></span> <span data-ttu-id="50742-115">Оно тесно интегрировано с центрами Microsoft 365, Outlook и Teams.</span><span class="sxs-lookup"><span data-stu-id="50742-115">So it’s deeply integrated with Microsoft 365 hubs, Outlook, and Teams.</span></span> <span data-ttu-id="50742-116">Задачи, созданные в этих продуктах, синхронизируются с To Do, чтобы вы могли обращаться к ним и управлять ими на разных устройствах.</span><span class="sxs-lookup"><span data-stu-id="50742-116">Tasks created in those products sync with To Do so you can access and manage them across devices.</span></span> <span data-ttu-id="50742-117">Благодаря интеграции To Do вы можете связываться с миллионами пользователей, использующих To Do, для сбора задач из Outlook и Teams в едином объединенном представлении.</span><span class="sxs-lookup"><span data-stu-id="50742-117">To Do integration can help you reach millions of users who use To Do to gather tasks from Outlook and Teams into one integrated view.</span></span>  

### <a name="support-task-completion-using-linked-resources"></a><span data-ttu-id="50742-118">Поддержка выполнения задач с помощью связанных ресурсов</span><span class="sxs-lookup"><span data-stu-id="50742-118">Support task completion using linked resources</span></span>
<span data-ttu-id="50742-119">Microsoft To Do предоставляет новый объект под названием _связанный ресурс_ . Вы можете использовать его для создания задач, которые могут быть связаны со своими исходными источниками.</span><span class="sxs-lookup"><span data-stu-id="50742-119">Microsoft To Do provides a new entity called _linked resource_ , which you can use to create tasks that can link back to their original sources.</span></span> <span data-ttu-id="50742-120">Это позволяет легко интегрировать To Do в свой рабочий процесс, создавая задачи, связанные с вашим продуктом или службой.</span><span class="sxs-lookup"><span data-stu-id="50742-120">You can use this to seamlessly integrate To Do in your workflow by creating tasks that link to your product or service.</span></span> 

## <a name="common-to-do-api-operations"></a><span data-ttu-id="50742-121">Распространенные операции API To Do</span><span class="sxs-lookup"><span data-stu-id="50742-121">Common To Do API operations</span></span>

|<span data-ttu-id="50742-122">Операция</span><span class="sxs-lookup"><span data-stu-id="50742-122">Operation</span></span>|<span data-ttu-id="50742-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="50742-123">Request</span></span>|
|:--------|:--|
| <span data-ttu-id="50742-124">Перечисление всех списков задач</span><span class="sxs-lookup"><span data-stu-id="50742-124">List all the task lists</span></span> | <span data-ttu-id="50742-125">GET https://graph.microsoft.com/v1.0/me/todo/lists</span><span class="sxs-lookup"><span data-stu-id="50742-125">GET https://graph.microsoft.com/v1.0/me/todo/lists</span></span> |
| <span data-ttu-id="50742-126">Перечисление всех задач в списке задач</span><span class="sxs-lookup"><span data-stu-id="50742-126">List all tasks in a task list</span></span> | <span data-ttu-id="50742-127">GET https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks</span><span class="sxs-lookup"><span data-stu-id="50742-127">GET https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks</span></span> |
| <span data-ttu-id="50742-128">Создание задачи</span><span class="sxs-lookup"><span data-stu-id="50742-128">Create a new task</span></span> | <span data-ttu-id="50742-129">POST https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks</span><span class="sxs-lookup"><span data-stu-id="50742-129">POST https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks</span></span> |
| <span data-ttu-id="50742-130">Обновление задачи</span><span class="sxs-lookup"><span data-stu-id="50742-130">Update a task</span></span> | <span data-ttu-id="50742-131">PATCH https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span><span class="sxs-lookup"><span data-stu-id="50742-131">PATCH https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span></span> |
| <span data-ttu-id="50742-132">Удаление задачи</span><span class="sxs-lookup"><span data-stu-id="50742-132">Delete a task</span></span> | <span data-ttu-id="50742-133">DELETE https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span><span class="sxs-lookup"><span data-stu-id="50742-133">DELETE https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span></span> |

## <a name="api-reference"></a><span data-ttu-id="50742-134">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="50742-134">API reference</span></span>
<span data-ttu-id="50742-135">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="50742-135">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="50742-136">API To Do в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="50742-136">To Do API in Microsoft Graph</span></span>](/graph/api/resources/todo-overview)
