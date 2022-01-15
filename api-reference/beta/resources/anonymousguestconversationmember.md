---
title: тип ресурса anonymousGuestConversationMember
description: Представляет анонимного гостя в чате.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f439daa2e5146b37b94862e2dce87a2efb603f02
ms.sourcegitcommit: 096bad7aaaa5d9b5ce698a524cb21f4070c7b4d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2022
ms.locfileid: "62056385"
---
# <a name="anonymousguestconversationmember-resource-type"></a>тип ресурса anonymousGuestConversationMember

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет анонимного гостя в чате. 

Анонимные пользователи не имеют удостоверения Microsoft Teams и могут присоединяться к собраниям с помощью ссылок на присоединиться к собранию. Дополнительные сведения см. в [материале Анонимные пользователи](/microsoftteams/non-standard-users#anonymous-users).


Наследует от [conversationMember](../resources/conversationmember.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|anonymousGuestId|Строка|Уникальный ID, который представляет пользователя. **Примечание:** Этот ID может измениться, если пользователь покидает собрание или присоединяется к нему с другого устройства.|
|displayName|Строка|Имя, предоставленное пользователем при присоединении к собранию. Наследуется [от conversationMember](../resources/conversationmember.md).|
|id|Строка|Членский ID, который представляет этот ресурс. Наследуется от [сущности](../resources/entity.md).|
|roles|Набор строк|Специальные роли для этого пользователя. Наследуется [от conversationMember](../resources/conversationmember.md).|
|visibleHistoryStartDateTime|DateTimeOffset|Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы. Наследуется [от conversationMember](../resources/conversationmember.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.anonymousGuestConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.anonymousGuestConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "anonymousGuestId": "String"
}
```

