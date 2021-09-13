---
title: тип ресурса serviceAnnouncementBase
description: Это абстрактный базовый тип для serviceHealthIssue и serviceUpdateMessage.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 8ea4ddaed2a3ea67833be103da58f703957f2373
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019141"
---
# <a name="serviceannouncementbase-resource-type"></a>тип ресурса serviceAnnouncementBase

Пространство имен: microsoft.graph

Это абстрактный базовый тип [для serviceHealthIssue](../resources/servicehealthissue.md) и [serviceUpdateMessage.](../resources/serviceupdatemessage.md)

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
Нет.

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
