---
title: тип ресурса conversationMemberRoleUpdatedEventMessageDetail
description: Представляет сведения о сообщении события об обновленной роли участника беседы в канале или команде.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2ab15ff8f874ffeaa4424f29b8cc452ae128ae2c
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534423"
---
# <a name="conversationmemberroleupdatedeventmessagedetail-resource-type"></a>тип ресурса conversationMemberRoleUpdatedEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события об обновленной роли участника беседы в канале или команде.
Это сообщение создается при обновлении роли участника в канале или команде.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|conversationMemberRoles|Коллекция String|Роли для пользователя-участника обложек.|
|conversationMemberUser|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|Удостоверение пользователя участника беседы.|
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
- [Пример ответа на сообщение события об обновленной роли участника беседы в канале или команде](/graph/system-messages/#conversation-member-role-updated)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)