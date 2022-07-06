---
title: Тип ресурса joinMeetingIdMeetingInfo
description: Содержит сведения, позволяющие присоединиться к существующему собранию с помощью joinMeetingId и секретного кода.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a35dff2db37686bae85a52d47a4b1f1aa3a10ff0
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645711"
---
# <a name="joinmeetingidmeetinginfo-resource-type"></a>Тип ресурса joinMeetingIdMeetingInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения, позволяющие присоединиться к существующему собранию с **помощью joinMeetingId** и секретного **кода** (при необходимости). Эти свойства можно получить из [API Get onlineMeeting](../api/onlinemeeting-get.md) .

Наследуется [от meetingInfo](../resources/meetinginfo.md).

## <a name="properties"></a>Свойства

| Свойство                | Тип    | Описание                                                   |
| :---------------------- | :------ | :------------------------------------------------------------ |
| joinMeetingId           | String  | Идентификатор, используемый для присоединения к собранию.                              |
| passcode                | String  | Секретный код, используемый для присоединения к собранию. Необязательное.              |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.joinMeetingIdMeetingInfo"
}-->
```json
{
    "joinMeetingId": "String",
    "passcode": "String"
}
```
