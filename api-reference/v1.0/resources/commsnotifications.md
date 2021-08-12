---
title: тип ресурса commsNotifications
description: Список уведомлений, используемых серверами связи для отправки нескольких уведомлений в одной партии.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ec5a1cd338a0b774f93096172dc4940defcec4efb59615172918667ddd82f8f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235704"
---
# <a name="commsnotifications-resource-type"></a>тип ресурса commsNotifications

Пространство имен: microsoft.graph

Список уведомлений, используемых серверами связи для отправки нескольких уведомлений в одной партии.

## <a name="properties"></a>Свойства

| Свойство       | Тип                                                 | Описание                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| значение          | [коллекция commsNotification](commsnotification.md) | Уведомление об изменении ресурса. |

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

