---
title: Создание группы с помощью команды Microsoft Teams
description: 'Создание группы, которая включает команду, состоит из двух этапов: '
author: nkramer
ms.openlocfilehash: ea11d0ee7ee4e6e1d0bf6dc10ab8c9d064aa3610
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313890"
---
# <a name="creating-a-group-with-a-microsoft-teams-team"></a>Создание группы с помощью команды Microsoft Teams

Создание [группы](/graph/api/resources/group?view=graph-rest-beta), которая включает [команду](/graph/api/resources/team?view=graph-rest-beta), состоит из двух этапов: 

- [Создание группы](/graph/api/group-post-groups?view=graph-rest-beta) с правильными свойствами.
- [Добавление команды](/graph/api/team-put-teams?view=graph-rest-beta) в группу.

## <a name="create-a-group"></a>Создание группы

Чтобы добавить группу, вам необходимо настроить указанные ниже значения свойств, как показано в приведенном ниже примере:

- **groupTypes** = { "Unified" } 
- **mailEnabled** = true
- **securityEnabled** = false

```http
POST /groups
{
    "displayName":"Flight 157",
    "mailNickname":"flight157",
    "description":"Everything about flight 157",
    "visibility":"Private",
    "groupTypes":["Unified"],
    "mailEnabled":true,
    "securityEnabled":false,
    "members@odata.bind":[
        "https://graph.microsoft.com/v1.0/users/bec05f3d-a818-4b58-8c2e-2b4e74b0246d",
        "https://graph.microsoft.com/v1.0/users/ae67a4f4-2308-4522-9021-9f402ff0fba8",
        "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783",
        "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133"
    ],
    "owners@odata.bind":[
        "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133",
        "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783"
    ]
}
```

Ниже показан пример ответа. 

>**Примечание.** Показанный объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a>Добавление команды в группу

Добавьте команду в группу, как показано.

```http
PUT /groups/{id}/team
{ }
```

Ниже показан пример ответа. 

>**Примечание.** Показанный объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context" : "https://graph.microsoft.com/v1.0/$metadata#teams/$entity",
    "id" : "b7f968af-ca51-42f6-a77e-82c7147bc8f2",
    "webUrl" : "https://example.com",
    "isArchived" : null,
    "memberSettings" : { },
    "guestSettings" : { },
    "messagingSettings" : { },
    "funSettings" : {}
}
```

Идентификатор созданной команды такой же, как и идентификатор группы.
