---
title: Перечисление всех команд в Microsoft Teams для организации
description: 'Чтобы перечислить все команды '
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 1045c71fadcd70f9888f6357366d7097178dbec4
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133575"
---
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a>Перечисление всех команд в Microsoft Teams для организации

Чтобы перечислить все [команды](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) в организации (клиенте), найдите все группы с командами, а затем получите сведения для каждой команды.

## <a name="get-a-list-of-groups"></a>Получение списка групп

Чтобы получить список всех [групп](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) в организации, содержащих команды, получите [список всех групп](/graph/api/group-list?view=graph-rest-beta&preserve-view=true) и затем в коде найдите нужные, имеющие свойство **resourceProvisioningOptions** со значением "Team".
Так как группы являются большими объектами, используйте аргумент $select, чтобы получить только нужные свойства группы.

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> **Примечание**. У некоторых неиспользуемых старых групп отсутствует присвоенное свойство resourceProvisioningOptions. Дополнительные сведения см. в статье [Известные проблемы](known-issues.md#properties-are-missing-in-the-list-of-teams-that-a-user-has-joined).

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

## <a name="get-a-list-of-groups-using-beta-apis"></a>Получение списка групп с помощью бета-версий интерфейсов API

С помощью бета-версий интерфейсов API можно использовать аргумент $filter для возврата только групп, содержащих команды.

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> **Примечание.** Фильтрация групп по свойству resourceProvisioningOptions доступна только в конечной точке бета-версии. Свойство resourceProvisioningOptions доступно в версии 1.0 и бета-версии.

> **Примечание**. Некоторые неиспользуемые старые команды не указываются в списке. Дополнительные сведения см. в статье [Известные проблемы](known-issues.md#properties-are-missing-in-the-list-of-teams-that-a-user-has-joined).

Ниже приведен пример ответа. 

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
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

## <a name="get-team-information-for-a-group"></a>Получение сведений о команде для группы

Чтобы получить сведения о команде в определенной группе, вызовите API [get team](/graph/api/team-get?view=graph-rest-beta&preserve-view=true) и включите идентификатор группы.

```http
GET /teams/{group-id}
```

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

- [Перечисление объектов joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-beta&preserve-view=true)
- [Перечисление групп](/graph/api/group-list?view=graph-rest-beta&preserve-view=true)
