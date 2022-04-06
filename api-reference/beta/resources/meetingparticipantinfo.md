---
title: тип ресурса meetingParticipantInfo
description: Сведения о участнике собрания.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5d3f8e5fb055fa45ef150aa9ef7eef82980d0755
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63668586"
---
# <a name="meetingparticipantinfo-resource-type"></a>тип ресурса meetingParticipantInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о участнике собрания.

## <a name="properties"></a>Свойства

| Свойство | Тип             | Описание                 |
| :------- | :-------------------- | :------------------------------ |
| удостоверение | [identitySet](identityset.md) | Сведения о удостоверениях участника.           |
| upn      | Строка                        | Основное имя участника пользователя.             |
| role     | [onlineMeetingRole](#onlinemeetingrole-values)     | Указывает роль участника собрания.|

### <a name="onlinemeetingrole-values"></a>значения onlineMeetingRole

В следующей таблице перечислены участники [развивающегося перечисления](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations). Чтобы получить значение `Prefer: include-unknown-enum-members` `coorganizer` в этом развиваемом переуме, необходимо использовать заглавную заготку запроса.

| Значение              | Описание                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| attendee            | Роль участника — участник. Это значение применяется ко всем собраниям.   |
| presenter           | Роль участника — презентер. Это значение применимо к собраниям с разрешенным **значениемPresenter** `roleIsPresenter`или Teams в прямом эфире. |
| производитель            | Роль участника — продюсер. Это значение применяется только к Teams событию.  |
| coorganizer | Роль участника является соорганизатором. Это значение применимо ко всем собраниям, кроме Teams события в прямом эфире. |
| unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать. |

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


