---
title: Тип ресурса Организермитингинфо
description: 'Содержит сведения об организаторе собрания. '
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 210dfecb6252091663aeb981fcf82e2b3535dcac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998427"
---
# <a name="organizermeetinginfo-resource-type"></a>Тип ресурса Организермитингинфо

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения об организаторе собрания. 

Чтобы присоединиться к существующему собранию, необходимо либо указать сочетание типов ресурсов Организермитингинфо и [чатинфо](./chatinfo.md) , либо сам тип ресурса [токенмитингинфо](./tokenmeetinginfo.md) .

## <a name="properties"></a>Свойства

| Свойство                     | Тип                          | Описание                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| organizer                    | [identitySet](identityset.md) | Удостоверение Azure Active Directory для организатора.  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


