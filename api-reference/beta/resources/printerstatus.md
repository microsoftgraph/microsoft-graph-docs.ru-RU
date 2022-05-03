---
title: Тип ресурса printerStatus
description: Представляет состояние обработки принтера, включая все ошибки.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4b405fe00ab7dfe0e3ce90e79b1e7a82607f012c
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176547"
---
# <a name="printerstatus-resource-type"></a>Тип ресурса printerStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние обработки принтера, включая все ошибки.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|state|printerProcessingState|Текущее состояние обработки. Допустимые значения описаны в следующей таблице. Только для чтения.|
|details|Коллекция printerProcessingStateDetail|Список сведений, описывающий, почему принтер находится в текущем состоянии. Допустимые значения описаны в следующей таблице. Только для чтения.|
|description|Строка|Понятное для человека описание текущего состояния обработки принтера. Только для чтения.|

### <a name="printerprocessingstate-values"></a>Значения printerProcessingState

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние обработки, сообщаемое принтером, неизвестно.|
|Простоя|1|Принтер неактивен и готов к приему новых заданий печати.|
|Обработки|2|Принтер в настоящее время обрабатывает задание печати и будет обрабатывать все ожидающие задания по завершении.|
|Остановился|3|На принтере возникла проблема (например, из-за того, что в активной области не печаталась бумага) и не удается продолжить текущее задание печати, пока проблема не будет устранена. Дополнительные **сведения см**. в сведениях о  значениях или описании.|
|unknownFutureValue|4|Значение sentinel для развиваемого перечисления. Не следует использовать.|

### <a name="printerprocessingstatedetail-values"></a>Значения printerProcessingStateDetail

[Тип перечисления printerProcessingStateDetail](./printerprocessingstatedetail.md)

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerStatus"
}-->

```json
{
    "state": "String",
    "details": ["String"],
    "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

