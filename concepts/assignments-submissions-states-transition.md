---
title: Состояния, переходы и ограничения для назначений и представлений в Microsoft Graph
description: В этой статье описываются изменения в состояниях назначения и отправки во время процесса и какие API образования в Microsoft Graph вовлечены.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 97e75c7ef87d47c0359d6b8d6a5e5db2bb21a518
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647009"
---
# <a name="states-transitions-and-limitations-for-assignments-and-submissions-in-microsoft-graph"></a>Состояния, переходы и ограничения для назначений и представлений в Microsoft Graph

Назначения и отправки являются важной частью взаимодействия между преподавателями и действиями учащихся. В этой статье описываются изменения в состояниях назначения и отправки во время процесса и какие API образования в Microsoft Graph вовлечены.

## <a name="assignment-states-and-transitions"></a>Состояния назначения и переходы

Назначение представляет собой задачу или единицу работы, назначенную учащемуся или членам группы в классе в рамках своего обучения. Только преподаватели или владельцы команд могут создавать, копировать или планировать назначения. Эти действия влияют на состояния назначения. В следующей таблице перечислены состояния назначения и API, доступные для изменения состояния. 

| Состояние | Описание | Вызов API REST |
|:--|:--|:--|
| Draft | Начальный статус, когда новое назначение создается или копируется из существующего назначения. | `POST /education/classes/{id}/assignments` |
| Published | Состояние фоновой обработки при распределении назначения каждому назначенного учащемуся. | `POST /education/classes/{id}/assignments/{id}/publish` |
| Scheduled | Состояние, когда учитель заплановал публикацию задания в будущем. | `PATCH /education/classes/{id}/assignments/{id}`<br/>`POST /education/classes/{id}/assignments/{id}/publish` |
| Назначенное | После завершения публикации назначение перемещается в назначенное состояние и доступно для учащихся. | `POST /education/classes/{id}/assignments/{id}/publish` |
| Pending | Состояние фоновой обработки при копировании нового назначения из существующего. | `POST /education/classes/{id}/assignments/{id}/copy`<br/>`PATCH /education/classes/{id}/assignments/{id}` |

На следующей схеме показаны переходы состояния, которые могут происходить для назначений.

![Схема переходов состояния назначения](images/states-transitions/diagram-assignments.PNG)

### <a name="how-to-verify-that-an-assignment-is-published"></a>Проверка публикации назначения
Вызывающий должен использовать операцию [назначения GET](/graph/api/educationassignment-get.md) для проверки текущего состояния назначения и проверки успешного процесса публикации.

### <a name="assignments-states-transitions-based-on-the-allowed-actions"></a>Назначения состояния переходов на основе разрешенных действий
| Текущее состояние назначения | Действие | Новое состояние |
|:--|:--|:--|
| Draft | Учитель запланировать назначение | Scheduled |
| Draft | Публикация | Published |
| Draft | Отредактирован | Draft |
| Draft | Отбрасывается | | 
| Published | Публикация завершена | Назначенное |
| Published | Отбрасывается | |
| Scheduled | Дата достижения срока | Published |
| Scheduled | Отмена расписания | Draft |
| Scheduled | Перенос | Scheduled |
| Назначенное | Отбрасывается | |
| Pending | Завершено копирование | Draft |
| Pending | Отбрасывается | |   

`Note: Any action and state transition not listed in the table is NOT allowed`

### <a name="sync-vs-async-operations-over-assignments-api-calls"></a>Синхронизация операций и операций async по вызовам API назначений
В следующей таблице упоминаются вызовы API, влияющие на состояние назначения и тип операции.

Синхронные операции выполняются по одному, и только после завершения одной операции можно запустить следующую операцию, и результат возвращается до завершения последней операции. При асинхронных операциях операция начинается, а другая операция может быть завершена до завершения предыдущей. Асинхронная операция выполняет некоторые фоновые действия, и для получения результата вызывающий должен проводить опрос.

| API | Синхронизация или async | Механизм получения последнего состояния |
|:--|:--|:--|
| `DELETE /education/classes/{id}/assignments/{id}` | Async | Опрос |
| `POST /education/classes/{id}/assignments/{id}/publish` | Async | Опрос |
| `PATCH /education/classes/{id}/assignments/{id}` | Async | Опрос |
| `POST /education/classes/{id}/assignments` | Async | Опрос |

## <a name="submission-states-and-transitions"></a>Состояния отправки и переходы

Отправка представляет ресурсы, которые человек (или группа) получает для назначения. Отправки принадлежат назначению и создаются автоматически при публикации назначения.

Состояние является свойством только для чтения в представлении и изменяется в зависимости от действий учащихся и преподавателей.
 

| Состояние | Описание | Вызов API REST |
|:--|:--|:--|
| Выполняется | Начальное состояние после создания отправки. | `POST /education/classes/{id}/assignments`<br/>`POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` |
| Submitted | Это происходит после того, как учащийся включит задание. | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` |
| Возвращено | После того как учитель возвращает задание ученику. | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` |
| Повторное присвоение | После того как учитель вернул задание учащемуся для пересмотра. | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/reassign` |

На следующей схеме показан поток перехода состояния.

![Схема переходов состояния отправки](images/states-transitions/diagram-submissions.PNG)

### <a name="submissions-states-transitions-based-on-allowed-actions"></a>Переходы состояния представлений на основе разрешенных действий
| Текущее состояние отправки | Действие | Новое состояние |
|:--|:--|:--|
| Выполняется | Включаем | Submitted |
| Выполняется | Возвращение для пересмотра | Повторное присвоение |
| Выполняется | Возврат | Возвращено |
| Submitted | Отмена включаемой | Выполняется |
| Submitted | Возврат | Возвращено |
| Submitted | Возвращение для пересмотра | Повторное присвоение |
| Возвращено | Включаем | Submitted |
| Возвращено | Возврат | Возвращено |
| Возвращено | Возвращение для пересмотра | Повторное присвоение |
| Повторное присвоение | Включаем | Submitted |
| Повторное присвоение | Возврат | Возвращено |
| Повторное присвоение | Возвращение для пересмотра | Повторное присвоение |

`Note: Any action and state transition not listed in the table is NOT allowed`

### <a name="sync-vs-async-operations-over-submissions-api-calls"></a>Синхронизация операций с async над вызовами API отправки
В следующей таблице перечислены вызовы API, влияющие на состояние отправки и тип операции.

В этом случае все вызовы являются асинхронными, что означает, что операция начинается, а еще одна операция может начаться до завершения первой. Асинхронная операция выполняет некоторые фоновые действия, и для получения результата вызывающий должен проводить опрос.  

| API | Синхронизация или async | Механизм получения последнего состояния |
|:--|:--|:--|
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` | Async | Опрос |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` | Async | Опрос |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` | Async | Опрос |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/reassign` | Async | Опрос |

### <a name="limits"></a>Ограничения
Для всех вызовов API применяются следующие ограничения:

* Максимальное количество назначений и ресурсов отправки — 10 для преподавателя и плюс 10 для учащегося.
* Максимальный допустимый размер ресурсов — 50 МБ в целом или 10 ресурсов.
* Применяются ограничения регулирования; подробные сведения см. в Graph руководства по [регулированием.](https://docs.microsoft.com/graph/throttling)
