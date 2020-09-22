---
title: Тип ресурса Принттасктригжер
description: Определяет условия, при которых новый Принттаск будет выполняться на основе связанного Принттаскдефинитион.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fc05fe9011d91ac9da5f74a6079537ebfba25160
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078294"
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
| [получение](../api/printtasktrigger-get.md); | [printTaskTrigger](printtasktrigger.md) | Получение Принттасктригжер, связанного с определенным [принттаск](printtask.md). |


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

## <a name="relationships"></a>Отношения
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|RDLC|[printTaskDefinition](printtaskdefinition.md)|Абстрактное определение, которое будет использоваться для создания объекта [принттаск](printtask.md) при запуске события Print. Только для чтения.|

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


