---
title: Тип ресурса meetingParticipantInfo
description: Сведения об участнике собрания.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d46f15a86742a23b6ec4e9f6c270308de34c169c
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883987"
---
# <a name="meetingparticipantinfo-resource-type"></a>Тип ресурса meetingParticipantInfo

Пространство имен: microsoft.graph

Сведения об участнике собрания.

## <a name="properties"></a>Свойства

| Свойство | Тип                          | Описание                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| Идентичности | [identitySet](identityset.md) | Сведения об удостоверении участника.                                            |
| Upn      | String                        | Имя участника-пользователя.                                             |
| role     | onlineMeetingRole             | Указывает роль участника в собрании.  Возможные значения: `attendee`, `presenter`и `producer``unknownFutureValue`.|

> [!TIP]
>
> Чтобы задать **роль** докладчика участника собрания при создании или обновлении [onlineMeeting](onlinemeeting.md), необходимо также задать значение **allowedPresenters**`roleIsPresenter`.

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

