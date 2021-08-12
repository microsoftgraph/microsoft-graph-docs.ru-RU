---
title: тип ресурса archivedPrintJob
description: Запись задания печати "окончательное состояние" (завершено, прервано или не выполнено) для отчетов. Это не активная работа печати.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 45d1988e95661f586b4093b5ff033197b623b891ae5e78e59a57352c406f4085
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163910"
---
# <a name="archivedprintjob-resource-type"></a>тип ресурса archivedPrintJob

Пространство имен: microsoft.graph

Запись задания печати "окончательное состояние" (завершено, прервано или не выполнено) для отчетов. Это не активная работа печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|GUID архивного задания печати. Только для чтения.|
|printerId|String|ID принтера, для работы в очереди. Только для чтения.|
|processingState|printJobProcessingState|Окончательное состояние обработки задания печати. Только для чтения.|
|createdDateTime|DateTimeOffset|DateTimeOffset, когда было создано задание. Только для чтения.|
|acquiredDateTime|DateTimeOffset|DateTimeOffset, когда задание было приобретено принтером, если таково. Только для чтения.|
|completionDateTime|DateTimeOffset|DateTimeOffset, когда задание было завершено, отменено или прервано. Только для чтения.|
|acquiredByPrinter|Логическое|True, если задание было приобретено принтером; false в противном случае. Только для чтения.|
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