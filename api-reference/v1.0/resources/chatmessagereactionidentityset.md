---
title: тип ресурса chatMessageReactionIdentitySet
description: Представляет пользователя, который реагировал на сообщение в чате или канале.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 59b1e110f5d74fdf4883cf7e59adfe5aacdf8b88fcd6e5e6da5728cc2e948f9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189891"
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

## <a name="relationships"></a>Связи
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

