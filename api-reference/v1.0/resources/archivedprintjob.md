---
title: тип ресурса archivedPrintJob
description: Запись задания печати "окончательное состояние" (завершено, прервано или не выполнено) для отчетов. Это не активная работа печати.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2132b5a7cdf5024fb13845c57844220594ba6e1f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517965"
---
# <a name="archivedprintjob-resource-type"></a>тип ресурса archivedPrintJob

Пространство имен: microsoft.graph

Запись задания печати "окончательное состояние" (завершено, прервано или не выполнено) для отчетов. Это не активная работа печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|GUID архивного задания печати. Только для чтения.|
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