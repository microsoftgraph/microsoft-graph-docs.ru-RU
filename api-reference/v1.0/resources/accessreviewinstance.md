---
title: тип ресурсов accessReviewInstance
description: Представляет собой повторение `accessReviewScheduleDefinition` .
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f77e5ae6d16b96fff2586b5b2bd920d01737196d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025673"
---
# <a name="accessreviewinstance-resource-type"></a>тип ресурсов accessReviewInstance

Пространство имен: microsoft.graph

Представляет повторение проверки доступа Azure [AD.](accessreviewsv2-root.md) Система, созданная на основе родительского [доступаReviewScheduleDefinition](accessreviewscheduledefinition.md). Все свойства только для чтения.

Если экземпляр является частью повторного обзора доступа, экземпляры представляют каждое повторение. Обзор, который не повторяется, будет иметь точно один экземпляр. Экземпляры также представляют каждый уникальный ресурс, который просматривается в определении расписания. Если определение расписания проверяет несколько ресурсов, каждый ресурс будет иметь уникальный экземпляр для каждого повторения.

Каждый **accessReviewInstance содержит** список решений, которые могут приниматься рецензентами. [](accessreviewinstancedecisionitem.md) Существует одно решение для каждого проверяемого удостоверения.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список accessReviewInstances](../api/accessreviewinstance-list.md)|[accessReviewInstance](../resources/accessreviewinstance.md) collection|Получите список объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств.|
|[Получить accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstance.](../resources/accessreviewinstance.md)|
|[stop](../api/accessreviewinstance-stop.md)|Нет|Вручную остановите accessReviewInstance.|
|[sendReminder](../api/accessreviewinstance-sendreminder.md)|Нет|Отправьте напоминание рецензентам accessReviewInstance.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Нет|Сброс всех элементов решений в экземпляре `notReviewed`|
|[applyDecisions](../api/accessreviewinstance-applydecisions.md)|Нет|Вручную применить решение для accessReviewInstance.|
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|Нет| Позволяет вызываемой пользователю принять рекомендацию по принятию решений для каждого notReviewed accessReviewInstanceDecisionItem, на которых он является рецензентом для определенного accessReviewInstance.|
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Нет|Просмотр пакетов принципов или ресурсов в одном вызове.|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) collection|Возвращает все объекты экземпляра в определение, для которого вызываемая пользователь является рецензентом.|
|[Список решений](../api/accessreviewinstance-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Получите ресурсы accessReviewInstanceDecisionItem из свойства навигации решений.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| endDateTime | DateTimeOffset | DateTime, когда экземпляр проверки должен завершиться. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$select`. Только для чтения.|
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей рецензентов используется для определения списка рецензентов откатов. Эти рецензенты откатов будут уведомлены о необходимости принятия мер, если пользователи не будут найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует. Поддерживает `$select`.|
| id | Строка | Уникальный идентификатор экземпляра. Наследуется от [сущности](../resources/entity.md). Поддерживает `$select`. Только для чтения.|
| scope | [accessReviewScope](accessreviewscope.md) | Создан на **основе области** и **экземпляраEnumerationScope** на уровне accessReviewScheduleDefinition. Определяет область пользователей, рассмотренных в группе. Поддерживает `$select` и `$filter` `contains` (только). Только для чтения. |
| startDateTime | DateTimeOffset | DateTime при запуске экземпляра проверки. Может быть в будущем. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$select`. Только для чтения. |
| status | String | Указывает состояние accessReview. Возможные значения: `Initializing` , , , , , , и `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . Поддерживает `$select` и `$orderby` `$filter` `eq` (только). Только для чтения.|
| рецензенты   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей обзора доступа используется для определения того, кто такие рецензенты. Поддерживает `$select`. Примеры вариантов назначения рецензентов см. в примере Назначение рецензентов определению обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-scope-concept)|


## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|решения|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Каждый из основных элементов, рассмотренных в элементе решения, представляет, были ли они утверждены, отклонены `accessReviewInstance` или еще не рассмотрены.|

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
