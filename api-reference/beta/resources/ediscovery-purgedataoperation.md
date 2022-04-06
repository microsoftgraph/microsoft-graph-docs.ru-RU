---
title: тип ресурса purgeDataOperation
description: Представляет операцию по окончательному удалите данные в sourceCollection. В настоящее время операция только Microsoft Teams сообщений.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 5562658c40831cea39922dfd5d1e1edc1d214392
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608422"
---
# <a name="purgedataoperation-resource-type"></a>тип ресурса purgeDataOperation

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет операцию по окончательному удалите данные в sourceCollection. В настоящее время эта операция Microsoft Teams только для сообщений; в будущем будет больше источников данных.

Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| Тип действия, который представляет операция. Возможные значения: `addToReviewSet`,`applyTags`,`contentExport`,`convertToPdf`,,`estimateStatistics`.`purgeData`|
|completedDateTime|DateTimeOffset| Дата и время завершения операции. |
|createdBy|[identitySet](../resources/identityset.md)| Пользователь, создав операцию. |
|createdDateTime|DateTimeOffset| Дата и время создания операции. |
|id|String| ID для операции. Только для чтения. |
|percentProgress|Int32| Ход операции. |
|resultInfo|[resultInfo](../resources/resultinfo.md)| Содержит сведения о результатах, характерных для успешного и неудачного сбоя. |
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)| Состояние операции дела. Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.purgeDataOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.purgeDataOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```
