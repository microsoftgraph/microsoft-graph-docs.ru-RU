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
# <a name="use-the-microsoft-to-do-api"></a>Использование API Microsoft To Do

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте API To Do Microsoft Graph для создания приложения, подключающегося к задачам в клиентах Microsoft To Do. Создавайте разнообразные возможности с задачами, например следующие:

* Создавайте задачи из рабочего процесса приложения, например из электронной почты или уведомлений, и сохраняйте их в To Do. Используйте объект [linkedResource](linkedresource.md), чтобы сохранить ссылку, ведущую к вашему приложению.
* Синхронизируйте существующие задачи приложения с помощью To Do и создайте единое представление задач, чтобы лучше определить приоритеты и управлять ими.
* Управляйте задачами To Do в пользовательском бизнес-приложении.

В настоящее время этот API поддерживает только разрешения, делегированные вошедшим пользователем.
 
Прежде чем приступить к работе с API To Do, ознакомьтесь с ресурсами и их связью между собой.

![Объекты API To Do](/graph/images/todo-api-entities.png)

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

