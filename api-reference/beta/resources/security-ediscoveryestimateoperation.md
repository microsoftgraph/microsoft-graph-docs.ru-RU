---
title: Тип ресурса ediscoveryEstimateOperation
description: Представляет процесс оценки статистики (количество элементов, размер и количество расположений) поиска по обнаружению электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f4edad31ab7e5c1018cae4e681559d189ba8ef30
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838257"
---
# <a name="ediscoveryestimateoperation-resource-type"></a>Тип ресурса ediscoveryEstimateOperation

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет процесс оценки статистики (количество элементов, размер и количество расположений) поиска по обнаружению электронных данных.

Наследуется от [caseOperation](../resources/security-caseoperation.md).

## <a name="methods"></a>Методы
Нет.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|microsoft.graph.security.caseAction| Тип действия, представляемого операцией. Возможные значения: `addToReviewSet`,,,`contentExport`,`convertToPdf``estimateStatistics``applyTags`,`purgeData`|
|completedDateTime|DateTimeOffset|Дата и время завершения операции. Только для чтения. |
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший операцию. Только для чтения. |
|createdDateTime|DateTimeOffset|Дата и время начала операции. Только для чтения.|
|id|Строка| Идентификатор операции. Только для чтения.|
|indexedItemCount|Int64|Предполагаемое количество элементов для поиска **,** соответствующих запросу содержимого.|
|indexedItemsSize|Int64|Предполагаемый размер элементов для поиска **,** соответствующих запросу содержимого.|
|mailboxCount|Int32|Количество почтовых ящиков с совпадением поиска.|
|percentProgress|Int32|Ход выполнения операции. Только для чтения. |
|resultInfo|[resultInfo](../resources/resultinfo.md)|Содержит сведения о результатах успешного выполнения и сбоя. |
|siteCount|Int32|Количество почтовых ящиков с совпадением поиска.|
|status|microsoft.graph.security.caseOperationStatus| Состояние операции обращения. Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|
|unindexedItemCount|Int64|Предполагаемое количество неиндексированных элементов для коллекции.|
|unindexedItemsSize|Int64|Предполагаемый размер неиндексированных элементов для коллекции.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|search|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Поиск по обнаружению электронных данных.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryEstimateOperation",
  "baseType": "microsoft.graph.security.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryEstimateOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "percentProgress": "Integer",
  "status": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "indexedItemCount": "Integer",
  "indexedItemsSize": "Integer",
  "unindexedItemCount": "Integer",
  "unindexedItemsSize": "Integer",
  "mailboxCount": "Integer",
  "siteCount": "Integer"
}
```

