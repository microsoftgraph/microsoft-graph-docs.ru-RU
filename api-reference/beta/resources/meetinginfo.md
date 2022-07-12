---
title: Тип ресурса meetingInfo
description: Сведения о собрании, указанные для создания или присоединения к собранию.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d7aebdbd0236f0c1223e295456d408f37fb0708e
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731598"
---
# <a name="meetinginfo-resource-type"></a>Тип ресурса meetingInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Это абстрактный класс, содержащий сведения о собрании.
 
Чтобы присоединиться к существующему собранию, необходимо указать [organizerMeetingInfo](organizermeetinginfo.md) в сочетании с [chatInfo](./chatinfo.md), [tokenMeetingInfo](tokenmeetinginfo.md) или [joinMeetingIdMeetingInfo](joinmeetingidmeetinginfo.md).


## <a name="derived-types"></a>Производные типы

| Тип                                                    | Описание                                                         |
|:--------------------------------------------------------|:--------------------------------------------------------------------|
| [joinMeetingIdMeetingInfo](joinmeetingidmeetinginfo.md) | Содержит **идентификатор joinMeetingId** **и секретный код** собрания.     |
| [organizerMeetingInfo](./organizermeetinginfo.md)       | Сведения об организаторе собрания.                         |
| [TokenMeetingInfo](tokenmeetinginfo.md)                 | Зашифрованный маркер, содержащий сведения о собрании. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


