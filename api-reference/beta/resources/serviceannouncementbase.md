---
title: тип ресурса serviceAnnouncementBase
description: Это абстрактный базовый тип для serviceHealthIssue и serviceUpdateMessage.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 46e1e6428d1371683a8ad1febae990146a9fe898
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109241"
---
# <a name="serviceannouncementbase-resource-type"></a>тип ресурса serviceAnnouncementBase

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Это абстрактный базовый тип [для serviceHealthIssue](../resources/servicehealthissue.md) и [serviceUpdateMessage.](../resources/serviceupdatemessage.md)

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|подробности|[Коллекция(keyValuePair)](../resources/keyvaluepair.md)|Дополнительные сведения о событии службы. Это свойство не поддерживает фильтры.|
|endDateTime|DateTimeOffset|Конечное время события службы.|
|id|Строка|Id события службы.|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время события службы.|
|startDateTime|DateTimeOffset|Время начала события службы.|
|title|Строка|Название события службы.|

## <a name="relationships"></a>Отношения
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