---
title: Тип ресурса Арчиведпринтжоб
description: Запись "конечного состояния" (выполненного, прерванного или неудачного) задания печати, используемого для создания отчетов. Это не активное задание печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: d4bd76dc84ad41c6d412144d13a784bec4f6a9f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050131"
---
# <a name="archivedprintjob-resource-type"></a>Тип ресурса Арчиведпринтжоб

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запись "конечного состояния" (выполненного, прерванного или неудачного) задания печати, используемого для создания отчетов. Это не активное задание печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Глобальный уникальный идентификатор (GUID) задания печати. Только для чтения.|
|принтерид|Строка|ИДЕНТИФИКАТОР принтера, для которого было задано задание в очереди. Только для чтения.|
|процессингстате|принтжобпроцессингстате|Последнее состояние обработки задания печати. Только для чтения.|
|createdDateTime|DateTimeOffset|Значение dateTimeOffset при создании задания. Только для чтения.|
|аккуиреддатетиме|DateTimeOffset|Значение dateTimeOffset, когда задание было получено принтером (при его наличии). Только для чтения.|
|комплетиондатетиме|DateTimeOffset|Значение dateTimeOffset, когда задание было завершено, отменено или прервано. Только для чтения.|
|аккуиредбипринтер|Boolean|Значение true, если задание было приобретено принтером; в противном случае — false. Только для чтения.|
|копиеспринтед|Int32|Число напечатанных копий. Только для чтения.|
|pageCount|Int32|Общее количество напечатанных страниц. Только для чтения.|
|блаккандвхитепажекаунт|Int32|Количество напечатанных черно-белых страниц. Только для чтения.|
|колорпажекаунт|Int32|Число напечатанных страниц цветов. Только для чтения.|
|симплекспажекаунт|Int32|Число напечатанных страниц симплекс (односторонняя). Только для чтения.|
|дуплекспажекаунт|Int32|Число отпечатанных дуплексных страниц (двусторонних). Только для чтения.|
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

