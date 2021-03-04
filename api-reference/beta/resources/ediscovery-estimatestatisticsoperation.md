---
title: тип ресурса estimateStatisticsOperation
description: Представляет операцию, которая обрабатывает оценку подсчета и размера коллекции исходных данных.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e816ba01d4bb648a8e78b5b96369236f63fb163e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447487"
---
# <a name="estimatestatisticsoperation-resource-type"></a>тип ресурса estimateStatisticsOperation

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет операцию, которая обрабатывает оценку подсчета и размера [sourceCollection.](../resources/ediscovery-sourcecollection.md) Дополнительные сведения [см. в материале Сбор данных по делу в advanced eDiscovery.](/microsoft-365/compliance/collecting-data-for-ediscovery)

Наследует [от caseOperation](../resources/ediscovery-caseoperation.md).

## <a name="methods"></a>Methods

Нет.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|action|microsoft.graph.ediscovery.caseAction| Тип операции. Действие случая для этой сущности всегда будет `estimateStatistics` . Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|completedDateTime|DateTimeOffset|Дата и время завершения операции. Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший операцию. Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|createdDateTime|DateTimeOffset|Дата и время начала операции. Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|id|String| ID для операции. Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|indexedItemCount|Int64|Предполагаемое количество элементов **для sourceCollection,** которые соответствуют запросу контента.|
|indexedItemsSize|Int64|Предполагаемый размер элементов **для sourceCollection,** совпадающий с запросом контента.|
|mailboxCount|Int32|Количество почтовых ящиков с хитами поиска.|
|percentProgress|Int32|Ход операции. Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Содержит сведения о результатах, характерных для успешного и неудачного сбоя. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|siteCount|Int32|Количество почтовых ящиков с хитами поиска.|
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|Состояние операции дела. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md). Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|
|unindexedItemCount|Int64|Предполагаемое количество неиндексуальных элементов для коллекции.|
|unindexedItemsSize|Int64|Предполагаемый размер неиндексуальных элементов для коллекции.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|sourceCollection|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|коллекция электронных данных, обычно известная как поиск.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.estimateStatisticsOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/operations/$entity",
    "@odata.type": "#microsoft.graph.ediscovery.estimateStatisticsOperation",
    "createdDateTime": "2021-01-12T18:47:23.3974907Z",
    "completedDateTime": "2021-01-12T18:47:51.1461805Z",
    "percentProgress": 100,
    "status": "succeeded",
    "action": "estimateStatistics",
    "id": "82edd40e182a464fa02c24a36fa94873",
    "indexedItemCount": 2,
    "indexedItemsSize": 39276,
    "unindexedItemCount": 0,
    "unindexedItemsSize": 0,
    "mailboxCount": 1,
    "siteCount": 0,
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```
