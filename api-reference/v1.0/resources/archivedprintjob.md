---
title: Тип ресурса archivedPrintJob
description: Запись задания печати с окончательным состоянием (завершенным, прерванным или неудачным), которое используется для создания отчетов. Это не активное задание печати.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 90e694b0a6bd4019fd75f871b03bcc34d999df3a
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971387"
---
# <a name="archivedprintjob-resource-type"></a>Тип ресурса archivedPrintJob

Пространство имен: microsoft.graph

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
  "@odata.type": "#microsoft.graph.archivedPrintJob",   
  "id": "String (identifier)",  
  "printerId": "String",    
  "processingState": "String",  
  "createdDateTime": "String (timestamp)",  
  "acquiredDateTime": "String (timestamp)", 
  "completionDateTime": "String (timestamp)",   
  "acquiredByPrinter": "Boolean",   
  "copiesPrinted": "Integer",   
  "createdBy": {    
    "@odata.type": "microsoft.graph.userIdentity"   
  } 
}
```
