---
title: тип ресурсов accessReviewInstance
description: Представляет собой повторение .`accessReviewScheduleDefinition`
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 68863a90e4b059a22525c6f8342c32fb513a2e7c
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "62815981"
---
# <a name="accessreviewinstance-resource-type"></a>тип ресурсов accessReviewInstance

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет повторение проверки доступа Azure [AD.](accessreviewsv2-overview.md) Если родительский [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) является повторяемой проверкой доступа, экземпляры представляют каждое повторение. Обзор, который не повторяется, будет иметь точно один экземпляр. Экземпляры также представляют каждую уникальную группу, проверяемую в определении расписания. Если определение расписания проверяет несколько групп, каждая группа будет иметь уникальный экземпляр для каждого повторения.

**Каждый accessReviewInstance содержит** список решений [,](accessreviewinstancedecisionitem.md) которые могут приниматься рецензентами. Существует одно решение для каждого проверяемого удостоверения.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Список accessReviewInstances](../api/accessreviewscheduledefinition-list-instances.md) | [accessReviewInstance](accessreviewinstance.md) collection | Получите список объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств. |
|[Получить accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstance](../resources/accessreviewinstance.md) . |
|[Обновление accessReviewInstance](../api/accessreviewinstance-update.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Обновление рецензентов объекта [accessReviewInstance](../resources/accessreviewinstance.md) .|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) collection|Возвращает все экземпляры в данном [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) , для которого вызываемая пользователь является рецензентом одного или более решений.|
|[Список контактных рецензентов](../api/accessreviewinstance-list-contactedreviewers.md)|[коллекция accessReviewReviewer](../resources/accessreviewreviewer.md)|Получите рецензентов, которые получили уведомления для экземпляра проверки доступа.|
|[sendReminder](../api/accessreviewinstance-sendreminder.md) | Нет. | Отправьте напоминание рецензентам accessReviewInstance. |
|[stop](../api/accessreviewinstance-stop.md) | Нет. | Вручную остановите accessReviewInstance. |
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md) | Нет. | Позволяет вызываемой пользователю принять рекомендацию по принятию решений для каждого notReviewed accessReviewInstanceDecisionItem, на которых он является рецензентом для определенного accessReviewInstance. |
|[applyDecisions](../api/accessreviewinstance-applydecisions.md) | Нет. | Вручную применять решения для accessReviewInstance. |
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Нет|Просмотр пакетов принципов или ресурсов в одном вызове.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Нет|Сброс всех элементов решений в экземпляре в `notReviewed`.|
|[Этапы списка](../api/accessreviewinstance-list-stages.md)|[коллекция accessReviewStage](../resources/accessreviewstage.md)| Извлечение этапов в экземпляре проверки многоступенчатого доступа.|
|[Список решений](../api/accessreviewinstance-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Получите ресурсы accessReviewInstanceDecisionItem из свойства навигации решений.|
|[Список ожидающихAccessReviewInstances (обесценив)](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [accessReviewInstance collection](accessreviewinstance.md) . | Получите все ожидающих accessReviewInstance ресурсы, назначенные вызываемой пользователю. Этот метод отстает и заменяется [фильтромByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md). |

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------------------------------- | :---------- |
| endDateTime | DateTimeOffset | DateTime, когда экземпляр проверки должен завершиться. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$select`. Только для чтения.|
| ошибки | [коллекция accessReviewError](accessreviewerror.md)| Набор ошибок в жизненном цикле экземпляра проверки доступа. Только для чтения. |
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей рецензентов используется для определения списка рецензентов откатов. Эти рецензенты откатов будут уведомлены о необходимости принятия мер, если пользователи не будут найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует. Поддерживает `$select`.|
| id | Строка | Уникальный идентификатор экземпляра. Поддерживает `$select`. Только для чтения.|
| scope | [accessReviewScope](accessreviewscope.md) | Создан на **основе области** и **экземпляраEnumerationScope** на уровне accessReviewScheduleDefinition. Определяет область пользователей, рассмотренных в группе. Поддерживает и `$select` `$filter` (`contains` только). Только для чтения. |
| startDateTime | DateTimeOffset | DateTime при запуске экземпляра проверки. Может быть в будущем. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$select`. Только для чтения. |
| status | String | Указывает состояние accessReview. Возможные значения: `Initializing`, `NotStarted`, `Starting`, `InProgress`, , `Completing`, `Completed`и `AutoReviewing``AutoReviewed`. `$select`Поддерживает и `$orderby``$filter` (`eq`только). Только для чтения.|
| рецензенты   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей обзора доступа используется для определения того, кто такие рецензенты. Поддерживает `$select`. Примеры вариантов назначения рецензентов см. в примере Назначение рецензентов определению обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-scope-concept)|


## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| contactedReviewers   |[коллекция accessReviewReviewer](../resources/accessreviewreviewer.md)| Возвращает коллекцию рецензентов, с которыми связывались для завершения этого обзора. Хотя свойства  рецензентов и **fallbackReviewers** **accessReviewScheduleDefinition** могут указывать владельцев групп или менеджеров в качестве рецензентов **,** **contactedReviewers** возвращает их индивидуальные удостоверения. Поддерживает `$select`. Только для чтения. |
| определение               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | Существует точно один **accessReviewScheduleDefinition** , связанный с каждым экземпляром. Это родительское расписание экземпляра, в котором создаются экземпляры для каждого повторения определения обзора и каждой группы, выбранной для проверки по определению. |
|stages|[коллекция accessReviewStage](accessreviewstage.md)| Если экземпляр имеет несколько этапов, это возвращает коллекцию этапов. Новый этап будет создан только после окончания предыдущего этапа. Существование, число и параметры этапов в экземпляре обзора создаются на основе [accessReviewStageSettings](accessreviewstagesettings.md) в родительском [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). |
| решения               |[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection        | Каждый пользователь, рассмотренный в **accessReviewInstance** , имеет элемент решения, представляющий, были ли они утверждены, отклонены или еще не рассмотрены. |

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
