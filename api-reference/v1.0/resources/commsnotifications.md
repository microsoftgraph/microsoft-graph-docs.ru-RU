---
title: Тип ресурса Коммснотификатионс
description: Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c3d6ac676013509502dd7af0ddfee4c115aa523e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018972"
---
# <a name="commsnotifications-resource-type"></a>Тип ресурса Коммснотификатионс

Пространство имен: microsoft.graph

Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.

## <a name="properties"></a>Свойства

| Свойство       | Тип                                                 | Описание                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| значение          | Коллекция [коммснотификатион](commsnotification.md) | Уведомление об изменении ресурса. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

