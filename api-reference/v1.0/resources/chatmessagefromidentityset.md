---
title: тип ресурса chatMessageFromIdentitySet
description: Представляет отправитель сообщения в чате или канале.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 58f5654dc8019950134c25cdc50529b29032d8870462d46a46481b489f4ba15a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192581"
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

## <a name="relationships"></a>Связи
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

