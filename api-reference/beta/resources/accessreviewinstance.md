---
title: Тип ресурса accessReviewInstance
description: Представляет повторение `accessReviewScheduleDefinition` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0f480b870af2fd4717ff1341a1ab66b73301fc7f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158536"
---
# <a name="accessreviewinstance-resource-type"></a>Тип ресурса accessReviewInstance

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет повторение [проверки](accessreviewsv2-root.md) доступа Azure AD. Если родительский [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) является повторяющимся обзором доступа, экземпляры представляют каждое повторение. Повторная проверка будет иметь только один экземпляр. Экземпляры также представляют каждую уникальную группу, проверяемую в определении расписания. Если определение расписания проверяет несколько групп, каждая группа будет иметь уникальный экземпляр для каждого повторения.

Каждый **accessReviewInstance** содержит список решений, которые могут принять рецензенты. [](accessreviewinstancedecisionitem.md) Существует одно решение для каждого проверяемого удостоверения.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Список accessReviewInstances](../api/accessreviewinstance-list.md) | [Коллекция accessReviewInstance](accessreviewinstance.md) | Получите список объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств. |
|[Get accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Возвращает accessReviewInstance для accessReviewScheduleDefinition. Не включает связанные объекты accessReviewInstanceDecisionItem. |
|[Список pendingAccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [коллекция accessReviewInstance;](accessreviewinstance.md) | Получите все ожидающих ресурсов accessReviewInstance, которые назначены вызываемму пользователю. |
|[Отправка напоминания accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Нет. | Отправьте напоминание рецензентам accessReviewInstance. |
|[Остановка accessReviewInstance](../api/accessreviewinstance-stop.md) | Нет. | Вручную остановите accessReviewInstance. |
|[Принятие рекомендаций](../api/accessreviewinstance-acceptrecommendations.md) | Нет. | Позволяет вызываемой пользователю принять рекомендации по принятию решений для каждого notReviewed accessReviewInstanceDecisionItem, в которых он является рецензентом для определенного accessReviewInstance. |
|[Применение решений](../api/accessreviewinstance-applydecisions.md) | Нет. | Вручную применить решение для accessReviewInstance. |



## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------------------------------- | :---------- |
| id | String | Уникальный идентификатор экземпляра. |
| displayName | String | Имя родительского accessReviewScheduleDefinition. |
| startDateTime | DateTimeOffset | Дата и время, когда запланирован запуск экземпляра проверки. Может быть в будущем. |
| endDateTime | DateTimeOffset | DateTime, когда планируется завершение экземпляра проверки. |
| status | string | Указывает состояние accessReview. Типичные состояния: `Initializing` , , , , , и `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` .  Только для чтения.|
| scope | [accessReviewScope](accessreviewscope.md) | Создается **на основе области** и **экземпляраEnumerationScope** на уровне accessReviewScheduleDefinition. Определяет область пользователей, проверяемую в группе. В случае одногруппной проверки область, определяемая на уровне, применяется `accessReviewScheduleDefinition` ко всем экземплярам. В случае проверки всех групп область действия для каждой группы может быть разной. Только для чтения.  | 
| decisions | [Коллекция accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Каждый пользователь, рассмотренный в accessReviewInstance, имеет элемент решения, представляющий, был ли его доступ утвержден, отклонен или еще не рассмотрен. |
| definition |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | С каждым экземпляром связан только один accessReviewScheduleDefinition. Это родительское расписание экземпляра, в котором создаются экземпляры для каждого повторения определения проверки и каждой группы, выбранной для проверки определением. |

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `definition`               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | С каждым экземпляром связан именно один `accessReviewScheduleDefinition` экземпляр. Это родительское расписание экземпляра, в котором создаются экземпляры для каждого повторения определения проверки и каждой группы, выбранной для проверки определением. |
| `decisions`               |[Коллекция accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)        | Каждый пользователь, рассмотренный в документе, имеет элемент решения, представляющий, утвержден ли, отклонен или `accessReviewInstance` еще не рассмотрен. |

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
