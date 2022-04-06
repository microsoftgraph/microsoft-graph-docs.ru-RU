---
title: тип ресурса accessPackageAssignmentRequestorSettings
description: Используется для свойства requestorSettings политики назначения пакета доступа. Предоставляет дополнительные параметры, чтобы выбрать, кто может создать запрос.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d7a60166f60c2c5882872ed011722fbe14257462
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608380"
---
# <a name="accesspackageassignmentrequestorsettings-complex-type"></a>accessPackageAssignmentRequestorSettings сложный тип

Пространство имен: microsoft.graph

Используется для параметров запроса политики назначения [пакета доступа](accesspackageassignmentpolicy.md). Предоставляет дополнительные параметры, чтобы выбрать, кто может создать запрос на пакет доступа к этой политике и что они могут включить в свой запрос.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowCustomAssignmentSchedule|Boolean|Если `false`запросчику не разрешено включать расписание в свой запрос.|
|enableOnBehalfRequestorsToAddAccess|Boolean|Если `true`, позволяет от имени запрашивателей создать запрос, чтобы добавить доступ к другому принципу.|
|enableOnBehalfRequestorsToRemoveAccess|Boolean|Если `true`, позволяет от имени запрашивателей создать запрос на удаление доступа для другого основного.|
|enableOnBehalfRequestorsToUpdateAccess|Boolean|Если `true`, позволяет от имени запрашивателей создать запрос на обновление доступа для другого основного.|
|enableTargetsToSelfAddAccess|Boolean|Если `true`, позволяет запрашивателям создать запрос, чтобы добавить доступ для себя.|
|enableTargetsToSelfRemoveAccess|Boolean|Если `true`, позволяет запрашивателям создать запрос, чтобы удалить их доступ.|
|enableTargetsToSelfUpdateAccess|Boolean|Если `true`, позволяет запрашивателям создать запрос на обновление их доступа.|
|onBehalfRequestors|[коллекция subjectSet](../resources/subjectset.md)|Директора, которые могут запрашивать от имени других лиц.|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequestorSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequestorSettings",
  "enableTargetsToSelfAddAccess": "Boolean",
  "enableTargetsToSelfUpdateAccess": "Boolean",
  "enableTargetsToSelfRemoveAccess": "Boolean",
  "allowCustomAssignmentSchedule": "Boolean",
  "enableOnBehalfRequestorsToAddAccess": "Boolean",
  "enableOnBehalfRequestorsToUpdateAccess": "Boolean",
  "enableOnBehalfRequestorsToRemoveAccess": "Boolean",
  "onBehalfRequestors": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ]
}
```


