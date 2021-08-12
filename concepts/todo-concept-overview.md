---
title: Обзор API To Do
description: Приложение To Do предоставляет простой способ управления задачами и планирования дня
author: avijityadav
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 0d93ba100fb48d2c6e833582a7f8238a5e51800e6b92d56ed4707e2aad2d8499
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54245401"
---
# <a name="to-do-api-overview"></a>Обзор API To Do
Приложение Microsoft To Do предоставляет пользователям простой способ управления задачами и планирования дня. Задачи упорядочиваются в списках задач, доступных в клиентах To Do, Outlook и Teams с любого устройства.

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

- [API To Do в Microsoft Graph](/graph/api/resources/todo-overview)
