---
title: тип ресурса accessReviewStage
description: Представляет этап accessReviewInstance.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 53d0fa58f4aa494f1815a1205f45ba2673b9620c
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816225"
---
# <a name="accessreviewstage-resource-type"></a>тип ресурса accessReviewStage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет собой этап повторения повторного просмотра доступа Azure [AD.](accessreviewsv2-overview.md) Если родительский [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) определил свойство **stageSettings** , [то accessReviewInstance](accessReviewInstance.md) будет состоять из трех последующих этапов. На каждом этапе может быть разный набор рецензентов, которые могут действовать на этапе принятия решений, а также параметры, определяющие, какие решения будут передаваться от стадии к этапу.

**Каждый accessReviewStage** содержит список решений [,](accessreviewinstancedecisionitem.md) которые могут приниматься рецензентами. Существует только одно решение для каждого проверяемого удостоверения.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Списки accessReviewStages](../api/accessreviewinstance-list-stages.md)|[коллекция accessReviewStage](../resources/accessreviewstage.md)|Получите список объектов [accessReviewStage](../resources/accessreviewstage.md) и их свойств.|
|[Получить accessReviewStage](../api/accessreviewstage-get.md)|[accessReviewStage](../resources/accessreviewstage.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewStage](../resources/accessreviewstage.md) .|
|[Обновление accessReviewStage](../api/accessreviewstage-update.md)|[accessReviewStage](../resources/accessreviewstage.md)|Обновление свойств объекта [accessReviewStage](../resources/accessreviewstage.md) .|
|[stop](../api/accessreviewstage-stop.md)|Нет| Вручную остановите accessReviewStage.|
|[filterByCurrentUser](../api/accessreviewstage-filterbycurrentuser.md)|[коллекция accessReviewStage](../resources/accessreviewstage.md)|Возвращает все этапы на заданном [accessReviewInstance](accessReviewInstance.md)  , для которого вызываемая пользователь является рецензентом.|
|[Список решений](../api/accessreviewstage-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Получите решения, принятые в accessReviewStage.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|endDateTime|DateTimeOffset|DateTime, когда планируется завершить этап проверки. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Это свойство является совокупным итогом **продолжительностиInDays** для всех этапов. Только для чтения. |
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|Эта коллекция областей рецензентов используется для определения списка рецензентов откатов. Эти рецензенты откатов будут уведомлены о необходимости принятия мер, если пользователи не будут найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует.|
|id|String|Уникальный идентификатор сцены. Только для чтения.|
|рецензенты|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|Эта коллекция областей обзора доступа используется для определения того, кто такие рецензенты. Примеры вариантов назначения рецензентов см. в примере Назначение рецензентов определению обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-scope-concept)|
|startDateTime|DateTimeOffset|DateTime, когда планируется начать этап проверки. Может быть в будущем. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
|status|String|Указывает состояние accessReviewStage. Возможные значения: `Initializing`, `NotStarted`, `Starting`, `InProgress`, , `Completing`, `Completed`и `AutoReviewing``AutoReviewed`. Поддерживает и `$orderby``$filter` (`eq`только). Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|решения|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Каждый пользователь, рассмотренный в accessReviewStage, имеет элемент решения, представляющий, были ли они утверждены, отклонены или еще не рассмотрены.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewStage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewStage",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "status": "String",
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

