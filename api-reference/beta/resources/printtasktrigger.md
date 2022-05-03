---
title: Тип ресурса printTaskTrigger
description: Определяет условия, при которых будет выполняться новый printTask на основе связанного printTaskDefinition.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 461a3ed348cfb0dc4329d641944ddf39f9e4a56d
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176347"
---
# <a name="printtasktrigger-resource-type"></a>Тип ресурса printTaskTrigger

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет условие, при котором будет активирован [новый printTask](printtask.md) на основе связанного [printTaskDefinition](printtaskdefinition.md).

Дополнительные сведения об использовании этого ресурса для добавления поддержки печати по запросу в универсальную печать см. в разделе "Расширение универсальной печати для [поддержки печати по запросу"](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/printer-list-tasktriggers.md) | [Коллекция printTaskTrigger](printtasktrigger.md) | Получение списка printTaskTriggers, связанных с определенным [принтером](printer.md). |
| [получение](../api/printtasktrigger-get.md); | [printTaskTrigger](printtasktrigger.md) | Получение определенного printTaskTrigger, связанного с определенным [принтером](printer.md).|


## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор printTaskTrigger. Только для чтения.|
|event|printEvent|Событие универсальной печати, которое приведет к активации [нового printTask](printtask.md) . Допустимые значения описаны в следующей таблице.|

### <a name="printevent-values"></a>значения printEvent

|Элемент|Значение|Описание|
|:---|:---|:---|
|jobStarted|0|Представляет событие, возникающее при запуске нового задания печати.|
|unknownFutureValue|1|Значение sentinel для развиваемого перечисления. Не следует использовать.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Определение|[printTaskDefinition](printtaskdefinition.md)|Абстрактное определение, которое будет использоваться для создания [printTask](printtask.md) при активации события печати. Только для чтения.|

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


