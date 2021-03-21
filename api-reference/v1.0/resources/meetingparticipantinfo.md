---
title: тип ресурса meetingParticipantInfo
description: Сведения о участнике собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 40209354f1621839bd51a20fcbafa4cd58b4fd8d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962457"
---
# <a name="meetingparticipantinfo-resource-type"></a>тип ресурса meetingParticipantInfo

Пространство имен: microsoft.graph

Сведения о участнике собрания.

## <a name="properties"></a>Свойства

| Свойство | Тип                          | Описание                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| identity | [identitySet](identityset.md) | Сведения о удостоверениях участника.                                            |
| upn      | String                        | Основное имя участника пользователя.                                             |
| role     | onlineMeetingRole             | Указывает роль участника собрания.  Возможные значения: `attendee`, `presenter` и `unknownFutureValue`.|

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

