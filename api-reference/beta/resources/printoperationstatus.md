---
title: Тип ресурса printOperationStatus
description: Представляет текущее состояние длительной операции универсальной печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 79cc94a38335bede616ef57bc33db12db63a5664
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176655"
---
# <a name="printoperationstatus-complex-type"></a>Сложный тип printOperationStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние длительной операции универсальной печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|state|printOperationProcessingState|Текущее состояние обработки printOperation. Допустимые значения описаны в следующей таблице. Только для чтения.|
|description|Строка|Понятное описание текущего состояния обработки printOperation. Только для чтения.|

### <a name="printoperationprocessingstate-values"></a>Значения printOperationProcessingState

|Элемент|Значение|Описание|
|:---|:---|:---|
|notStarted|0|Операция еще не запущена.|
|Запущена|1|Операция выполняется.|
|Удалось|2|Операция успешно завершена.|
|Сбой при|3|Сбой операции.|
|unknownFutureValue|4|Значение sentinel для развиваемого перечисления. Не следует использовать.|

## <a name="json-representation"></a>Представление JSON

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

