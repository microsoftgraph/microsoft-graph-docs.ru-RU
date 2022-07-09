---
title: Тип ресурса accessReviewStage
description: Представляет этап accessReviewInstance.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 20e23693bce96e0e10eb0f173ceb65ee1516a0a8
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698081"
---
# <a name="accessreviewstage-resource-type"></a>Тип ресурса accessReviewStage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет этап Azure AD [проверки](accessreviewsv2-overview.md) доступа. Если родительский [объект accessReviewScheduleDefinition](accessreviewscheduledefinition.md) определил свойство **stageSettings** , [accessReviewInstance](accessReviewInstance.md) будет состоять из трех последующих этапов. На каждом этапе может быть разный набор рецензентов, которые могут действовать над промежуточными решениями, и параметры, определяющее, какие решения будут передаваться от этапа к этапу.

**Каждый accessReviewStage** содержит список решений [,](accessreviewinstancedecisionitem.md) с помощью которых рецензенты могут принимать меры. Для каждого проверяемого удостоверения принимается только одно решение.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов accessReviewStage](../api/accessreviewinstance-list-stages.md)|[Коллекция accessReviewStage](../resources/accessreviewstage.md)|Получение списка объектов [accessReviewStage](../resources/accessreviewstage.md) и их свойств.|
|[Получение accessReviewStage](../api/accessreviewstage-get.md)|[accessReviewStage](../resources/accessreviewstage.md)|Чтение свойств и связей объекта [accessReviewStage](../resources/accessreviewstage.md) .|
|[Обновление accessReviewStage](../api/accessreviewstage-update.md)|[accessReviewStage](../resources/accessreviewstage.md)|Обновление свойств объекта [accessReviewStage](../resources/accessreviewstage.md) .|
|[stop](../api/accessreviewstage-stop.md)|Отсутствует| Остановите accessReviewStage вручную.|
|[filterByCurrentUser](../api/accessreviewstage-filterbycurrentuser.md)|[Коллекция accessReviewStage](../resources/accessreviewstage.md)|Возвращает все этапы для данного [объекта accessReviewInstance](accessReviewInstance.md)  , для которого вызывающий пользователь является рецензентом.|
|[Список решений](../api/accessreviewstage-list-decisions.md)|[Коллекция accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Получение решений, принятых в accessReviewStage.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|endDateTime|DateTimeOffset|Дата и время окончания этапа проверки. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда используется во время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Это свойство является совокупным итогом **длительностиInDays** для всех этапов. Только для чтения. |
|fallbackReviewers|[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Эта коллекция областей рецензента используется для определения списка резервных рецензентов. Эти резервные рецензенты будут получать уведомления о том, что нужно принять меры, если пользователи не найдены в указанном списке рецензентов. Это может произойти, если владелец группы указан в качестве рецензента, но владелец группы не существует, или руководитель указан в качестве рецензента, но руководитель пользователя не существует.|
|id|String|Уникальный идентификатор этапа. Только для чтения.|
|Авторам|[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Эта коллекция областей проверки доступа используется для определения рецензентов. Примеры параметров назначения рецензентов см. в статье "Назначение рецензентов определению проверки доступа с [помощью microsoft API Graph"](/graph/accessreviews-scope-concept).|
|startDateTime|DateTimeOffset|Дата и время начала этапа проверки. Может быть в будущем. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
|status|String|Указывает состояние accessReviewStage. Возможные значения: `Initializing`, `NotStarted`, `Starting`, , `InProgress`, `Completing`, `Completed`, и `AutoReviewed``AutoReviewing`. Поддерживает и `$orderby``$filter` (`eq`только). Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|Решения|[Коллекция accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|У каждого пользователя, проверяемого в accessReviewStage, есть элемент принятия решения, который указывает, утверждены ли они, отклонены или еще не просмотрелись.|

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

