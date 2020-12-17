---
title: Тип ресурса channelModerationSettings
description: Используется для управления тем, кто может запускать новые записи и отвечать на них в канале.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2de1c16ed998a0b793d14c6a4d791613e0bef62
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706373"
---
# <a name="channelmoderationsettings-resource-type"></a>Тип ресурса channelModerationSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В Microsoft Teams владельцы команд могут включить модерацию для канала, чтобы контролировать, кто может запускать новые записи и отвечать на публикации в этом канале. Например, владельцам может потребоваться сделать следующее:

- Используйте канал только для объявлений.
- Используйте канал для обсуждений в команде класса, где только преподаватель может начинать новые обсуждения.
- Используйте канал для проблем с сайтами, в которых соединители могут начать новые публикации.

По умолчанию модерация — это означает, что обычные параметры канала применяются к владельцам и участникам команды с дополнительным контролем, чтобы разрешить только членам команды или всем, включая гостей, запускать новую публикацию `OFF` канала. Настройка модерации канала, позволяющая только модераторам запускать новые записи с дополнительным контролем `ON` для участников команды.

Для поддержки параметров модерации каналов с помощью API Microsoft Graph:

- Участники группы должны иметь возможность запрашивать параметры модерации канала.
- Владельцы команд должны иметь возможность настраивать параметры модерации каналов.

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
