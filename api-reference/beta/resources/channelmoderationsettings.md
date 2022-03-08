---
title: тип ресурса channelModerationSettings
description: Используется для управления тем, кто может запускать новые сообщения и отвечать на сообщения в канале.
author: anandjo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 31538f7b5db717977490fa0b6e37749ef2787edd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337049"
---
# <a name="channelmoderationsettings-resource-type"></a>тип ресурса channelModerationSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В Microsoft Teams владельцы команд могут включить модерацию для канала, чтобы контролировать, кто может запускать новые сообщения и отвечать на сообщения в этом канале. Например, владельцам может потребоваться сделать следующее:

- Используйте канал только для объявлений.
- Используйте канал для обсуждений в группе классов, где только учитель может начать новые обсуждения.
- Используйте канал для проблем с livesite, где новые сообщения могут быть запущены соединиттелями.

По умолчанию `OFF`применяется умеренность, а это значит, что обычные параметры канала применяются к владельцам и членам команды с дополнительным контролем, позволяющим только членам группы или всем, включая гостей, запускать новую должность канала. Настройка модерации канала `ON` позволяет только модераторам запускать новые сообщения с дополнительным контролем для членов группы.

Поддержка параметров модерации каналов с помощью API Graph Microsoft:

- Члены группы должны иметь возможность запрашивать параметры модерации канала.
- Владельцы команд должны иметь возможность устанавливать параметры модерации канала.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowNewMessageFromBots|Boolean|Указывает, разрешено ли ботам отправлять сообщения.|
|allowNewMessageFromConnectors|Boolean|Указывает, разрешено ли соединитетелям отправлять сообщения.|
|replyRestriction|replyRestriction|Указывает, кому разрешено отвечать на канал команд. Возможные значения: `everyone`, `authorAndModerators`, `unknownFutureValue`.|
|userNewMessageRestriction|userNewMessageRestriction|Указывает, кому разрешено отправлять сообщения в командный канал. Возможные значения: `everyone`, `everyoneExceptGuests`, `moderators`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelModerationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelModerationSettings",
  "userNewMessageRestriction": "String",
  "replyRestriction": "String",
  "allowNewMessageFromBots": "Boolean",
  "allowNewMessageFromConnectors": "Boolean"
}
```

## <a name="see-also"></a>См. также

- Чтобы изменить параметры модерации канала, см. в примере 2 в [канале Update](../api/channel-patch.md).
