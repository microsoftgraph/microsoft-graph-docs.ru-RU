---
title: Тип ресурса accessReviewInstance
description: Представляет повторение объекта accessReviewScheduleDefinition.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5fe495a689a27f5d7dcd76f9148e51185339bdbe
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698312"
---
# <a name="accessreviewinstance-resource-type"></a>Тип ресурса accessReviewInstance

Пространство имен: microsoft.graph

Представляет Azure AD [проверки](accessreviewsv2-overview.md) доступа. Созданное системой на основе родительского [объекта accessReviewScheduleDefinition](accessreviewscheduledefinition.md) . Все свойства доступны только для чтения.

Если экземпляр является частью повторяющейся проверки доступа, экземпляры представляют каждое повторение. Повторная проверка будет иметь только один экземпляр. Экземпляры также представляют каждый уникальный ресурс, проверяемый в определении расписания. Если определение расписания проверяет несколько ресурсов, каждый ресурс будет иметь уникальный экземпляр для каждого повторения.

**Каждый объект accessReviewInstance** содержит список решений [,](accessreviewinstancedecisionitem.md) с помощью которых рецензенты могут принять меры. Для каждого проверяемого удостоверения принимается одно решение.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов accessReviewInstance](../api/accessreviewscheduledefinition-list-instances.md)|[Коллекция accessReviewInstance](../resources/accessreviewinstance.md)|Получение списка объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств.|
|[Получение accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Чтение свойств и связей объекта [accessReviewInstance](../resources/accessreviewinstance.md) .|
|[Обновление accessReviewInstance](../api/accessreviewinstance-update.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Обновление рецензентов объекта [accessReviewInstance](../resources/accessreviewinstance.md) .|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[Коллекция accessReviewInstance](../resources/accessreviewinstance.md)|Возвращает все объекты экземпляра в определении, для которого вызывающий пользователь является рецензентом.|
|[Перечисление контактных рецензентов](../api/accessreviewinstance-list-contactedreviewers.md)|[Коллекция accessReviewReviewer](../resources/accessreviewreviewer.md)|Получение рецензентов, которые получили уведомления для экземпляра проверки доступа.|
|[sendReminder](../api/accessreviewinstance-sendreminder.md)|Отсутствует|Отправьте напоминание рецензентам accessReviewInstance.|
|[stop](../api/accessreviewinstance-stop.md)|Отсутствует|Вручную остановите accessReviewInstance.|
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|Отсутствует| Позволяет вызывающему пользователю принять рекомендацию по принятию решения для каждого объекта NotReviewInstanceDecisionItem, в котором он является рецензентом для определенного объекта accessReviewInstance.|
|[applyDecisions](../api/accessreviewinstance-applydecisions.md)|Нет|Вручную примените решение к accessReviewInstance.|
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Отсутствует|Просмотрите пакеты субъектов или ресурсов за один вызов.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Отсутствует|Сбрасывает все элементы принятия решений в экземпляре на `notReviewed`|
|[Список решений](../api/accessreviewinstance-list-decisions.md)|[Коллекция accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Получите ресурсы accessReviewInstanceDecisionItem из свойства навигации решений.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| endDateTime | DateTimeOffset | DateTime при запланированном завершении экземпляра проверки. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда используется во время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$select`. Только для чтения.|
| fallbackReviewers   |[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Эта коллекция областей рецензента используется для определения списка резервных рецензентов. Эти резервные рецензенты будут получать уведомления о том, что нужно принять меры, если пользователи не найдены в указанном списке рецензентов. Это может произойти, если владелец группы указан в качестве рецензента, но владелец группы не существует, или руководитель указан в качестве рецензента, но руководитель пользователя не существует. Поддерживает `$select`.|
| id | String | Уникальный идентификатор экземпляра. Наследуется от [сущности](../resources/entity.md). Поддерживает `$select`. Только для чтения.|
| scope | [accessReviewScope](accessreviewscope.md) | Создается на **основе области** и **экземпляраEnumerationScope** на уровне accessReviewScheduleDefinition. Определяет область пользователей, проверяемых в группе. Поддерживает и `$select` `$filter` (`contains` только). Только для чтения. |
| startDateTime | DateTimeOffset | DateTime при запланированном запуске экземпляра проверки. Может быть в будущем. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$select`. Только для чтения. |
| status | String | Указывает состояние accessReview. Возможные значения: `Initializing`, `NotStarted`, `Starting`, , `InProgress`, `Completing`, `Completed`, и `AutoReviewed``AutoReviewing`. Поддерживает , `$select``$orderby`и `$filter` (`eq`только). Только для чтения.|
| Авторам   |[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Эта коллекция областей проверки доступа используется для определения рецензентов. Поддерживает `$select`. Примеры параметров назначения рецензентов см. в статье "Назначение рецензентов определению проверки доступа с [помощью microsoft API Graph"](/graph/accessreviews-scope-concept).|


## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|Решения|[Коллекция accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|У каждого участника, проверяемого в **accessReviewInstance** , есть элемент принятия решения, который указывает, утверждены ли они, отклонены или еще не просмотрелись.|
| contactedReviewers   |[Коллекция accessReviewReviewer](../resources/accessreviewreviewer.md)| Возвращает коллекцию рецензентов, с которыми связывались для завершения этой проверки. Хотя рецензенты  и **свойства fallbackReviewers** **объекта accessReviewScheduleDefinition** могут указывать владельцев групп или руководителей в качестве рецензентов **,** **contactedReviewers** возвращает свои отдельные удостоверения. Поддерживает `$select`. Только для чтения. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstance",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "status": "String",
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```
