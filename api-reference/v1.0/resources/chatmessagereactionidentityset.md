---
title: тип ресурса chatMessageReactionIdentitySet
description: Представляет пользователя, который реагировал на сообщение в чате или канале.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 35b97d1b7fe470beced8daca4b92f5e1c167b467
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109397"
---
# <a name="chatmessagereactionidentityset-resource-type"></a>тип ресурса chatMessageReactionIdentitySet

Пространство имен: microsoft.graph

Представляет **пользователя, который** реагировал на [сообщение](../resources/chatmessage.md) в чате или канале. Только `user` свойство имеет значение.


Наследует от [identitySet](../resources/identityset.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|application|[identity](../resources/identity.md)|Наследуется от [identitySet](../resources/identityset.md). Не установлено, так как приложения не могут реагировать на сообщения.|
|device;|[identity](../resources/identity.md)|Наследуется от [identitySet](../resources/identityset.md). Не установлено, так как устройства не могут реагировать на сообщения.|
|пользователь|[identity](../resources/identity.md)|Наследуется от [identitySet](../resources/identityset.md). Сведения о пользователе, который отреагировал на сообщение.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageReactionIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageReactionIdentitySet",
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

