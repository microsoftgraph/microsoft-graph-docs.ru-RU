---
title: Тип ресурса Принттаскстатус
description: Представляет текущее состояние выполнения Принттаск.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5f340acf8357155893020985aa6036d93ed5b2df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078306"
---
# <a name="printtaskstatus-resource-type"></a>Тип ресурса Принттаскстатус

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние выполнения [принттаск](printtask.md). 

>**Примечание:** Приложения, которые регистрируют триггеры задач, несут ответственность за обновление состояния задач при завершении обработки, если соответствующее задание печати не было перенаправлено на другой принтер.

Дополнительные сведения о том, как использовать этот ресурс для поддержки печати по запросу в универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|state|принттаскпроцессингстате|Текущее состояние обработки [принттаск](printtask.md). Допустимые значения описаны в приведенной ниже таблице.|
|description|String|Удобное для человека описание текущего состояния обработки [принттаск](printtask.md).|

### <a name="printtaskprocessingstate-values"></a>значения Принттаскпроцессингстате

|Элемент|Значение|Описание|
|:---|:---|:---|
|закончен|нуль|Ожидание выполнения задачи.|
|двухпроцессорной|1 |Выполняется выполнение задачи.|
|готовы|2 |Выполнение задачи завершено.|
|прерван|4|Выполнение задачи было прервано.|
|unknownFutureValue|4 |Значение Sentinel для перечисления расширяемые. Не следует использовать.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskStatus"
}-->

```json
{
  "state": {"@odata.type": "microsoft.graph.printTaskProcessingState"},
  "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


