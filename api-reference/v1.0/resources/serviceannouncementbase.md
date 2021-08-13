---
title: тип ресурса serviceAnnouncementBase
description: Это абстрактный базовый тип для serviceHealthIssue и serviceUpdateMessage.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 5e1c8783615645461d3dc7bafdb403e52c94cf4bebd3f7e8cc5d6bbd3d1aec0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54195613"
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
|подробности|[Коллекция(keyValuePair)](../resources/keyvaluepair.md)|Дополнительные сведения о событии службы. Это свойство не поддерживает фильтры.|
|endDateTime|DateTimeOffset|Конечное время события службы.|
|id|String|Id события службы.|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время события службы.|
|startDateTime|DateTimeOffset|Время начала события службы.|
|title|String|Название события службы.|

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