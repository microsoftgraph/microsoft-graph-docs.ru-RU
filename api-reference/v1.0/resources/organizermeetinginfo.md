---
title: тип ресурса organizerMeetingInfo
description: 'Содержит сведения об организаторе собрания. '
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fc97e94b2657273a55798528991762e43ec98023ba3e861f51a0e03d3d27f13f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178131"
---
# <a name="organizermeetinginfo-resource-type"></a>тип ресурса organizerMeetingInfo

Пространство имен: microsoft.graph

Содержит сведения об организаторе собрания. 

Чтобы присоединиться к существующему собранию, необходимо либо предоставить сочетание типов ресурсов organismeetingInfo и [chatInfo,](./chatinfo.md) либо тип [ресурсов tokenMeetingInfo](./tokenmeetinginfo.md) сам по себе.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                          | Описание                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| organizer                    | [identitySet](identityset.md) | Организатор Azure Active Directory удостоверение.  |

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

