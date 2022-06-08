---
title: Тип ресурса ediscoveryAddToReviewSetOperation
description: Добавляет результаты объекта sourceCollection в reviewSet.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 888f96bc37b476055513f43c9086a57b4d2c6cbc
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946139"
---
# <a name="ediscoveryaddtoreviewsetoperation-resource-type"></a>Тип ресурса ediscoveryAddToReviewSetOperation

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет операцию добавления [объекта eDiscoverySearch](../resources/security-ediscoverysearch.md) в [eDiscoveryReviewSet](../resources/security-ediscoveryreviewset.md).

Наследуется от [caseOperation](../resources/security-caseoperation.md).

## <a name="methods"></a>Методы
Нет.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|Строка| Тип действия, представляемого операцией. Возможные значения: `addToReviewSet`,,,`contentExport`,`convertToPdf``estimateStatistics``applyTags`,`purgeData`|
|completedDateTime|DateTimeOffset| Дата и время завершения операции. |
|createdBy|[identitySet](../resources/identityset.md)| Пользователь, создавшего операцию. |
|createdDateTime|DateTimeOffset| Дата и время создания операции. |
|id|String| Идентификатор операции. Только для чтения. |
|percentProgress|Int32| Ход выполнения операции. |
|resultInfo|[resultInfo](../resources/resultinfo.md)| Содержит сведения о результатах успешного выполнения и сбоя. |
|status|String| Состояние операции обращения. Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

## <a name="relationships"></a>Отношения
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

