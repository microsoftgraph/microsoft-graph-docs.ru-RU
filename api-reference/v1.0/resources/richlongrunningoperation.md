---
title: Тип ресурса richLongRunningOperation
description: Представляет состояние длительной операции на сайте или в списке.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 73f57e5daaf2f55aca6fa03f0958d19d8323bdf8
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191883"
---
# <a name="richlongrunningoperation-resource-type"></a>Тип ресурса richLongRunningOperation

Пространство имен: microsoft.graph

Представляет состояние длительной операции на [сайте или](../resources/site.md) в [списке](../resources/list.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение richLongRunningOperation](../api/richlongrunningoperation-get.md)|[richLongRunningOperation](../resources/richlongrunningoperation.md)|Получение состояния [полнофункциональных длительных операций](../resources/richlongrunningoperation.md) на [сайте или](../resources/site.md) в [списке](../resources/list.md).|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания этой операции.|
|error|[publicError](../resources/publicerror.md)| Ошибка, вызвавшая сбой операции.|
|id|Строка|Уникальный идентификатор операции. Наследуется от [сущности](../resources/entity.md).|
|lastActionDateTime|DateTimeOffset| Дата и время последнего действия, выполненного с этой операцией.|
|percentageComplete|Int32|Значение от 0 до 100, указывающее ход выполнения операции.|
|resourceId|String|Уникальный идентификатор результата.|
|resourceLocation|Строка|Канонический URL-адрес ресурса.|
|status|longRunningOperationStatus|Состояние длительной операции. Возможные значения: `notStarted`, `running`, `succeeded`, `failed`, `unknownFutureValue`.|
|statusDetail|Строка|Сведения о значении состояния.|
|type|String| Тип операции.|

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
  "createdDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "percentageComplete": "Integer",
  "resourceId": "String",
  "resourceLocation": "String",
  "status": "String",
  "statusDetail": "String",
  "type": "String"
}
```

