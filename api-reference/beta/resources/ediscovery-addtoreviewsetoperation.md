---
title: тип ресурса addToReviewSetOperation
description: Добавляет результаты sourceCollection в reviewSet
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d7323fbd6d2d068888d556328fc3ea4e399ab2fe
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447586"
---
# <a name="addtoreviewsetoperation-resource-type"></a>тип ресурса addToReviewSetOperation

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет операцию по добавлению [sourceCollection](../resources/ediscovery-sourcecollection.md) в [reviewSet.](../resources/ediscovery-reviewset.md)

Наследует [от caseOperation](../resources/ediscovery-caseoperation.md).

## <a name="methods"></a>Methods

Нет.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|action|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| Действие случая для этой сущности всегда будет `addToReviewSet` . Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|completedDateTime|DateTimeOffset|Дата и время завершения операции. Только для чтения. Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший операцию. Только для чтения. Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)|
|createdDateTime|DateTimeOffset|Дата и время начала операции. Только для чтения. Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)|
|id|String| ID для операции. Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|percentProgress|Int32|Ход операции. Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Содержит сведения о результатах, характерных для успешного и неудачного сбоя. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|Состояние операции дела. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md). Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

### <a name="datacollectionscope-values"></a>значения dataCollectionScope

|Member|Описание|
|:----|-----------|
|allVersions|Включай все версии файлов с сайтов.|
|linkedFiles|**Включайте облачное** вложение с электронными письмами в коллекцию.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|reviewSet|[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)| Набор отзывов, к которым добавляются элементы, совпадающие с запросом коллекции источника. |
|sourceCollection|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourceCollection.md)| SourceCollection, из него добавляются элементы. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.addToReviewSetOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.addToReviewSetOperation",
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
