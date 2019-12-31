---
title: Тип ресурса Коммснотификатионс
description: Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b5cbd2e2e2875a3e2ab207925a11fa258ad117f2
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913242"
---
# <a name="commsnotifications-resource-type"></a>Тип ресурса Коммснотификатионс

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
