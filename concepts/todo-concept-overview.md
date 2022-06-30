---
title: Обзор API To Do
description: Используйте Microsoft To Do API в Microsoft Graph, чтобы управлять задачами и планировать свой день. Задачи организованы в виде списков задач, доступных в клиентах To Do, Outlook и Teams.
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 30e4655ddcf4ff96b6cd3c82df80402c2f83d330
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556292"
---
# <a name="to-do-api-overview"></a>Обзор API To Do

Microsoft To Do API в Microsoft Graph предоставляет людям простой способ управлять своими задачами и планировать свой день. Задачи организованы в виде списков задач, к которым можно получить доступ через клиенты To Do, Outlook и Teams с любого устройства.

**Приложение To Do для Windows**

![Снимок экрана: приложение Microsoft To Do для Windows](./images/todo-windows-app.png "Изображение приложения Microsoft To Do для Windows")

## <a name="why-integrate-with-to-do"></a>Зачем нужна интеграция с To Do?

### <a name="ease-of-organizing-and-tracking-tasks"></a>Простота упорядочения и отслеживания задач
Microsoft To Do помогает создать список для любых задач, от рабочих заданий до домашних проектов и покупок. Вы можете отслеживать крайние сроки, добавляя напоминания, даты выполнения и заметки. Вы можете открыть свой список откуда угодно с помощью приложений Microsoft To Do для iOS, Android, Mac, Windows и Интернета. 

### <a name="integrate-across-microsoft-365"></a>Интеграция в Microsoft 365
Приложение To Do — единый центр для личных задач в Microsoft 365. Оно тесно интегрировано с центрами Microsoft 365, Outlook и Teams. Задачи, созданные в этих продуктах, синхронизируются с To Do, чтобы вы могли обращаться к ним и управлять ими на разных устройствах. Благодаря интеграции To Do вы можете связываться с миллионами пользователей, использующих To Do, для сбора задач из Outlook и Teams в едином объединенном представлении.  

### <a name="support-task-completion-using-linked-resources"></a>Поддержка выполнения задач с помощью связанных ресурсов
Microsoft To Do предоставляет новый объект под названием _связанный ресурс_. Вы можете использовать его для создания задач, которые могут быть связаны со своими исходными источниками. Это позволяет легко интегрировать To Do в свой рабочий процесс, создавая задачи, связанные с вашим продуктом или службой. 

## <a name="common-to-do-api-operations"></a>Распространенные операции API To Do

|Операция|Запрос|
|:--------|:--|
| Перечисление всех списков задач | GET https://graph.microsoft.com/v1.0/me/todo/lists |
| Перечисление всех задач в списке задач | GET https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks |
| Создание задачи | POST https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks |
| Обновление задачи | PATCH https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId} |
| Удаление задачи | DELETE https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId} |

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [API To Do в Microsoft Graph v1.0](/graph/api/resources/todo-overview?view=graph-rest-1.0&preserve-view=true)
- [To Do API в бета-версии Microsoft Graph](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true)
