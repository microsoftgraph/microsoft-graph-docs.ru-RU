---
title: тип ресурса teamworkConversationIdentity
description: Представляет беседу в Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a463f37152b6d2108ac6ca04d9971cb908d6ba4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59055831"
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
|id|Строка|Унаследованный от [удостоверения](../resources/identity.md). ID беседы.|

## <a name="relationships"></a>Отношения
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

