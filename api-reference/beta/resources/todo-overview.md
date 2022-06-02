---
title: Использование API Microsoft To Do
description: С помощью интерфейса API Microsoft Graph, использующего todoTask, можно создать приложение, подключающееся к задачам в Microsoft To Do.
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: e20b6102eb94e05b62b701026fa6958b895739d3
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820391"
---
# <a name="use-the-microsoft-to-do-api"></a>Использование API Списка дел Microsoft

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте интерфейс API To Do Microsoft Graph, использующий [todoTask](todotask.md), для создания приложения, подключающегося к задачам в клиентах Microsoft To Do. Создавайте разнообразные возможности с задачами, например следующие:

* Создавайте задачи из рабочего процесса приложения, например из электронной почты или уведомлений, и сохраняйте их в To Do. Используйте объект [linkedResource](linkedresource.md), чтобы сохранить ссылку, ведущую к вашему приложению.
* Синхронизируйте существующие задачи приложения с помощью To Do и создайте единое представление задач, чтобы лучше определить приоритеты и управлять ими.
* Управляйте задачами To Do в пользовательском бизнес-приложении.

В настоящее время этот API поддерживает только разрешения, делегированные вошедшим пользователем.

Прежде чем приступить к работе с API To Do, ознакомьтесь с ресурсами и их связью между собой.

![Снимок экрана с выделенными объектами API Списка дел. Снимок экрана: перечень списков задач слева, задачи в определенном списке задач по центру и элементы контрольного списка и связанные ресурсы вместе с другими свойствами задач справа.](/graph/images/tasks-api-entities.png)

## <a name="task-list"></a>Список задач

В этом наборе API список задач представлен ресурсом [todoTaskList](./todotasklist.md), который является логическим контейнером ресурсов [todoTask](./todotask.md). В настоящее время вы можете создавать задачи только в списке задач. Чтобы [получить все свои списки задач](../api/todotasklist-get.md), выполните следующий HTTP-запрос:

``` http
GET /me/todo/lists
```

## <a name="task"></a>Задача

В этом наборе API задача представлена ресурсом [todoTask](./todotask.md): это работа или личный элемент, который можно отслеживать и выполнить. Чтобы получить свои задачи из списка задач, выполните следующий HTTP-запрос:
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
```

## <a name="checklist-item"></a>Элемент контрольного списка 

[ChecklistItem](checklistitem.md) представляет подзадачу в более крупном элементе [todoTask](./todotask.md). **ChecklistItem** позволяет разделить сложную задачу на более удобные задачи меньшего размера. Чтобы получить объект **checklistItem** из задачи, выполните следующий HTTP-запрос.
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems/{checklistItems}
```

## <a name="linked-resource"></a>Связанный ресурс

Объект [linkedResource](linkedresource.md) представляет любой элемент из партнерского приложения, связанный с задачей, например такой элемент, как письмо, из которого создана задача. Вы можете использовать его для хранения данных и связи с соответствующим элементом в приложении. Чтобы получить связанный ресурс из задачи, выполните следующий HTTP-запрос:
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/linkedresources/{linkedResourceId}
```

## <a name="track-changes-using-delta-query"></a>Отслеживание изменений с помощью разностного запроса

Для повышения производительности вы можете использовать локальный кэш объектов и периодически синхронизировать локальный кэш с сервером, используя [разностный запрос](/graph/delta-query-overview).

Разностный запрос поддерживают следующие ресурсы API To Do:
* Коллекция [todoTask](./todotask.md) в списке задач
* [todoTaskList](./todotasklist.md)

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

