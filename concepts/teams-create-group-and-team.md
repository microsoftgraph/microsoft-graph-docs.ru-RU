---
title: Создание группы с помощью команды Microsoft Teams
description: 'Создание группы, которая включает команду, состоит из двух этапов: '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 06b25a6da159030407c904622ffebde09c704d98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549022"
---
# <a name="creating-a-group-with-a-microsoft-teams-team"></a><span data-ttu-id="f8230-103">Создание группы с помощью команды Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f8230-103">Creating a group with a Microsoft Teams team</span></span>

<span data-ttu-id="f8230-104">Создание [группы](/graph/api/resources/group?view=graph-rest-beta), которая включает [команду](/graph/api/resources/team?view=graph-rest-beta), состоит из двух этапов:</span><span class="sxs-lookup"><span data-stu-id="f8230-104">Creating a [group](/graph/api/resources/group?view=graph-rest-beta) that includes a [team](/graph/api/resources/team?view=graph-rest-beta) involves two steps:</span></span> 

- <span data-ttu-id="f8230-105">[Создание группы](/graph/api/group-post-groups?view=graph-rest-beta) с правильными свойствами.</span><span class="sxs-lookup"><span data-stu-id="f8230-105">[Create a group](/graph/api/group-post-groups?view=graph-rest-beta) with the right properties.</span></span>
- <span data-ttu-id="f8230-106">[Добавление команды](/graph/api/team-put-teams?view=graph-rest-beta) в группу.</span><span class="sxs-lookup"><span data-stu-id="f8230-106">[Add a team](/graph/api/team-put-teams?view=graph-rest-beta) to the group.</span></span>

## <a name="create-a-group"></a><span data-ttu-id="f8230-107">Создание группы</span><span class="sxs-lookup"><span data-stu-id="f8230-107">Create a group</span></span>

<span data-ttu-id="f8230-108">Чтобы добавить группу, вам необходимо настроить указанные ниже значения свойств, как показано в приведенном ниже примере:</span><span class="sxs-lookup"><span data-stu-id="f8230-108">In order to include a team, you need to set the following property values, as shown in the following example:</span></span>

- <span data-ttu-id="f8230-109">**groupTypes** = { "Unified" }</span><span class="sxs-lookup"><span data-stu-id="f8230-109">**groupTypes** = { "Unified" }</span></span> 
- <span data-ttu-id="f8230-110">**mailEnabled** = true</span><span class="sxs-lookup"><span data-stu-id="f8230-110">**mailEnabled** = true</span></span>
- <span data-ttu-id="f8230-111">**securityEnabled** = false</span><span class="sxs-lookup"><span data-stu-id="f8230-111">**securityEnabled** = false</span></span>

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

<span data-ttu-id="f8230-112">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f8230-112">The following example shows response.</span></span> 

><span data-ttu-id="f8230-113">**Примечание.** Показанный объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f8230-113">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="f8230-114">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8230-114">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a><span data-ttu-id="f8230-115">Добавление команды в группу</span><span class="sxs-lookup"><span data-stu-id="f8230-115">Add a team to the group</span></span>

<span data-ttu-id="f8230-116">Добавьте команду в группу, как показано.</span><span class="sxs-lookup"><span data-stu-id="f8230-116">Add a team to the group, as shown.</span></span>

```http
PUT /groups/{id}/team
{ }
```

<span data-ttu-id="f8230-117">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f8230-117">The following example shows the response.</span></span> 

><span data-ttu-id="f8230-118">**Примечание.** Показанный объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f8230-118">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="f8230-119">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8230-119">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="f8230-120">Идентификатор созданной команды такой же, как и идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="f8230-120">The created team has the same ID as the group.</span></span>
