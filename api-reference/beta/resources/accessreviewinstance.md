---
title: тип ресурсов accessReviewInstance
description: Представляет собой повторение `accessReviewScheduleDefinition` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8ef2e48900484c32669a56c15b88de87dc4710d3
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469058"
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
|[Получить accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Возвращает accessReviewInstance для accessReviewScheduleDefinition. Не включает связанный accessReviewInstanceDecisionItem в объекте. |
|[Список ожидающихAccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [accessReviewInstance collection.](accessreviewinstance.md) | Получите все ожидающих accessReviewInstance ресурсы, назначенные вызываемой пользователю. |
|[Отправка напоминания accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Нет. | Отправьте напоминание рецензентам accessReviewInstance. |
|[Остановка accessReviewInstance](../api/accessreviewinstance-stop.md) | Нет. | Вручную остановите accessReviewInstance. |
|[Принятие рекомендаций](../api/accessreviewinstance-acceptrecommendations.md) | Нет. | Позволяет вызываемой пользователю принять рекомендацию по принятию решений для каждого notReviewed accessReviewInstanceDecisionItem, на которых он является рецензентом для определенного accessReviewInstance. |
|[Применение решений](../api/accessreviewinstance-applydecisions.md) | Нет. | Вручную применить решение для accessReviewInstance. |
|[Решения о пакетной записи](../api/accessreviewinstance-batchrecorddecisions.md)|Нет|Просмотр пакетов принципов или ресурсов в одном вызове.|

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------------------------------- | :---------- |
| id | String | Уникальный идентификатор экземпляра. |
| displayName | String | Имя родительского [доступаReviewScheduleDefinition](accessreviewscheduledefinition.md). |
| startDateTime | DateTimeOffset | DateTime при запуске экземпляра проверки. Может быть в будущем. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| endDateTime | DateTimeOffset | DateTime, когда экземпляр проверки должен завершиться. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| status | String | Указывает состояние accessReview. Типичные состояния `Initializing` включают , , , , , , и `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` .  Только для чтения.|
| scope | [accessReviewScope](accessreviewscope.md) | Создан на **основе области** и **экземпляраEnumerationScope** на `accessReviewScheduleDefinition` уровне. Определяет область пользователей, рассмотренных в группе. В случае одногруппного обзора область, определяемая на уровне, `accessReviewScheduleDefinition` применяется ко всем экземплярам. В случае проверки всех групп область действия для каждой группы может быть различной. Только для чтения.  | 
| решения | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection | Каждый пользователь, рассмотренный в [accessReviewInstance,](#accessreviewinstance-resource-type) имеет элемент решения, представляющий, был ли его доступ одобрен, отклонен или еще не рассмотрен. |
| определение |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Существует точно один **accessReviewScheduleDefinition,** связанный с каждым экземпляром. Это родительское расписание экземпляра, в котором создаются экземпляры для каждого повторения определения обзора и каждой группы, выбранной для проверки по определению. |

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
