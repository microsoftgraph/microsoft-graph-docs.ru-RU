---
title: Создание команды
description: Создание новой команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 3e901225f5a8f94abb61a6b4052b0db2d47865c3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519614"
---
# <a name="create-team"></a><span data-ttu-id="e8eb6-103">Создание команды</span><span class="sxs-lookup"><span data-stu-id="e8eb6-103">Create team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8eb6-104">Создание новой [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="e8eb6-104">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8eb6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8eb6-105">Permissions</span></span>

<span data-ttu-id="e8eb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8eb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8eb6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8eb6-108">Permission type</span></span>                        | <span data-ttu-id="e8eb6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8eb6-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e8eb6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8eb6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8eb6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8eb6-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="e8eb6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8eb6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8eb6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8eb6-113">Not supported.</span></span>                              |
| <span data-ttu-id="e8eb6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8eb6-114">Application</span></span>                            | <span data-ttu-id="e8eb6-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8eb6-115">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e8eb6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8eb6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="e8eb6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8eb6-117">Request headers</span></span>

| <span data-ttu-id="e8eb6-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8eb6-118">Header</span></span>        | <span data-ttu-id="e8eb6-119">Значение</span><span class="sxs-lookup"><span data-stu-id="e8eb6-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="e8eb6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8eb6-120">Authorization</span></span> | <span data-ttu-id="e8eb6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8eb6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8eb6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8eb6-123">Content-Type</span></span>  | <span data-ttu-id="e8eb6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e8eb6-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="e8eb6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8eb6-125">Request body</span></span>

<span data-ttu-id="e8eb6-126">Предоставьте в тексте запроса описание объекта [team](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8eb6-126">In the request body, supply a JSON representation of [plannerBucket](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e8eb6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8eb6-127">Response</span></span>

<span data-ttu-id="e8eb6-128">В случае успешного выполнения этот API возвращает отклик `202 Accepted`, содержащий ссылку на [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e8eb6-128">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="e8eb6-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8eb6-129">Examples</span></span>

### <a name="example---delegated-permissions"></a><span data-ttu-id="e8eb6-130">Пример: делегированные разрешения</span><span class="sxs-lookup"><span data-stu-id="e8eb6-130">Example - delegated permissions</span></span>

<span data-ttu-id="e8eb6-131">Ниже приведен пример минимального запроса.</span><span class="sxs-lookup"><span data-stu-id="e8eb6-131">Here is an example of a minimal request.</span></span> <span data-ttu-id="e8eb6-132">Исключив другие свойства, клиент неявно принимает значения по умолчанию из готового шаблона, представленного объектом `template`.</span><span class="sxs-lookup"><span data-stu-id="e8eb6-132">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="e8eb6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8eb6-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
}
```

##### <a name="response"></a><span data-ttu-id="e8eb6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8eb6-134">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="e8eb6-135">Пример: создание команды с помощью установленного приложения с несколькими каналами с закрепленными вкладками при использовании делегированных разрешений</span><span class="sxs-lookup"><span data-stu-id="e8eb6-135">Example - create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="e8eb6-136">Ниже приведен запрос с указанием полного набора полезных данных.</span><span class="sxs-lookup"><span data-stu-id="e8eb6-136">Here is request with a full payload.</span></span> <span data-ttu-id="e8eb6-137">Клиент может переопределить значения в базовом шаблоне и добавить элементы со значениями массива в пределах, допускаемых правилами проверки для объекта `specialization`.</span><span class="sxs-lookup"><span data-stu-id="e8eb6-137">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="e8eb6-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8eb6-138">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
    "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
    "visibility": "Private",
    "displayName": "Sample Engineering Team",
    "description": "This is a sample engineering team, used to showcase the range of properties supported by this API",
    "channels": [
        {
            "displayName": "Announcements 📢",
            "isFavoriteByDefault": true,
            "description": "This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements."
        },
        {
            "displayName": "Training 🏋️",
            "isFavoriteByDefault": true,
            "description": "This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.",
            "tabs": [
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.web')",
                    "name": "A Pinned Website",
                    "configuration": {
                        "contentUrl": "https://docs.microsoft.com/en-us/microsoftteams/microsoft-teams"
                    }
                },
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.youtube')",
                    "name": "A Pinned YouTube Video",
                    "configuration": {
                        "contentUrl": "https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ",
                        "websiteUrl": "https://www.youtube.com/watch?v=X8krAMdGvCQ"
                    }
                }
            ]
        },
        {
            "displayName": "Planning 📅 ",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.",
            "isFavoriteByDefault": false
        },
        {
            "displayName": "Issues and Feedback 🐞",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu."
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": true,
        "allowDeleteChannels": true,
        "allowAddRemoveApps": true,
        "allowCreateUpdateRemoveTabs": true,
        "allowCreateUpdateRemoveConnectors": true
    },
    "guestSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false
    },
    "funSettings": {
        "allowGiphy": true,
        "giphyContentRating": "Moderate",
        "allowStickersAndMemes": true,
        "allowCustomMemes": true
    },
    "messagingSettings": {
        "allowUserEditMessages": true,
        "allowUserDeleteMessages": true,
        "allowOwnerDeleteMessages": true,
        "allowTeamMentions": true,
        "allowChannelMentions": true
    },
    "installedApps": [
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
        },
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="e8eb6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8eb6-139">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---application-permissions"></a><span data-ttu-id="e8eb6-140">Пример: разрешения для приложений</span><span class="sxs-lookup"><span data-stu-id="e8eb6-140">Example - application permissions</span></span>

<span data-ttu-id="e8eb6-141">Ниже приведен минимальный запрос с использованием разрешений для приложения.</span><span class="sxs-lookup"><span data-stu-id="e8eb6-141">Here is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="e8eb6-142">Исключив другие свойства, клиент неявно принимает значения по умолчанию из готового шаблона, представленного объектом `template`.</span><span class="sxs-lookup"><span data-stu-id="e8eb6-142">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span> <span data-ttu-id="e8eb6-143">При отправке запроса с разрешениями для приложения ресурс [user](../resources/user.md) должен быть указан в коллекции `owners`.</span><span class="sxs-lookup"><span data-stu-id="e8eb6-143">When issuing a request with application permissions a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="e8eb6-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8eb6-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users('abc123')"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="e8eb6-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8eb6-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="e8eb6-146">См. также</span><span class="sxs-lookup"><span data-stu-id="e8eb6-146">See also</span></span>

- [<span data-ttu-id="e8eb6-147">Создание группы с командой</span><span class="sxs-lookup"><span data-stu-id="e8eb6-147">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/team-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
