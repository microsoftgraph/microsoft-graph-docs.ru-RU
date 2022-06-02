---
title: Использование API Microsoft To Do
description: API Microsoft Graph можно использовать для создания приложения, подключающегося к задачам в Microsoft To Do.
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: f5a1c64039f1ba2fd77913e76a1c18f4ff48927c
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821164"
---
# <a name="use-the-microsoft-to-do-api"></a>Использование API Microsoft To Do

Используйте API To Do Microsoft Graph для создания приложения, подключающегося к задачам в клиентах Microsoft To Do. Создавайте разнообразные возможности с задачами, например следующие:

* Создавайте задачи из рабочего процесса приложения, например из электронной почты или уведомлений, и сохраняйте их в To Do. Используйте объект [linkedResource](linkedresource.md), чтобы сохранить ссылку, ведущую к вашему приложению.
* Синхронизируйте существующие задачи приложения с помощью To Do и создайте единое представление задач, чтобы лучше определить приоритеты и управлять ими.
* Управляйте задачами To Do в пользовательском бизнес-приложении.

В настоящее время этот API поддерживает только разрешения, делегированные вошедшим пользователем.
 
Прежде чем приступить к работе с API To Do, ознакомьтесь с ресурсами и их связью между собой.

![Снимок экрана с выделенными объектами API Списка дел. Снимок экрана: перечень списков задач слева, задачи в определенном списке задач по центру и элементы контрольного списка и связанные ресурсы вместе с другими свойствами задач справа.](/graph/images/tasks-api-entities.png)

## <a name="task-list"></a>Список задач

Объект [todoTaskList](./todotasklist.md) представляет логический контейнер ресурсов [todoTask](./todotask.md). В настоящее время вы можете создавать задачи только в списке задач. Чтобы [получить все свои списки задач](../api/todotasklist-get.md), выполните следующий HTTP-запрос:

``` http
GET /me/todo/lists
```

## <a name="task"></a>Задача

Объект [todoTask](./todotask.md) представляет задачу, т. е. рабочий или личный элемент, который можно отследить и завершить. Чтобы получить свои задачи из списка задач, выполните следующий HTTP-запрос:
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

