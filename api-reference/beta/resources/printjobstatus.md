---
title: Тип ресурса printJobStatus
description: Представляет текущее состояние задания печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 73038bbea54860ef37b8ebbf2602450dc556efd2
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176677"
---
# <a name="printjobstatus-resource-type"></a>Тип ресурса printJobStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние задания печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|state|printJobProcessingState|Текущее состояние обработки задания печати. Допустимые значения описаны в следующей таблице. Только для чтения.|
|details|Коллекция printJobProcessingDetail|Дополнительные сведения о состоянии задания печати. Допустимые значения описаны в следующей таблице. Только для чтения.|
|description|Строка|Понятное описание текущего состояния обработки задания печати. Только для чтения.|
|isAcquiredByPrinter|Логическое|Значение true, если задание было подтверждено принтером; Значение false в противном случае. Только для чтения.|

### <a name="printjobprocessingstate-values"></a>Значения printJobProcessingState

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние обработки, сообщаемое принтером, не распознается.|
|Ожидающие|1|Задание печати ожидает обработки принтером.|
|Обработки|2|Задание печати в настоящее время обрабатывается принтером.|
|Приостановлена|3|Задание печати приостановлено.|
|Остановился|4|Задание печати остановлено, так как перед продолжением задания необходимо устранить проблему с принтером. Дополнительные сведения можно найти в ресурсе состояния принтера.|
|Завершена|5|Задание печати успешно завершено, и дальнейшая обработка не выполняется.|
|Отменен|6 |Задание печати отменено пользователем, и дальнейшая обработка не выполняется.|
|Прервана|7 |Задание печати прервано пользователем или принтером, и дальнейшая обработка не выполняется.|

### <a name="printjobprocessingdetail-values"></a>Значения printJobProcessingDetail

|Элемент|Значение|Описание|
|:---|:---|:---|
|uploadPending|0|Полезные данные документа не были отправлены.|
|Преобразования|1|Полезные данные документа преобразуются.|
|completedSuccessfully|2|Задание успешно завершено.|
|completedWithWarnings|3|Задание завершено с предупреждениями.|
|completedWithErrors|4|Задание завершено с ошибками.|
|releaseWait|5|Задание ожидает освобождения.|
|Интерпретации|6 |Задание находится в состоянии обработки, но, в частности, полезные данные документа интерпретируются.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobStatus"
}-->

```json
{
    "state": "String",
    "description": "String",
    "isAcquiredByPrinter": true,    
    "details": ["String"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJobStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

