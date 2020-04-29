---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cdd0bb125fd8b84177b1370bca633f6d9ae5bb87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534264"
---
# <a name="meetingparticipantinfo-resource-type"></a>Тип ресурса МитингпартиЦипантинфо

Пространство имен: microsoft.graph

Сведения о участниках собрания.

## <a name="properties"></a>Свойства

| Свойство       | Тип                          | Описание                              |
|:---------------|:------------------------------|:-----------------------------------------|
| хищения       | [identitySet](identityset.md) | Сведения об удостоверении участника. |
| Основное            | String                        | Имя участника пользователя.  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
