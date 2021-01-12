---
title: Тип ресурса channelModerationSettings
description: Используется для управления тем, кто может запускать новые записи и отвечать на них в канале.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b67d55eb57d1a4b554b027270f700cbd590d4416
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796586"
---
# <a name="channelmoderationsettings-resource-type"></a>Тип ресурса channelModerationSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В Microsoft Teams владельцы команд могут включить модерацию для канала, чтобы контролировать, кто может запускать новые записи и отвечать на публикации в этом канале. Например, владельцам может потребоваться сделать следующее:

- Используйте канал только для объявлений.
- Используйте канал для обсуждений в группе класса, где только преподаватель может начинать новые обсуждения.
- Используйте канал для проблем с сайтами, в которых соединители могут начать новые публикации.

По умолчанию модерация — это означает, что обычные параметры канала применяются к владельцам и участникам команды с дополнительным контролем, чтобы разрешить только участникам команды или всем, включая гостей, запускать новую публикацию `OFF` канала. Настройка модерации канала, позволяющая только модераторам запускать новые записи с дополнительным контролем `ON` для участников группы.

Для поддержки параметров модерации каналов с помощью API Microsoft Graph:

- Участники группы должны иметь возможность запрашивать параметры модерации канала.
- Владельцы команд должны иметь возможность устанавливать параметры модерации каналов.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowNewMessageFromBots|Логический|Указывает, разрешено ли ботам размещать сообщения.|
|allowNewMessageFromConnectors|Логический|Указывает, разрешено ли соединитетелям отправлять сообщения.|
|replyRestriction|replyRestriction|Указывает, кому разрешено отвечать на канал teams. Возможные значения: `everyone`, `authorAndModerators`, `unknownFutureValue`.|
|userNewMessageRestriction|userNewMessageRestriction|Указывает, кому разрешено отправлять сообщения в канал Teams. Возможные значения: `everyone`, `everyoneExceptGuests`, `moderators`, `unknownFutureValue`.|

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

- Чтобы изменить параметры модерации канала, см. пример 2 в [канале Update.](../api/channel-patch.md)
