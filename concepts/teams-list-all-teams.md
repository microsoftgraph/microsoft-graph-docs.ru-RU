---
title: Перечисление всех команд в Microsoft Teams для организации
description: Используйте API Microsoft Teams в Microsoft Graph, чтобы составить список всех команд в организации, найдя все группы, в которых есть команды, и получив сведения для каждой команды.
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 955d55d521d1dda3ace17943261477020f2fb935
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556145"
---
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a>Перечисление всех команд в Microsoft Teams для организации

Чтобы использовать API Microsoft Teams в Microsoft Graph для получения списка всех [команд](/graph/api/resources/team) в организации (клиенте), вы найдете все группы, в которых есть команды, а затем получите сведения для каждой команды.

## <a name="get-a-list-of-groups"></a>Получение списка групп

### <a name="example-1-get-a-list-of-groups-that-contain-a-team"></a>Пример 1. Получение списка групп, содержащих команду

Чтобы получить список всех [групп](/graph/api/resources/group) в организации, у которых есть команды, получите [список всех групп](/graph/api/group-list), а затем в коде найдите те, у которых есть свойство **resourceProvisioningOptions**, содержащее "Team".

Используйте API с `$filter` для возврата только тех групп, в которых есть команды.

#### <a name="request"></a>Запрос

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> [!NOTE]
> Для некоторых неиспользуемых старых команд не будет установлен параметр **resourceProvisioningOptions**. Дополнительные сведения см. в статье [Известные проблемы](known-issues.md#properties-are-missing-in-the-list-of-teams-that-a-user-has-joined).

#### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

>**Примечание.** Показанный объект ответа может быть сокращен для удобочитаемости. 
>
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "02bd9fd6-8f93-4758-87c3-1fb73740a315",
            "description": "Welcome to the HR Taskforce team.",
            "displayName": "HR Taskforce",
            "groupTypes": [
                "Unified"
            ],
            "mailEnabled": true,
            "mailNickname": "HRTaskforce",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [
                "Team"
            ],
            "securityEnabled": false,
            "visibility": "Private"
        },
        {
            "id": "8090c93e-ba7c-433e-9f39-08c7ba07c0b3",
            "description": "Welcome to the team that we've assembled to launch our product.",
            "displayName": "X1050 Launch Team",
            "groupTypes": [
                "Unified"
            ],
            "mailEnabled": true,
            "mailNickname": "X1050LaunchTeam",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [
                "Team"
            ],
            "securityEnabled": false,
            "visibility": "Private"
        }
    ]
}
```

### <a name="example-2-get-a-list-of-groups-by-selecting-required-properties-only"></a>Пример 2: Получение списка групп с помощью выбора только необходимых свойств

Так как группы являются большими объектами, используйте `$select`, чтобы получить только нужные свойства группы.

#### <a name="request"></a>Запрос

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> [!NOTE]
> Для некоторых неиспользуемых старых команд не будет установлен параметр **resourceProvisioningOptions**. Дополнительные сведения см. в статье [Известные проблемы](known-issues.md#properties-are-missing-in-the-list-of-teams-that-a-user-has-joined).

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "00e897b1-70ba-4cb9-9126-fd5f95c4bb78",
            "resourceProvisioningOptions": []
        },
        {
            "id": "00f6e045-f884-4359-a617-d459ee626862",
            "resourceProvisioningOptions": [
                "Team"
            ]
        }
    ]
}

```

## <a name="get-team-information-for-a-group"></a>Получение сведений о команде для группы

Чтобы получить сведения о команде в определенной группе, вызовите API [get team](/graph/api/team-get) и включите идентификатор группы.

### <a name="request"></a>Запрос

```http
GET /teams/{group-id}
```

### <a name="response"></a>Отклик

Ниже показан пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

## <a name="see-also"></a>См. также

- [Перечисление объектов joinedTeams](/graph/api/user-list-joinedteams)
- [Перечисление групп](/graph/api/group-list)
- [Обзор API Microsoft Teams](teams-concept-overview.md)