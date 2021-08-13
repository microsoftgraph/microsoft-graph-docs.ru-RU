---
title: тип ресурса teamworkConversationIdentity
description: Представляет беседу в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fe6315b6546d603c203fad878c291f61e1f8394fc56acba4cfdf788ee86a2856
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249113"
---
# <a name="teamworkconversationidentity-resource-type"></a>тип ресурса teamworkConversationIdentity

Пространство имен: microsoft.graph

Представляет **беседу (чат,** команду или канал) в Microsoft Teams.

Наследует от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|conversationIdentityType|teamworkConversationIdentityType|Тип беседы. Возможные значения: `team`, `channel`, `chat` и `unknownFutureValue`.|
|displayName|String|Унаследованный от [удостоверения](../resources/identity.md). Отображение имени беседы. Необязательно.|
|id|String|Унаследованный от [удостоверения](../resources/identity.md). ID беседы.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConversationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConversationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "conversationIdentityType": "String"
}
```

