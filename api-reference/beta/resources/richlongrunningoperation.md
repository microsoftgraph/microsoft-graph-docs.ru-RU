---
title: тип ресурса richLongRunningOperation
description: Содержит метаданные о длительной работе.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 2f16e9abb8dc3a22ad7a3d3b32e707ddb595c06a
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162328"
---
# <a name="richlongrunningoperation-resource-type"></a>тип ресурса richLongRunningOperation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит метаданные о длительной работе.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список richLongRunningOperations на сайте](../api/site-list-operations.md)|[richLongRunningOperation](../resources/richlongrunningoperation.md) collection|Получите список объектов [richLongRunningOperation](../resources/richlongrunningoperation.md) и их свойств на сайте.|
|[Список richLongRunningOperations в списке](../api/list-list-operations.md)|[richLongRunningOperation](../resources/richlongrunningoperation.md) collection|Получите список объектов [richLongRunningOperation](../resources/richlongrunningoperation.md) и их свойств в списке.|
|[Получить richLongRunningOperation](../api/richlongrunningoperation-get.md)|[richLongRunningOperation](../resources/richlongrunningoperation.md)|Ознакомьтесь с свойствами объекта [richLongRunningOperation.](../resources/richlongrunningoperation.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Время создания этой операции.|
|error|[publicError](../resources/publicerror.md)| Ошибка, из-за которой операция не удалась.|
|id|Строка|Идентификатор операции. Наследует от [объекта](../resources/entity.md).|
|lastActionDateTime|DateTimeOffset| Время выполнения последнего действия в этой операции.|
|percentageComplete|Int32|Значение от 0 до 100, которое указывает на ход операции.|
|resourceId|String|Уникальный идентификатор для результата.|
|resourceLocation|Строка|Канонический URL-адрес ресурса.|
|status|longRunningOperationStatus|Состояние opertaion. Возможные значения: `notStarted` `running` , , , `succeeded` `failed` `unknownFutureValue` .|
|statusDetail|Строка|Подробные подробности о значении состояния.|
|type|Строка| Тип операции.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.richLongRunningOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.richLongRunningOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "resourceLocation": "String",
  "status": "String",
  "statusDetail": "String",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "percentageComplete": "Integer",
  "resourceId": "String",
  "type": "String"
}
```

