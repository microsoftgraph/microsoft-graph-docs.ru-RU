---
title: Тип ресурса Принтоператионстатус
description: Представляет текущее состояние длительной универсальной операции печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 14c66cf59dc1715a16bd786657202a554d7c1753
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052553"
---
# <a name="printoperationstatus-complex-type"></a>сложный тип Принтоператионстатус

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние длительной универсальной операции печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|state|принтоператионпроцессингстате|Текущее состояние обработки Принтоператион. Допустимые значения описаны в приведенной ниже таблице. Только для чтения.|
|description|String|Удобное для человека описание текущего состояния обработки Принтоператион. Только для чтения.|

### <a name="printoperationprocessingstate-values"></a>значения Принтоператионпроцессингстате

|Элемент|Значение|Описание|
|:---|:---|:---|
|notStarted|нуль|Операция еще не запущена.|
|запускается|1 |Выполняется операция.|
|закончил|2 |Операция успешно завершена.|
|сбоев|4|Сбой операции.|
|unknownFutureValue|4 |Значение Sentinel для перечисления расширяемые. Не следует использовать.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperationStatus"
}-->

```json
{
    "state": "String",
    "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

