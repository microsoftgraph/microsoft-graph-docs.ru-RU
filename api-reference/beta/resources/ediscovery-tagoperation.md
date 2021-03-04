---
title: тип ресурса tagOperation
description: Представляет операцию, которая обрабатывает применение тегов к документам в наборе отзывов на основе запроса набора отзывов.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 2af9b255e643a46f5f065b3caf62fda0ae9967a4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447546"
---
# <a name="tagoperation-resource-type"></a>тип ресурса tagOperation

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет операцию, которая обрабатывает применение тегов к документам в наборе отзывов на основе запроса набора отзывов.

Наследует [от caseOperation](../resources/ediscovery-caseoperation.md).

## <a name="methods"></a>Methods

Нет.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|action|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| Действие случая для этой сущности всегда будет `applyTags` . Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|completedDateTime|DateTimeOffset|Дата и время завершения операции. Только для чтения. Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший операцию. Только для чтения. Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)|
|createdDateTime|DateTimeOffset|Дата и время начала операции. Только для чтения. Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)|
|id|String| ID для операции. Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|percentProgress|Int32|Ход операции. Только для чтения. Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Содержит сведения о результатах, характерных для успешного и неудачного сбоя. Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)|
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|Состояние операции дела. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md). Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tagOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tagOperation",
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
