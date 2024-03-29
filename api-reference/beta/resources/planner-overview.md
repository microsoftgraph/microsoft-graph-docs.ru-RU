---
title: Использование REST API Планировщика
description: API Планировщика в Microsoft Graph можно использовать для создания задач и назначения их пользователям в группе Microsoft 365.
author: TarkanSevilmis
ms.localizationpriority: high
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: 75ba0d53b4e83df5dd8f9faad2501d5dbbaa94f1
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420735"
---
# <a name="use-the-planner-rest-api"></a>Использование REST API Планировщика

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

API Планировщика в Microsoft Graph можно использовать для создания задач и назначения их пользователям в группе Microsoft 365.

Перед началом работы с API Планировщика изучите, как основные объекты связаны друг с другом и группами Microsoft 365.

## <a name="plan-containers"></a>Контейнеры плана
В Планировщике (Майкрософт) планы всегда содержатся в другом ресурсе. Содержащий их ресурс определяет правила авторизации плана и все задачи в нем, а также жизненный цикл плана. Например, для планов, содержащихся в группах Microsoft 365, участники группы смогут создавать, изменять, разрешать и удалять задачи в плане, а также изменять некоторые свойства на уровне плана, такие как имя плана и названия меток. Кроме того, при удалении группы автоматически удаляются все планы из нее, а если группа восстанавливается, все планы будут автоматически восстановлены.

Самый распространенный тип контейнера — группа Microsoft 365.

### <a name="container-type-microsoft-365-groups"></a>Тип контейнера: группы Microsoft 365

Планы обычно содержатся в группах Microsoft 365 в API Планировщика.
Чтобы [получить планы, принадлежащие группе](../api/plannergroup-list-plans.md), выполните HTTP-запрос, описанный ниже.

``` http
GET /groups/{group-id}/planner/plans
```

При [создании плана](../api/planner-post-plans.md) настройте свойство **container** объекта плана, чтобы сделать группу его контейнером. Планы должны содержаться в поддерживаемом ресурсе.

>**Примечание.** Пользователь, создающий план, должен быть участником группы, в которой будет содержаться план. При создании группы с помощью средства [создания группы](../api/group-post-groups.md) вы не становитесь ее участником. После создания группы добавьте себя в качестве участника с помощью операции [добавления участников группы](../api/group-post-members.md).

## <a name="plans"></a>Планы

[Планы](plannerplan.md) представляют собой контейнеры [задач](plannertask.md).
Чтобы [создать задачу в плане](../api/planner-post-tasks.md), при ее создании укажите идентификатор плана в качестве свойства **planId** объекта задачи.
В настоящее время невозможно создавать задачи без планов.
Чтобы [получить задачи в плане](../api/plannerplan-list-tasks.md), выполните HTTP-запрос, описанный ниже.

``` http
GET /planner/plans/{plan-id}/tasks
```

## <a name="tasks"></a>Задачи

Задачу можно назначить пользователю, добавив [назначение](plannerassignment.md) в свойстве [assignments](plannerassignments.md) объекта задачи. Идентификатор исполнителя задачи — это имя открытого свойства в **assignments**. Необходимо также указать свойство **orderHint** назначения.

## <a name="task-and-plan-details"></a>Данные задач и плана

Ресурсы Планировщика делятся на базовые объекты и объекты сведений. Базовые объекты предоставляют доступ к основным свойствам ресурсов, подходящим для списков, а объекты сведений обеспечивают доступ к большим свойствам ресурсов, которые подходят для развернутых представлений.

## <a name="visualization"></a>Визуализация

Помимо данных задач и плана, API Планировщика предоставляет ресурсы для создания общей визуализации данных по клиентам. Для задач доступны несколько типов визуализации данных, как представлено в таблице ниже.

