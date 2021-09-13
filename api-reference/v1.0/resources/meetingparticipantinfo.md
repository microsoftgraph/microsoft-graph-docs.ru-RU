---
title: тип ресурса meetingParticipantInfo
description: Сведения о участнике собрания.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 505a31673ea110f899b37b7d6404b5020ed6d88e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113653"
---
# <a name="meetingparticipantinfo-resource-type"></a>тип ресурса meetingParticipantInfo

Пространство имен: microsoft.graph

Сведения о участнике собрания.

## <a name="properties"></a>Свойства

| Свойство | Тип                          | Описание                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| удостоверение | [identitySet](identityset.md) | Сведения о удостоверениях участника.                                            |
| upn      | String                        | Основное имя участника пользователя.                                             |
| role     | onlineMeetingRole             | Указывает роль участника собрания.  Возможные значения `attendee` , `presenter` и `producer` `unknownFutureValue` .|

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
  "upn": "String",
  "role": "String"
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

