---
title: Тип ресурса Принттасктригжер
description: Определяет условия, при которых новый Принттаск будет выполняться на основе связанного Принттаскдефинитион.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0a9ca4d06f43c9dd0964f0bb4c9614bfb4a78c1e
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091696"
---
# <a name="printtasktrigger-resource-type"></a>Тип ресурса Принттасктригжер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет условие, при котором новый [принттаск](printtask.md) будет запускаться на основе связанного [принттаскдефинитион](printtaskdefinition.md).

Дополнительные сведения о том, как использовать этот ресурс для поддержки печати по запросу в универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/printer-list-tasktriggers.md) | Коллекция [принттасктригжер](printtasktrigger.md) | Получение списка Принттасктригжерс, связанных с определенным [принтером](printer.md). |
| [Get](../api/printtasktrigger-get.md) | [принттасктригжер](printtasktrigger.md) | Получение Принттасктригжер, связанного с определенным [принттаск](printtask.md). |


## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор Принттасктригжер. Только для чтения.|
|event|принтевент|Универсальное событие печати, которое вызывает срабатывание нового [принттаск](printtask.md) . Допустимые значения описаны в приведенной ниже таблице.|

### <a name="printevent-values"></a>значения Принтевент

|Элемент|Значение|Описание|
|:---|:---|:---|
|жобстартед|нуль|Представляет событие, возникающее при запуске нового задания печати.|
|unknownFutureValue|1 |Значение Sentinel для перечисления расширяемые. Не следует использовать.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|RDLC|[принттаскдефинитион](printtaskdefinition.md)|Абстрактное определение, которое будет использоваться для создания объекта [принттаск](printtask.md) при запуске события Print. Только для чтения.|

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
