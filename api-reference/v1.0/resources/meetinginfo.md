---
title: тип ресурса meetingInfo
description: Сведения о собраниях, заданные для создания собрания или перейти к нему.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab866ada9fa4b886cbd90cb999132ff13b48d74437f11710a43aee31ba7857fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126412"
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

