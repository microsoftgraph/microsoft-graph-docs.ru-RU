---
title: Тип ресурса printTaskStatus
description: Представляет текущее состояние выполнения printTask.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c484ef988e7452096d63fe103a6c45a8d22d06ff
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176332"
---
# <a name="printtaskstatus-resource-type"></a>Тип ресурса printTaskStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние выполнения [printTask](printtask.md). 

>**Примечание:** Приложения, которые регистрируют триггеры задач, отвечают за обновление состояний задач после завершения обработки, если связанное задание печати не было перенаправлено на другой принтер.

Дополнительные сведения об использовании этого ресурса для добавления поддержки печати по запросу в универсальную печать см. в разделе "Расширение универсальной печати для [поддержки печати по запросу"](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|state|printTaskProcessingState|Текущее состояние обработки [printTask](printtask.md). Допустимые значения описаны в следующей таблице.|
|description|Строка|Понятное описание текущего состояния обработки [printTask](printtask.md).|

### <a name="printtaskprocessingstate-values"></a>Значения printTaskProcessingState

|Элемент|Значение|Описание|
|:---|:---|:---|
|Ожидающие|0|Выполнение задачи ожидается.|
|Обработки|1|Выполняется задача.|
|Завершена|2|Выполнение задачи завершено.|
|Прервана|3|Выполнение задачи прервано.|
|unknownFutureValue|4|Значение sentinel для развиваемого перечисления. Не следует использовать.|

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


