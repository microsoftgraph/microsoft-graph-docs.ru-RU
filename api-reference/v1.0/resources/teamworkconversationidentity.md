---
title: тип ресурса teamworkConversationIdentity
description: Представляет беседу в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1bf17f9954459a1e476106315db60f65dc536b02
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211137"
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

