---
title: тип ресурса printerStatus
description: Представляет состояние обработки принтера, включая все ошибки.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 97462f4e2c7059eb857a382c4944da7b697ee363
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508456"
---
# <a name="printerstatus-resource-type"></a>тип ресурса printerStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние обработки принтера, включая все ошибки.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|state|printerProcessingState|Текущее состояние обработки. Допустимые значения описаны в следующей таблице. Только для чтения.|
|details|коллекция printerProcessingStateDetail|Список сведений, описывающих, почему принтер находится в текущем состоянии. Допустимые значения описаны в следующей таблице. Только для чтения.|
|description|String|Описание текущего состояния обработки принтера, считываемым человеком. Только для чтения.|

### <a name="printerprocessingstate-values"></a>значения printerProcessingState

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние обработки, о чем сообщает принтер, неизвестно.|
|праздный|1 |Принтер простаивает и готов к приему новых заданий печати.|
|обработка|2|В настоящее время принтер обрабатывает задание печати и обрабатывает все ожидающие задания по завершении.|
|остановлено|3 |Принтер столкнулся с проблемой (например, закончились бумаги в активном лотке) и не может продолжить текущую работу печати до тех пор, пока проблема не будет устранена. Дополнительные **сведения см.** в  дополнительных сведениях о значении (s) или значении описания.|
|unknownFutureValue|4 |Эволюционирующее значение sentinel. Не следует использовать.|

### <a name="printerprocessingstatedetail-values"></a>значения printerProcessingStateDetail

[тип enum printerProcessingStateDetail](./printerprocessingstatedetail.md)

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

