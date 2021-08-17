---
title: тип ресурса serviceAnnouncementBase
description: Это абстрактный базовый тип для serviceHealthIssue и serviceUpdateMessage.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: f5f1beb5918833703fbbff48ba991b850bcd1ceb
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266907"
---
# <a name="serviceannouncementbase-resource-type"></a>тип ресурса serviceAnnouncementBase

Пространство имен: microsoft.graph

Это абстрактный базовый тип [для serviceHealthIssue](../resources/servicehealthissue.md) и [serviceUpdateMessage.](../resources/serviceupdatemessage.md)

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
Отсутствуют.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|details|[Коллекция(keyValuePair)](../resources/keyvaluepair.md)|Дополнительные сведения о событии службы. Это свойство не поддерживает фильтры.|
|endDateTime|DateTimeOffset|Конечное время события службы.|
|id|String|Id события службы.|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время события службы.|
|startDateTime|DateTimeOffset|Время начала события службы.|
|title|Строка|Название события службы.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncementBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncementBase",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```