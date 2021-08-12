---
title: тип ресурса chatMessageMentionedIdentitySet
description: Представляет ресурс, @mentioned в сообщении в чате или канале.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: bf19b34143935f66ab835cd12a47881bc0b1b1b2aa1f960d1d35f4be3d2ed41a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238155"
---
# <a name="chatmessagementionedidentityset-resource-type"></a>тип ресурса chatMessageMentionedIdentitySet

Пространство имен: microsoft.graph

Представляет ресурс (пользователь, приложение или беседа) @mentioned [в](../resources/chatmessage.md) сообщении в чате или канале.


Наследует от [identitySet](../resources/identityset.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|application|[identity](../resources/identity.md)|Наследуется от [identitySet](../resources/identityset.md). Если присутствует, представляет приложение (например, бот) @mentioned в [сообщении.](../resources/chatmessage.md)|
|conversation|[teamworkConversationIdentity](../resources/teamworkconversationidentity.md)|При этом представляет беседу (например, команду или канал) @mentioned в [сообщении.](../resources/chatmessage.md)|
|device;|[identity](../resources/identity.md)|Наследуется от [identitySet](../resources/identityset.md). Не используется, так как не поддерживается для @mention устройств.|
|пользователь|[identity](../resources/identity.md)|Наследуется от [identitySet](../resources/identityset.md). Если присутствует, представляет пользователя @mentioned в [сообщении](../resources/chatmessage.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMentionedIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageMentionedIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  },
  "conversation": {
    "@odata.type": "microsoft.graph.teamworkConversationIdentity"
  }
}
```