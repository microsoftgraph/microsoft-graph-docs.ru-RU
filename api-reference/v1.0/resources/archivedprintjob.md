---
title: тип ресурса archivedPrintJob
description: Запись задания печати "окончательное состояние" (завершено, прервано или не выполнено) для отчетов. Это не активная работа печати.
author: nilakhan
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 9f6818801a12eb635a86350432108d3d0e3b6332
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109523"
---
# <a name="archivedprintjob-resource-type"></a>тип ресурса archivedPrintJob

Пространство имен: microsoft.graph

Запись задания печати "окончательное состояние" (завершено, прервано или не выполнено) для отчетов. Это не активная работа печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|GUID архивного задания печати. Только для чтения.|
|printerId|Строка|ID принтера, для работы в очереди. Только для чтения.|
|processingState|printJobProcessingState|Окончательное состояние обработки задания печати. Только для чтения.|
|createdDateTime|DateTimeOffset|DateTimeOffset, когда было создано задание. Только для чтения.|
|acquiredDateTime|DateTimeOffset|DateTimeOffset, когда задание было приобретено принтером, если таково. Только для чтения.|
|completionDateTime|DateTimeOffset|DateTimeOffset, когда задание было завершено, отменено или прервано. Только для чтения.|
|acquiredByPrinter|Логический|True, если задание было приобретено принтером; false в противном случае. Только для чтения.|
|copiesPrinted|Int32|Количество напечатанных копий. Только для чтения.|
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
