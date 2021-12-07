---
title: тип ресурса conversationMemberRoleUpdatedEventMessageDetail
description: Представляет сведения о сообщении события об обновленной роли участника беседы в канале или команде.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2c91e2a476b048c6d451c31c96ac95a3756bbbe4
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322672"
---
# <a name="conversationmemberroleupdatedeventmessagedetail-resource-type"></a>тип ресурса conversationMemberRoleUpdatedEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события об обновленной [](../resources/conversationMember.md) роли участника беседы в канале [или](../resources/channel.md) [команде.](../resources/team.md)
Это сообщение создается при обновлении  роли участника  в канале или команде. 


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|conversationMemberRoles|Коллекция String|Роли для **пользователя-участника обложек.**|
|conversationMemberUser|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|Удостоверение **пользователя участника** беседы.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conversationMemberRoleUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversationMemberRoleUpdatedEventMessageDetail",
  "conversationMemberRoles": [
    "String"
  ],
  "converstaionMemberUser": {
    "@odata.type": "microsoft.graph.teamworkUserIdentity"
  },
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события об обновленной роли участника беседы в **канале** или **команде**](/graph/system-messages/#conversation-member-role-updated)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
