---
title: Тип ресурса archivedPrintJob
description: Запись задания печати с окончательным состоянием (завершенным, прерванным или неудачным), которое используется для создания отчетов. Это не активное задание печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 8ba8d49a01e3b10768e83b04b259d6cfd87d65b5
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944978"
---
# <a name="archivedprintjob-resource-type"></a>Тип ресурса archivedPrintJob

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запись задания печати с окончательным состоянием (завершенным, прерванным или неудачным), которое используется для создания отчетов. Это не активное задание печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|GUID архивного задания печати. Только для чтения.|
|printerId|Строка|Идентификатор принтера, для которого задание поставлено в очередь. Только для чтения.|
|processingState|printJobProcessingState|Конечное состояние обработки задания печати. Только для чтения.|
|createdDateTime|DateTimeOffset|DateTimeOffset при создании задания. Только для чтения.|
|acquiredDateTime|DateTimeOffset|DateTimeOffset, когда задание было приобретено принтером, если таковое есть. Только для чтения.|
|completionDateTime|DateTimeOffset|DateTimeOffset, когда задание было завершено, отменено или прервано. Только для чтения.|
|acquiredByPrinter|Boolean|Значение true, если задание было приобретено принтером; Значение false в противном случае. Только для чтения.|
|copiesPrinted|Int32|Количество выпечатаемых копий. Только для чтения.|
|Pagecount|Int32|Общее количество страниц, которые были напечатаны. Только для чтения.|
|blackAndWhitePageCount|Int32|Количество напечатаемых черно-белых страниц. Только для чтения.|
|colorPageCount|Int32|Количество цветовых страниц, которые были напечатаны. Только для чтения.|
|simplexPageCount|Int32|Количество печатаемых простых (однобоких) страниц. Только для чтения.|
|duplexPageCount|Int32|Количество двустороннего (двустороннего) страниц, которые были напечатаны. Только для чтения.|
|createdBy|[userIdentity](useridentity.md)|Пользователь, создавший задание печати. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.archivedPrintJob"
}-->

```json
{
    "id": "String (identifier)",
    "printer": {"@odata.type": "microsoft.graph.directoryObject"},
    "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
    "processingState": {"@odata.type": "microsoft.graph.printJobProcessingState"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "archivedPrintJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

