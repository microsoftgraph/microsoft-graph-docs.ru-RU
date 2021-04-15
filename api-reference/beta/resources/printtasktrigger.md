---
title: тип ресурса printTaskTrigger
description: Определяет условия, при которых будет выполнен новый printTask на основе связанного печатиTaskDefinition.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: de2da4f94894d9744fdfdd302b310251cd91fdb3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766324"
---
# <a name="printtasktrigger-resource-type"></a>тип ресурса printTaskTrigger

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет условие, при котором будет запускаться новый [printTask](printtask.md) на основе связанного с ним [принтаTaskDefinition.](printtaskdefinition.md)

Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/printer-list-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) collection | Получите список printTaskTriggers, связанных с определенным [принтером.](printer.md) |
| [Get](../api/printtasktrigger-get.md) | [printTaskTrigger](printtasktrigger.md) | Получите определенный шрифтTaskTrigger, связанный с определенным [принтером.](printer.md)|


## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор printTaskTrigger. Только для чтения.|
|event|printEvent|Событие Universal Print, которое приведет к запуску новой [печатиTask.](printtask.md) Допустимые значения описаны в следующей таблице.|

### <a name="printevent-values"></a>printEvent values

|Элемент|Значение|Описание|
|:---|:---|:---|
|jobStarted|0|Представляет событие, которое происходит при работе с новой печатью.|
|unknownFutureValue|1|Эволюционирующее значение sentinel. Не следует использовать.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|определение|[printTaskDefinition](printtaskdefinition.md)|Абстрактное определение, которое будет использоваться для создания [printTask](printtask.md) при запуске события печати. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "event": {"@odata.type": "microsoft.graph.printEvent"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


