---
title: тип ресурса skypeUserConversationMember
description: Представляет пользователя Skype в чате
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c31f0af2f7e61783e540e0fa1a714fd846deed8d
ms.sourcegitcommit: 096bad7aaaa5d9b5ce698a524cb21f4070c7b4d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2022
ms.locfileid: "62056382"
---
# <a name="skypeuserconversationmember-resource-type"></a>тип ресурса skypeUserConversationMember

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователя Skype пользователя в чате. 

Сведения о совместной Teams и Skype для бизнеса см. в Microsoft Teams и Skype для бизнеса сосуществовании и [совместной работы.](/microsoftteams/teams-and-skypeforbusiness-coexistence-and-interoperability)

Наследует от [conversationMember](../resources/conversationmember.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя пользователя. Наследуется [от conversationMember](../resources/conversationmember.md).|
|id|String|Членский ID, который представляет этот ресурс. Наследуется от [сущности](../resources/entity.md).|
|roles|Набор строк|Специальные роли для этого пользователя. Наследуется [от conversationMember](../resources/conversationmember.md).|
|SkypeId|String|Skype пользователя.|
|visibleHistoryStartDateTime|DateTimeOffset|Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы. Наследуется [от conversationMember](../resources/conversationmember.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "skypeId": "String"
}
```