| Способ представления задач                                                                        | Источник информации для упорядочивания задач                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| Простой список (задачи в плане)                                                               | Свойство **orderHint** задач                                                   |
| Простой список (задачи, назначенные пользователю)                                                      | Свойство **assigneePriority** задач                                            |
| Доска со столбцами для исполнителей (доска задач "Кому назначено")                            | Объект [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |
| Доска со столбцами для хода выполнения задачи (доска задач "Ход выполнения") | Объект [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)     |
| Доска с настраиваемыми столбцами задач (доска задач "Сегменты"):                              | Объект [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)         |

Настраиваемые столбцы на доске задач "Сегменты" представлены объектами [bucket](plannerbucket.md), а их порядок — свойством **orderHint** объекта.

Принципы упорядочивания описаны в статье [Использование указаний по упорядочиванию в Планировщике](planner-order-hint-format.md).

## <a name=""></a><a name="delta">Отслеживание изменений с помощью запроса изменений</a>

Запрос изменений Планировщика поддерживает запрос объектов, на которые подписан пользователь.

Пользователи подписаны на указанные ниже объекты.

| Тип ресурса Планировщика | Экземпляры подписки                                                                                                                                                                                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **задачи**                 | <ul><li>Созданные пользователем</li><li>Назначенные пользователю</li><li>Относящиеся к плану, принадлежащему пользователю</li><li>Содержащиеся в плане, предоставленном пользователю для совместного использования посредством коллекции **sharedWith** плана</li> |
| **планы**                 | <ul><li>Предоставленные пользователю для совместного использования посредством коллекции **sharedWith** плана</li></ul>                                                                                                                     |
| **сегменты**               | <ul><li>Содержащиеся в плане, предоставленном пользователю для совместного использования посредством коллекции **sharedWith** плана</li></ul>                                                                                                 |

### <a name=""></a><a name="objectcache">Заполнение кэша объекта для запросов изменений</a>

Если нужно использовать API запроса изменений Планировщика, сохраните локальный кэш объектов, которые хочет просмотреть пользователь, чтобы применить изменения из канала запроса изменений.

Ниже указаны типы объектов полезных данных изменений, которые могут в настоящее время возвращаться запросом изменений Планировщика.

* [plannerTask](plannertask.md);
* [plannerTaskDetails](plannertaskdetails.md);
* [plannerPlan](plannerplan.md)
* [plannerPlanDetails](plannerplandetails.md);
* [plannerBucket](plannerbucket.md);
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md);
* [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md).

Чтобы получить исходное состояние объектов для заполнения локального кэша, используйте соответствующе методы `GET`.

### <a name="differentiating-between-object-creation-and-object-modification"></a>Различие между созданием и изменением объекта

В некоторых случаях вызывающему объекту может потребоваться отличить создание объекта от изменения объекта в канале запроса изменений Планировщика.

Приведенные ниже инструкции можно использовать для определения создания объекта:

* Свойство **createdBy** отображается только для новых объектов.
* За новым объектом **plannerTask** следует соответствующий ему объект **plannerTaskDetails**.
* За новым объектом **plannerPlan** следует соответствующий ему объект **plannerPlanDetails**.

### <a name="usage"></a>Применение

