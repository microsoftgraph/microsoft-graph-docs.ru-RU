---
title: Тип ресурса accessReviewHistoryDefinition
description: Представляет коллекцию данных журнала проверки доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 935f27083f2c2f49d92079cad02aa1174d1cb68f
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697248"
---
# <a name="accessreviewhistorydefinition-resource-type"></a>Тип ресурса accessReviewHistoryDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию исторических данных проверки доступа и областей, используемых для сбора этих данных.

**AccessReviewHistoryDefinition** содержит список [объектов accessReviewHistoryInstance](accessReviewHistoryInstance.md). Каждое повторение определения журнала создает экземпляр. В случае определения единого журнала создается только один экземпляр.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов accessReviewHistoryDefinitions](../api/accessreviewset-list-historydefinitions.md)|[Коллекция accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Получение списка объектов [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) и их свойств.|
|[Создание accessReviewHistoryDefinition](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Создайте объект [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[Получение accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Чтение свойств и связей объекта [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[userIdentity](useridentity.md)| Пользователь, создавший это определение журнала проверки. |
|createdDateTime|DateTimeOffset|Метка времени создания определения проверки доступа.|
|Решения|Коллекция строк|Определяет, какие решения о проверке будут включены в извлеченные данные журнала проверки, если они указаны. Необязательный при создании. Все решения будут включены по умолчанию, если при создании не будут предоставлены решения. Возможные значения: `approve`, , , `dontKnow`, и `notReviewed``notNotified`. `deny`|
|displayName|Строка|Имя для сбора данных журнала проверки доступа. Обязательный.|
|id|String|Назначенный уникальный идентификатор определения журнала проверки доступа.|
|reviewHistoryPeriodEndDateTime|DateTimeOffset| Метка времени. Проверки, заканчивающиеся на эту дату или до этой даты, будут включены в извлеченные данные журнала. Требуется только в том случае, **если параметр scheduleSettings** не определен. |
|reviewHistoryPeriodStartDateTime|DateTimeOffset|Метка времени. Проверки, начиная с этой даты или до этой даты, будут включены в извлеченные данные журнала. Требуется только в том случае, **если параметр scheduleSettings** не определен.|
| scheduleSettings  |[accessReviewHistoryScheduleSettings](accessReviewHistoryScheduleSettings.md)| Параметры для серии определений журнала повторяющихся проверок доступа. Требуется только в том случае, если **параметр reviewHistoryPeriodStartDateTime** или **reviewHistoryPeriodEndDateTime** не определен. Пока не поддерживается.|
|scopes|[Коллекция accessReviewScope](accessreviewscope.md)|Используется для определения того, какие проверки включены в извлеченные данные журнала. Извлекает проверки, область которых соответствует указанной области. Обязательный элемент.|
|status| accessReviewHistoryStatus|Представляет состояние сбора данных журнала проверки. Допустимые значения: `done`, `inProgress`, `error`, `requested`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|instances|[Коллекция accessReviewHistoryInstance](accessreviewhistoryinstance.md)| Если **accessReviewHistoryDefinition** является повторяющимся определением, экземпляры представляют каждое повторение. Определение, которое не является повторяемой, будет иметь ровно один экземпляр.|

## <a name="json-representation"></a>Представление JSON

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
