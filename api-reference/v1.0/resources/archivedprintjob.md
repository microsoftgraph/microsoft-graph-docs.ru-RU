---
title: Тип ресурса archivedPrintJob
description: Запись задания печати "конечное состояние" (завершенное, прерванное или отмененное), которое используется для создания отчетов. Это не активное задание печати".
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d6f9922dfbd50b347f38959a94f36520f425f2d9
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160610"
---
# <a name="archivedprintjob-resource-type"></a>Тип ресурса archivedPrintJob

Пространство имен: microsoft.graph

Запись задания печати "конечное состояние" (завершенное, прерванное или отмененное), которое используется для создания отчетов. Это не активное задание печати.

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
