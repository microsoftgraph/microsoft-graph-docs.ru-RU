---
title: тип ресурса accessReviewHistoryDefinition
description: Представляет коллекцию данных истории обзоров доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7411ee6d3f8c078f1c8cfb9381632455b78be9bf
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804089"
---
# <a name="accessreviewhistorydefinition-resource-type"></a>тип ресурса accessReviewHistoryDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию исторических данных обзора доступа и областей, используемых для сбора этих данных.

**AccessReviewHistoryDefinition** содержит список [объектов accessReviewHistoryInstance](accessReviewHistoryInstance.md). Каждое повторение определения истории создает экземпляр. В случае разового определения истории создается только один экземпляр.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список accessReviewHistoryDefinitions](../api/accessreviewset-list-historydefinitions.md)|[accessReviewHistoryDefinition collection](accessreviewhistorydefinition.md)|Получите список объектов [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) и их свойств.|
|[Создание accessReviewHistoryDefinition](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Создайте новый [объект accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[Получить accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[userIdentity](useridentity.md)| Пользователь, создавший это определение истории обзора. |
|createdDateTime|DateTimeOffset|Timestamp, когда было создано определение проверки доступа.|
|решения|Коллекция строк|Определяет, какие решения по проверке будут включены в данные истории проверки, если заданы. Необязательный для создания. Все решения будут включены по умолчанию, если не будут предоставлены решения о создании. Возможные значения: `approve`, , , `dontKnow`, и `notReviewed``notNotified`. `deny`|
|displayName|String|Имя для сбора данных истории проверки доступа. Обязательный.|
|id|String|Назначен уникальный идентификатор определения истории проверки доступа.|
|reviewHistoryPeriodEndDateTime|DateTimeOffset| Timestamp. Обзоры, заканчивающийся до этой даты, будут включены в извлеченные данные истории. Только если **расписаниеSettings** не определено. |
|reviewHistoryPeriodStartDateTime|DateTimeOffset|Timestamp. Обзоры, начиная с этой даты или до этой даты, будут включены в извлеченные данные истории. Только если **расписаниеSettings** не определено.|
| scheduleSettings  |[accessReviewHistoryScheduleSettings](accessReviewHistoryScheduleSettings.md)| Параметры для серии определений истории повторного просмотра доступа. Только если не определены **reviewHistoryPeriodStartDateTime** или **reviewHistoryPeriodEndDateTime** .|
|scopes|[коллекция accessReviewScope](accessreviewscope.md)|Используется для области, включаемой отзывов в извлеченные данные истории. Извлекает отзывы, область которых совпадает с этой предоставленной областью. Обязательный.|
|status| accessReviewHistoryStatus|Представляет состояние коллекции данных истории отзывов. Допустимые значения: `done`, `inProgress`, `error`, `requested`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|instances|[accessReviewHistoryInstance](accessreviewhistoryinstance.md) collection| Если **accessReviewHistoryDefinition** является повторяющимся определением, экземпляры представляют каждое повторение. Определение, которое не повторяется, будет иметь точно один экземпляр.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "status": "String",
  "decisions": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "scopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "scheduleSettings": {
    "@odata.type": "microsoft.graph.accessReviewHistoryScheduleSettings"
  }
}
```
