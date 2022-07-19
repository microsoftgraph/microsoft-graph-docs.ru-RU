---
title: Тип ресурса ediscoveryAddToReviewSetOperation
description: Представляет операцию добавления объекта eDiscoverySearch в eDiscoveryReviewSet.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e0b48551b191b8ead96b27ec68a17090bbdfe5b8
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66840189"
---
# <a name="ediscoveryaddtoreviewsetoperation-resource-type"></a>Тип ресурса ediscoveryAddToReviewSetOperation

Пространство имен: microsoft.graph.security



Представляет операцию добавления [объекта eDiscoverySearch](../resources/security-ediscoverysearch.md) в [eDiscoveryReviewSet](../resources/security-ediscoveryreviewset.md).

Наследуется от [caseOperation](../resources/security-caseoperation.md).

## <a name="methods"></a>Методы
Нет.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|microsoft.graph.security.caseAction| Тип действия, представляемого операцией. Возможные значения: `addToReviewSet`,,,`contentExport`,`convertToPdf``estimateStatistics``applyTags`,`purgeData`|
|completedDateTime|DateTimeOffset| Дата и время завершения операции. |
|createdBy|[identitySet](../resources/identityset.md)| Пользователь, создавшего операцию. |
|createdDateTime|DateTimeOffset| Дата и время создания операции. |
|id|Строка| Идентификатор операции. Только для чтения. |
|percentProgress|Int32| Ход выполнения операции. |
|resultInfo|[resultInfo](../resources/resultinfo.md)| Содержит сведения о результатах успешного выполнения и сбоя. |
|status|microsoft.graph.security.caseOperationStatus| Состояние операции обращения. Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|reviewSet|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Для проверки обнаружения электронных данных задано, какие элементы, соответствующие запросу исходной коллекции, добавляются.|
|search|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Поиск обнаружения электронных данных, который добавляется в набор для проверки.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryAddToReviewSetOperation",
  "baseType": "microsoft.graph.security.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryAddToReviewSetOperation",
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
  }
}
```

