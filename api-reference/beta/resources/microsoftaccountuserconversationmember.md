---
title: тип ресурса microsoftAccountUserConversationMember
description: Представляет личного пользователя учетной записи Майкрософт в чате.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6d68d9bf9aa32bbb0965f5a892cd923627266c8e
ms.sourcegitcommit: 096bad7aaaa5d9b5ce698a524cb21f4070c7b4d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2022
ms.locfileid: "62056397"
---
# <a name="microsoftaccountuserconversationmember-resource-type"></a>тип ресурса microsoftAccountUserConversationMember

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет личного пользователя учетной записи Майкрософт в чате.


Наследует от [conversationMember](../resources/conversationmember.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя пользователя. Наследуется [от conversationMember](../resources/conversationmember.md).|
|id|String|Членский ID, который представляет этот ресурс. Наследуется от [сущности](../resources/entity.md).|
|roles|Набор строк|Специальные роли для этого пользователя. Наследуется [от conversationMember](../resources/conversationmember.md).|
|userId|String|ID пользователя.|
|visibleHistoryStartDateTime|DateTimeOffset|Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы. Наследуется [от conversationMember](../resources/conversationmember.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAccountUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAccountUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "userId": "String"
}
```

