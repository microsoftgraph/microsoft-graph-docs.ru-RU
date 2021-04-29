---
title: Перечисление всех команд в Microsoft Teams для организации
description: 'Чтобы перечислить все команды '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 8bacd936f67c0ba02ba547104eb9a7983017cbe8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051153"
---
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a><span data-ttu-id="bb203-103">Перечисление всех команд в Microsoft Teams для организации</span><span class="sxs-lookup"><span data-stu-id="bb203-103">List all teams in Microsoft Teams for an organization</span></span>

<span data-ttu-id="bb203-104">Чтобы перечислить все [команды](/graph/api/resources/team?view=graph-rest-beta) в организации (клиенте), найдите все группы с командами, а затем получите сведения для каждой команды.</span><span class="sxs-lookup"><span data-stu-id="bb203-104">To list all [teams](/graph/api/resources/team?view=graph-rest-beta) in an organization (tenant), you find all groups that have teams, and then get information for each team.</span></span>

## <a name="get-a-list-of-groups"></a><span data-ttu-id="bb203-105">Получение списка групп</span><span class="sxs-lookup"><span data-stu-id="bb203-105">Get a list of groups</span></span>

<span data-ttu-id="bb203-106">Чтобы получить список всех [групп](/graph/api/resources/group?view=graph-rest-beta) в организации, содержащих команды, получите [список всех групп](/graph/api/group-list?view=graph-rest-beta) и затем в коде найдите нужные, имеющие свойство **resourceProvisioningOptions** со значением "Team".</span><span class="sxs-lookup"><span data-stu-id="bb203-106">To get a list of all [groups](/graph/api/resources/group?view=graph-rest-beta) in the organization that have teams, get a [list of all groups](/graph/api/group-list?view=graph-rest-beta) and then in code find the ones that have a **resourceProvisioningOptions** property that contains "Team".</span></span>
<span data-ttu-id="bb203-107">Так как группы являются большими объектами, используйте аргумент $select, чтобы получить только нужные свойства группы.</span><span class="sxs-lookup"><span data-stu-id="bb203-107">Since groups are large objects, use $select to only get the properties of the group you care about.</span></span>

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> <span data-ttu-id="bb203-108">**Примечание**. У некоторых неиспользуемых старых групп отсутствует присвоенное свойство resourceProvisioningOptions.</span><span class="sxs-lookup"><span data-stu-id="bb203-108">**Note**: Certain unused old teams will not have resourceProvisioningOptions set.</span></span> <span data-ttu-id="bb203-109">Дополнительные сведения см. в статье [Известные проблемы](known-issues.md#missing-teams-in-list-all-teams).</span><span class="sxs-lookup"><span data-stu-id="bb203-109">For details, see [known issues](known-issues.md#missing-teams-in-list-all-teams).</span></span>

<span data-ttu-id="bb203-110">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bb203-110">The following is an example of the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

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

## <a name="get-a-list-of-groups-using-beta-apis"></a><span data-ttu-id="bb203-111">Получение списка групп с помощью бета-версий интерфейсов API</span><span class="sxs-lookup"><span data-stu-id="bb203-111">Get a list of groups using beta APIs</span></span>

<span data-ttu-id="bb203-112">С помощью бета-версий интерфейсов API можно использовать аргумент $filter для возврата только групп, содержащих команды.</span><span class="sxs-lookup"><span data-stu-id="bb203-112">Using the beta APIs, you can use $filter to return only the groups that have teams.</span></span>

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> <span data-ttu-id="bb203-113">**Примечание.** Фильтрация групп по свойству resourceProvisioningOptions доступна только в конечной точке бета-версии.</span><span class="sxs-lookup"><span data-stu-id="bb203-113">**Note**: Filtering groups by resourceProvisioningOptions is only available through the beta endpoint.</span></span> <span data-ttu-id="bb203-114">Свойство resourceProvisioningOptions доступно в версии 1.0 и бета-версии.</span><span class="sxs-lookup"><span data-stu-id="bb203-114">resourceProvisioningOptions is available in v1.0 and beta.</span></span>

> <span data-ttu-id="bb203-115">**Примечание**. Некоторые неиспользуемые старые команды не указываются в списке.</span><span class="sxs-lookup"><span data-stu-id="bb203-115">**Note**: Certain unused old teams will not be listed.</span></span> <span data-ttu-id="bb203-116">Дополнительные сведения см. в статье [Известные проблемы](known-issues.md#missing-teams-in-list-all-teams).</span><span class="sxs-lookup"><span data-stu-id="bb203-116">For details, see [known issues](known-issues.md#missing-teams-in-list-all-teams).</span></span>

<span data-ttu-id="bb203-117">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bb203-117">The following is an example of the response.</span></span> 

><span data-ttu-id="bb203-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb203-p105">**Note:** The response object shown might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

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

## <a name="get-team-information-for-a-group"></a><span data-ttu-id="bb203-120">Получение сведений о команде для группы</span><span class="sxs-lookup"><span data-stu-id="bb203-120">Get team information for a group</span></span>

<span data-ttu-id="bb203-121">Чтобы получить сведения о команде в определенной группе, вызовите API [get team](/graph/api/team-get?view=graph-rest-beta) и включите идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="bb203-121">To get team information for the team in a particular group, call the [get team](/graph/api/team-get?view=graph-rest-beta) API and include the group ID.</span></span>

```http
GET /teams/{group-id}
```

<span data-ttu-id="bb203-122">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb203-122">The following example shows the response.</span></span>

><span data-ttu-id="bb203-123">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bb203-123">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

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

## <a name="see-also"></a><span data-ttu-id="bb203-124">См. также</span><span class="sxs-lookup"><span data-stu-id="bb203-124">See also</span></span>

- [<span data-ttu-id="bb203-125">Перечисление объектов joinedTeams</span><span class="sxs-lookup"><span data-stu-id="bb203-125">List joinedTeams</span></span>](/graph/api/user-list-joinedteams?view=graph-rest-beta)
- [<span data-ttu-id="bb203-126">Перечисление групп</span><span class="sxs-lookup"><span data-stu-id="bb203-126">List groups</span></span>](/graph/api/group-list?view=graph-rest-beta)
