---
title: тип ресурса organizerMeetingInfo
description: 'Содержит сведения об организаторе собрания. '
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d39f12a611756836249bc6b5abc81e91e29db7c3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032267"
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

