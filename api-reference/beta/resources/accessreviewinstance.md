---
title: Тип ресурса accessReviewInstance
description: Представляет повторение объекта `accessReviewScheduleDefinition`.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5dece4ad638758a51e8aa839cbb755ec5b79d6fd
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697227"
---
# <a name="accessreviewinstance-resource-type"></a>Тип ресурса accessReviewInstance

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет Azure AD [проверки](accessreviewsv2-overview.md) доступа. Если родительский [объект accessReviewScheduleDefinition](accessreviewscheduledefinition.md) является повторяющейся проверкой доступа, экземпляры представляют каждое повторение. Повторная проверка будет иметь только один экземпляр. Экземпляры также представляют каждую уникальную группу, проверяемую в определении расписания. Если определение расписания проверяет несколько групп, каждая группа будет иметь уникальный экземпляр для каждого повторения.

**Каждый объект accessReviewInstance** содержит список решений [,](accessreviewinstancedecisionitem.md) с помощью которых рецензенты могут принять меры. Для каждого проверяемого удостоверения принимается одно решение.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Перечисление объектов accessReviewInstance](../api/accessreviewscheduledefinition-list-instances.md) | [Коллекция accessReviewInstance](accessreviewinstance.md) | Получение списка объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств. |
|[Получение accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Чтение свойств и связей объекта [accessReviewInstance](../resources/accessreviewinstance.md) . |
|[Обновление accessReviewInstance](../api/accessreviewinstance-update.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Обновление рецензентов объекта [accessReviewInstance](../resources/accessreviewinstance.md) .|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[Коллекция accessReviewInstance](../resources/accessreviewinstance.md)|Возвращает все экземпляры в заданном [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) , для которого вызывающий пользователь является рецензентом одного или нескольких решений.|
|[Перечисление контактных рецензентов](../api/accessreviewinstance-list-contactedreviewers.md)|[Коллекция accessReviewReviewer](../resources/accessreviewreviewer.md)|Получение рецензентов, которые получили уведомления для экземпляра проверки доступа.|
|[sendReminder](../api/accessreviewinstance-sendreminder.md) | Нет. | Отправьте напоминание рецензентам accessReviewInstance. |
|[stop](../api/accessreviewinstance-stop.md) | Нет. | Вручную остановите accessReviewInstance. |
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md) | Нет. | Позволяет вызывающему пользователю принять рекомендацию по принятию решения для каждого объекта NotReviewInstanceDecisionItem, в котором он является рецензентом для определенного объекта accessReviewInstance. |
|[applyDecisions](../api/accessreviewinstance-applydecisions.md) | Нет. | Вручную примените решения к accessReviewInstance. |
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Отсутствует|Просмотрите пакеты субъектов или ресурсов за один вызов.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Отсутствует|Сбрасывает все элементы принятия решений в экземпляре в значение `notReviewed`.|
|[Этапы списка](../api/accessreviewinstance-list-stages.md)|[Коллекция accessReviewStage](../resources/accessreviewstage.md)| Получение этапов в экземпляре многоэтабной проверки доступа.|
|[Список решений](../api/accessreviewinstance-list-decisions.md)|[Коллекция accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Получите ресурсы accessReviewInstanceDecisionItem из свойства навигации решений.|
|[Перечисление pendingAccessReviewInstances (не рекомендуется)](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [коллекция accessReviewInstance](accessreviewinstance.md) . | Получение всех ожидающих ресурсов accessReviewInstance, назначенных вызывающему пользователю. Этот метод является устаревшим и заменяется [filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md). |

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------------------------------- | :---------- |
| endDateTime | DateTimeOffset | DateTime при запланированном завершении экземпляра проверки. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда используется во время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$select`. Только для чтения.|
| ошибки | [Коллекция accessReviewError](accessreviewerror.md)| Коллекция ошибок в жизненном цикле экземпляра проверки доступа. Только для чтения. |
| fallbackReviewers   |[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Эта коллекция областей рецензента используется для определения списка резервных рецензентов. Эти резервные рецензенты будут получать уведомления о том, что нужно принять меры, если пользователи не найдены в указанном списке рецензентов. Это может произойти, если владелец группы указан в качестве рецензента, но владелец группы не существует, или руководитель указан в качестве рецензента, но руководитель пользователя не существует. Поддерживает `$select`.|
| id | String | Уникальный идентификатор экземпляра. Поддерживает `$select`. Только для чтения.|
| scope | [accessReviewScope](accessreviewscope.md) | Создается на **основе области** и **экземпляраEnumerationScope** на уровне accessReviewScheduleDefinition. Определяет область пользователей, проверяемых в группе. Поддерживает и `$select` `$filter` (`contains` только). Только для чтения. |
| startDateTime | DateTimeOffset | DateTime при запланированном запуске экземпляра проверки. Может быть в будущем. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$select`. Только для чтения. |
| status | String | Указывает состояние accessReview. Возможные значения: `Initializing`, `NotStarted`, `Starting`, , `InProgress`, `Completing`, `Completed`, и `AutoReviewed``AutoReviewing`. Поддерживает , `$select``$orderby`и `$filter` (`eq`только). Только для чтения.|
| Авторам   |[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Эта коллекция областей проверки доступа используется для определения рецензентов. Поддерживает `$select`. Примеры параметров назначения рецензентов см. в статье "Назначение рецензентов определению проверки доступа с [помощью microsoft API Graph"](/graph/accessreviews-scope-concept).|


## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| contactedReviewers   |[Коллекция accessReviewReviewer](../resources/accessreviewreviewer.md)| Возвращает коллекцию рецензентов, с которыми связывались для завершения этой проверки. Хотя рецензенты  и **свойства fallbackReviewers** **объекта accessReviewScheduleDefinition** могут указывать владельцев групп или руководителей в качестве рецензентов **,** **contactedReviewers** возвращает свои отдельные удостоверения. Поддерживает `$select`. Только для чтения. |
| Определение               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | С каждым экземпляром связан только один **accessReviewScheduleDefinition** . Это родительское расписание для экземпляра, где экземпляры создаются для каждого повторения определения проверки и каждой группы, выбранной для проверки определением. |
|stages|[Коллекция accessReviewStage](accessreviewstage.md)| Если экземпляр имеет несколько этапов, возвращается коллекция этапов. Новый этап будет создан только после завершения предыдущего этапа. Существование, число и параметры этапов в экземпляре проверки создаются на основе [accessReviewStageSettings](accessreviewstagesettings.md) в родительском [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). |
| Решения               |[Коллекция accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)        | Каждый пользователь, проверяемый в **accessReviewInstance** , имеет элемент принятия решения, который указывает, утверждены ли они, отклонены или еще не просмотрели. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "openType": false
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstance",
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
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
  ],
  "contactedReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewer"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
