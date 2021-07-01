---
title: тип ресурса chatMessageReactionIdentitySet
description: Представляет пользователя, который реагировал на сообщение в чате или канале.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 086cca8963bbb019ab7754a6aba3b644a5e14e2e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211119"
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
|user|[identity](../resources/identity.md)|Наследуется от [identitySet](../resources/identityset.md). Сведения о пользователе, который отреагировал на сообщение.|

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

