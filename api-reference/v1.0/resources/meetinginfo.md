---
title: тип ресурса meetingInfo
description: Сведения о собраниях, заданные для создания собрания или перейти к нему.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0df2c90c8600fea2b00cf465c17682714b0c8a6e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134593"
---
# <a name="meetinginfo-resource-type"></a>тип ресурса meetingInfo

Пространство имен: microsoft.graph

Это абстрактный класс, содержащий сведения о собраниях.
 
Чтобы присоединиться к существующему собранию, необходимо либо указать [организаторMeetingInfo](organizermeetinginfo.md) в сочетании с [chatInfo,](./chatinfo.md)либо [просто tokenMeetingInfo](tokenmeetinginfo.md).


## <a name="derived-types"></a>Производные типы

| Тип                                                 | Описание                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [organizerMeetingInfo](./organizermeetinginfo.md)    | Сведения об организаторе собрания                          |
| [tokenMeetingInfo](tokenmeetinginfo.md)              | Зашифрованный маркер, содержащий сведения о собрании  |

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