Ожидается, что у вызывающего объекта есть кэш, содержащий объекты подписки. Сведения о заполнении локального кэша объектов подписки см. в статье [Заполнение кэша объектов для запросов изменений](#populate-the-object-cache-for-delta-queries).

Поток вызова запроса изменений Планировщика выглядит указанным ниже образом.

1. Вызывающий объект запускает запрос синхронизации изменений, получая `nextLink` и пустую коллекцию изменений.
2. Вызывающий объект должен [заполнить кэш объектов для запросов изменений](#populate-the-object-cache-for-delta-queries) объектами, на которые подписан пользователь, обновив их кэш.
3. Вызывающий объект переходит по ссылке `nextLink`, предоставленной в исходном запросе синхронизации изменений, чтобы получить новую ссылку `deltaLink` для любых изменений с предыдущего этапа.
4. Вызывающий объект применяет изменения в возвращенном отклике изменений к объектам в кэше.
5. Вызывающий объект переходит по новой ссылке `deltaLink`, чтобы получить следующую ссылку `deltaLink` и изменения с момента создания текущей ссылки `deltaLink`.
6. Вызывающий объект применяет изменения (при наличии) и ожидает некоторое время, прежде чем перезапустить предыдущий и текущий шаг.

## <a name="planner-resource-versioning"></a>Версии ресурсов в Планировщике

Планировщик управляет версиями ресурсов с помощью тегов etag. Эти теги etag возвращаются со свойством **@odata.etag** для каждого ресурса. Для запросов `PATCH` и `DELETE` требуется последний тег etag, известный клиенту, чтобы указать его в заголовке `If-Match`.
Планировщик позволяет изменять старые версии ресурсов, если планируемое изменение не конфликтует с более новыми изменениями, принятыми службой Планировщика в том же ресурсе. Клиенты могут определить, какой тег etag ресурса новее, вычислив большее значение тега etag при сравнении порядкового номера строки.
У каждого ресурса есть уникальный тег etag. Невозможно сравнить значения тегов etag для разных ресурсов, в том числе с отношениями вложения.
Клиентские приложения должны обрабатывать [коды ошибок](/graph/errors) `409` и `412`, связанные с версиями, считывая последнюю версию элемента и устраняя конфликтующие изменения.

## <a name="common-planner-error-conditions"></a>Основные ошибки Планировщика

В дополнение к [общим ошибкам](/graph/errors) Microsoft Graph, некоторые ошибки относятся только к API Планировщика.

### <a name="400-bad-request"></a>400 (неправильный запрос)

В некоторых типовых сценариях на запросы `POST` и `PATCH` может быть получен код состояния 400. Ниже приведено несколько распространенных причин.

* Свойства Open Type имеют неправильный тип, тип не указан, или они не содержат свойств. Например, свойства [plannerAssignments](plannerassignments.md) со сложными значениями должны объявлять свойство **@odata.type** со значением `microsoft.graph.plannerAssignment`.
* Указания по упорядочиванию имеют неправильный формат. Например, в качестве указания по упорядочиванию задается значение, возвращаемое клиенту.
* Данные логически не согласованы. Например, дата начала задачи позже даты выполнения задачи.

### <a name="403-forbidden"></a>403 (доступ запрещен)

Помимо общих ошибок, API Планировщика возвращает код состояния `403`, если превышено ограничение, определенное в службе. Тип ограничения, превышенного в запросе, будет указан в свойстве **code** типа ресурса с ошибкой.
Ниже перечислены возможные значения для типов ограничений.

| Значение                         | Описание                                                                                                                                                                                              |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MaximumProjectsOwnedByUser    | Превышено максимальное количество планов, содержащихся в группе. Это ограничение применяется к планам, содержащимся в группе, на основе свойства **container** ресурса [plannerPlan](plannerplan.md).                                         |
| MaximumProjectsSharedWithUser | Превышено максимальное количество планов, к которому пользователю предоставляется общий доступ. Это ограничение основано на свойстве **sharedWith** ресурса [plannerPlanDetails](plannerplandetails.md).                   |
| MaximumTasksCreatedByUser     | Превышено максимальное количество задач, создаваемых пользователем. Это ограничение основано на свойстве **createdBy** ресурса [plannerTask](plannertask.md).                                    |
| MaximumTasksAssignedToUser    | Превышено максимальное количество задач, назначаемых пользователю. Это ограничение основано на свойстве **assignments** ресурса [plannerTask](plannertask.md).                                 |
| MaximumTasksInProject         | Превышено максимальное количество задач в плане. Это ограничение основано на свойстве **planId** ресурса [plannerTask](plannertask.md).                                               |
| MaximumActiveTasksInProject   | Превышено максимальное количество невыполненных задач в плане. Это ограничение основано на свойствах **planId** и **percentComplete** ресурса [plannerTask](plannertask.md). |
| MaximumBucketsInProject       | Превышено максимальное количество сегментов в плане. Это ограничение основано на свойстве **planId** ресурса [plannerBucket](plannerbucket.md).                                         |
| MaximumUsersSharedWithProject | Свойство **sharedWith** ресурса [plannerPlanDetails](plannerplandetails.md) содержит слишком много значений.                                                                                          |
| MaximumReferencesOnTask       | Свойство **references** ресурса [plannerTaskDetails](plannertaskdetails.md) содержит слишком много значений.                                                                                          |
| MaximumChecklistItemsOnTask   | Свойство **checklist** ресурса [plannerTaskDetails](plannertaskdetails.md) содержит слишком много значений.                                                                                           |
| MaximumAssigneesInTasks       | Свойство **assignments** ресурса [plannerTask](plannertask.md) содержит слишком много значений.                                                                                                       |
| MaximumFavoritePlansForUser   | Свойство **favoritePlanReferences** ресурса [plannerUser](planneruser.md) содержит слишком много значений.                                                                                            |
| MaximumRecentPlansForUser     | Свойство **recentPlanReferences** ресурса [plannerUser](planneruser.md) содержит слишком много значений.                                                                                              |
| MaximumContextsOnPlan         | Свойство **contexts** ресурса [plannerPlan](plannerplan.md) содержит слишком много значений.                                                                                                          |
| MaximumPlannerPlans       | Группа уже содержит **план**. В настоящее время группы могут содержать только один **план**. **Примечание.** Некоторые приложения Майкрософт могут превышать это ограничение. В будущем эта возможность будет реализована для всех приложений.                                                                                                      |

### <a name="412-precondition-failed"></a>412 (необходимое условие не выполнено)

Во всех запросах `POST`, `PATCH` и `DELETE` API Планировщика заголовок `If-Match` необходимо указывать с последним известным значением тега etag ресурса.
Код состояния 412 также может быть возвращен, если значение тега etag, указанное в запросе, больше не соответствует версии ресурса в службе. В этом случае клиентам следует прочитать ресурс еще раз и получить новый тег etag.

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

