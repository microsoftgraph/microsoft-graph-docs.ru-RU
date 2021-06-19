---
title: тип ресурсов accessReviewInstance
description: Представляет собой повторение `accessReviewScheduleDefinition` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b2b191cede0f50f10d75747ca55e329185f6a9c1
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030770"
---
# <a name="accessreviewinstance-resource-type"></a>тип ресурсов accessReviewInstance

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет повторение проверки доступа Azure [AD.](accessreviewsv2-root.md) Если родительский [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) является повторяемой проверкой доступа, экземпляры представляют каждое повторение. Обзор, который не повторяется, будет иметь точно один экземпляр. Экземпляры также представляют каждую уникальную группу, проверяемую в определении расписания. Если определение расписания проверяет несколько групп, каждая группа будет иметь уникальный экземпляр для каждого повторения.

Каждый **accessReviewInstance содержит** список решений, которые могут приниматься рецензентами. [](accessreviewinstancedecisionitem.md) Существует одно решение для каждого проверяемого удостоверения.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Список accessReviewInstances](../api/accessreviewinstance-list.md) | [accessReviewInstance](accessreviewinstance.md) collection | Получите список объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств. |
|[Получить accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstance.](../resources/accessreviewinstance.md) |
|[Отправка напоминания accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Нет. | Отправьте напоминание рецензентам accessReviewInstance. |
|[Остановка accessReviewInstance](../api/accessreviewinstance-stop.md) | Нет. | Вручную остановите accessReviewInstance. |
|[Принятие рекомендаций](../api/accessreviewinstance-acceptrecommendations.md) | Нет. | Позволяет вызываемой пользователю принять рекомендацию по принятию решений для каждого notReviewed accessReviewInstanceDecisionItem, на которых он является рецензентом для определенного accessReviewInstance. |
|[Применение решений](../api/accessreviewinstance-applydecisions.md) | Нет. | Вручную применять решения для accessReviewInstance. |
|[Решения о пакетной записи](../api/accessreviewinstance-batchrecorddecisions.md)|Нет|Просмотр пакетов принципов или ресурсов в одном вызове.|
|[Сброс решений](../api/accessreviewinstance-resetdecisions.md)|Нет|Сброс всех элементов решений в экземпляре `notReviewed` в .|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) collection|Возвращает все экземпляры в данном [accessReviewScheduleDefinition,](accessreviewscheduledefinition.md) для которого вызываемая пользователь является рецензентом одного или более решений.|
|[Список решений](../api/accessreviewinstance-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Получите ресурсы accessReviewInstanceDecisionItem из свойства навигации решений.|
|[Список ожидающихAccessReviewInstances (обесценив)](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [accessReviewInstance collection.](accessreviewinstance.md) | Получите все ожидающих accessReviewInstance ресурсы, назначенные вызываемой пользователю. Этот метод отмещается и заменяется [фильтромByCurrentUser.](../api/accessreviewinstance-filterbycurrentuser.md) |

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------------------------------- | :---------- |
| id | String | Уникальный идентификатор экземпляра. Поддерживает `$select`. Только для чтения.|
| startDateTime | DateTimeOffset | DateTime при запуске экземпляра проверки. Может быть в будущем. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$select`. Только для чтения. |
| endDateTime | DateTimeOffset | DateTime, когда экземпляр проверки должен завершиться. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$select`. Только для чтения.|
| status | String | Указывает состояние accessReview. Возможные значения: `Initializing` , , , , , , и `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . Поддерживает `$select` и `$orderby` `$filter` `eq` (только). Только для чтения.|
| scope | [accessReviewScope](accessreviewscope.md) | Создан на **основе области** и **экземпляраEnumerationScope** на уровне accessReviewScheduleDefinition. Определяет область пользователей, рассмотренных в группе. Поддерживает `$select` и `$filter` `contains` (только). Только для чтения. |

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `definition`               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | Существует точно один `accessReviewScheduleDefinition` связанный с каждым экземпляром. Это родительское расписание экземпляра, в котором создаются экземпляры для каждого повторения определения обзора и каждой группы, выбранной для проверки по определению. |
| `decisions`               |[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection        | Каждый пользователь, рассмотренный в элементе, имеет элемент решения, представляющий, были ли они утверждены, отклонены `accessReviewInstance` или еще не рассмотрены. |

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
  }
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
