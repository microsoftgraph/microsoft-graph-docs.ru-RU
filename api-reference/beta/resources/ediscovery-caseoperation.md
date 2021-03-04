---
title: тип ресурса caseOperation
description: Абстрактная сущность, которая представляет собой длительный процесс электронных разыскных открытий.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b94aeba03a49f2c49cbf991f0046422a18b20b50
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447559"
---
# <a name="caseoperation-resource-type"></a>тип ресурса caseOperation

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактная сущность, которая представляет собой длительный процесс электронных разыскных открытий. Он содержит общий набор свойств, которые разделяются между наследующих сущностями.  Сущности, которые вытекают из **caseOperation,** включают:

- [caseExportOperation](../resources/ediscovery-caseexportoperation.md)
- [tagOperation](../resources/ediscovery-tagoperation.md)
- [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md)

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Methods

Нет.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|action|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| Тип действия, который представляет операция. Возможные значения: `addToReviewSet` `applyTags` , , `contentExport` `convertToPdf` ,`estimateStatistics`|
|completedDateTime|DateTimeOffset| Дата и время завершения операции. |
|createdBy|[identitySet](../resources/identityset.md)| Пользователь, создав операцию. |
|createdDateTime|DateTimeOffset| Дата и время создания операции. |
|id|String| ID для операции. Только для чтения. |
|percentProgress|Int32| Ход операции. |
|resultInfo|[resultInfo](../resources/resultinfo.md)| Содержит сведения о результатах, характерных для успешного и неудачного сбоя. |
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)| Состояние операции дела. Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

### <a name="caseaction-values"></a>значения caseAction

|Member|Описание|
|:----|-----------|
| addToReviewSet | Операция представляет добавление данных в набор отзывов из коллекции eDiscovery. |
| applyTags | Операция представляет документы с массовыми тегами в наборе отзывов для указанного запроса набора обзоров. |
| contentExport | Операция представляет экспорт контента из набора отзывов. |
| convertToPdf | Операция представляет преобразование документов в PDF с помощью отредакций. |
| estimateStatistics  | Операция представляет поиск по таким службам Microsoft 365, как Exchange, SharePoint и OneDrive для бизнеса. |

### <a name="caseoperationstatus-values"></a>значения caseOperationStatus

|Member|Описание|
|:----|-----------|
| notStarted | Операция еще не началась. |
| submissionFailed | Отправка операции не удалась. |
| запуск | Операция в настоящее время запущена. |
| успешно | Операция была успешно выполнена без ошибок. |
| partiallySucceeded | Операция завершена, но произошли ошибки . Сведения об ошибках см. [в материале resultInfo.](../resources/resultinfo.md) |
| не удалось | Операция не удалась . Сведения об ошибках см. в результатах. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
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
