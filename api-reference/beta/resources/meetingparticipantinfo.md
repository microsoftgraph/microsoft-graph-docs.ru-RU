---
title: Тип ресурса meetingParticipantInfo
description: Сведения об участнике собрания.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2222c32db1f4dcee27fb4e3c88100d5e32788f60
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883868"
---
# <a name="meetingparticipantinfo-resource-type"></a>Тип ресурса meetingParticipantInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о участнике собрания.

## <a name="properties"></a>Свойства

| Свойство | Тип             | Описание                 |
| :------- | :-------------------- | :------------------------------ |
| Идентичности | [identitySet](identityset.md) | Сведения об удостоверении участника.           |
| Upn      | String                        | Имя участника-пользователя.             |
| role     | [onlineMeetingRole](#onlinemeetingrole-values)     | Указывает роль участника в собрании.|

### <a name="onlinemeetingrole-values"></a>Значения onlineMeetingRole

В следующей таблице перечислены элементы [развиваемого перечисления](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations). Чтобы получить значение `Prefer: include-unknown-enum-members` `coorganizer` в этом развиваемом перечислении, необходимо использовать заголовок запроса.

| Значение              | Описание                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| attendee            | Участник является участником. Это значение применяется ко всем собраниям.   |
| Ведущий           | Роль участника — выступающий. Это значение применяется к собраниям с **разрешенным атрибутом AllowedPresenter** `roleIsPresenter`или трансляции Teams. |
| Производитель            | Роль участника — производитель. Это значение относится только к трансляции Teams.  |
| соорганизатор | Роль участника является со организатором. Это значение применяется ко всем собраниям, кроме трансляции Teams. |
| unknownFutureValue | Значение sentinel для развиваемого перечисления. Не следует использовать. |

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


