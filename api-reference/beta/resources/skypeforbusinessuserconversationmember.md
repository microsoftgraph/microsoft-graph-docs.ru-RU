---
title: тип ресурса skypeForBusinessUserConversationMember
description: Представляет пользователя Skype для бизнеса в чате
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3badca1cb93a2e001e31bb9280a1a213f5be7805
ms.sourcegitcommit: 096bad7aaaa5d9b5ce698a524cb21f4070c7b4d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2022
ms.locfileid: "62056379"
---
# <a name="skypeforbusinessuserconversationmember-resource-type"></a>тип ресурса skypeForBusinessUserConversationMember

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователя Skype для бизнеса в чате. 

Сведения о совместной Teams и Skype для бизнеса см. в Microsoft Teams и Skype для бизнеса сосуществовании и [совместной работы.](/microsoftteams/teams-and-skypeforbusiness-coexistence-and-interoperability)

Наследует от [conversationMember](../resources/conversationmember.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя пользователя. Наследуется [от conversationMember](../resources/conversationmember.md).|
|id|String|Членский ID, который представляет этот ресурс. Наследуется от [сущности](../resources/entity.md).|
|roles|Набор строк|Специальные роли для этого пользователя. Наследуется [от conversationMember](../resources/conversationmember.md).|
|tenantId|String|ID клиента, к которой принадлежит пользователь.|
|userId|String|ID пользователя.|
|visibleHistoryStartDateTime|DateTimeOffset|Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы. Наследуется [от conversationMember](../resources/conversationmember.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeForBusinessUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "userId": "String",
  "tenantId": "String"
}
```

