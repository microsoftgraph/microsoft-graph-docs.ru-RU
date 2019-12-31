---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2e61b4032e3d8c0976659cb34de2b043fac2ef8e
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913074"
---
# <a name="meetingparticipantinfo-resource-type"></a>Тип ресурса МитингпартиЦипантинфо

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
