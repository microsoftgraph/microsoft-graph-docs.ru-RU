---
title: тип ресурса chatMessageFromIdentitySet
description: Представляет отправитель сообщения в чате или канале.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1f9b06063976e336a3e316c4ef5ca2c6ce9de622
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094423"
---
# <a name="chatmessagefromidentityset-resource-type"></a>тип ресурса chatMessageFromIdentitySet

Пространство имен: microsoft.graph

Представляет отправитель сообщения [в](../resources/chatmessage.md) чате или канале. Этот объект может быть для сообщения, которое было удалено или отправлено внутренней системой Microsoft Teams, например для сообщений событий для добавления `null` участников.


Наследует от [identitySet](../resources/identityset.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|application|[identity](../resources/identity.md)|Наследуется от [identitySet](../resources/identityset.md). При этом представляет приложение (например, бот), отправив сообщение.|
|device;|[identity](../resources/identity.md)|Наследуется от [identitySet](../resources/identityset.md). Не используется.|
|пользователь|[identity](../resources/identity.md)|Наследуется от [identitySet](../resources/identityset.md). Если присутствует, представляет пользователя, отправив сообщение.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageFromIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

