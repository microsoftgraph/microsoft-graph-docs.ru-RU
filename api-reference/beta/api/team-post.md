---
title: Создание группы
description: Создание новой группы.
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 891377ace047e51f653327fc081e183de14de5ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847147"
---
# <a name="create-team"></a><span data-ttu-id="27853-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="27853-103">Create team</span></span>

> <span data-ttu-id="27853-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="27853-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27853-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27853-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27853-106">Создание новой [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="27853-106">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="27853-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27853-107">Permissions</span></span>

<span data-ttu-id="27853-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27853-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27853-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27853-110">Permission type</span></span>                        | <span data-ttu-id="27853-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27853-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="27853-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27853-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="27853-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27853-113">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="27853-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27853-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27853-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27853-115">Not supported.</span></span>                              |
| <span data-ttu-id="27853-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27853-116">Application</span></span>                            | <span data-ttu-id="27853-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27853-117">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="27853-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27853-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="27853-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27853-119">Request headers</span></span>

| <span data-ttu-id="27853-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27853-120">Header</span></span>        | <span data-ttu-id="27853-121">Значение</span><span class="sxs-lookup"><span data-stu-id="27853-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="27853-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27853-122">Authorization</span></span> | <span data-ttu-id="27853-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27853-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27853-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27853-125">Content-Type</span></span>  | <span data-ttu-id="27853-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27853-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="27853-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="27853-127">Request body</span></span>

<span data-ttu-id="27853-128">В тексте запроса укажите представление JSON объекта [группы](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="27853-128">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="27853-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="27853-129">Response</span></span>

<span data-ttu-id="27853-130">Успешно завершена, этот интерфейс API возвращает `202 Accepted` ответ, содержащий ссылку на [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="27853-130">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="27853-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="27853-131">Examples</span></span>

### <a name="example---delegated-permissions"></a><span data-ttu-id="27853-132">Пример — делегированных разрешений</span><span class="sxs-lookup"><span data-stu-id="27853-132">Example - delegated permissions</span></span>

<span data-ttu-id="27853-133">Ниже приведен пример минимальной запроса.</span><span class="sxs-lookup"><span data-stu-id="27853-133">Here is an example of a minimal request.</span></span> <span data-ttu-id="27853-134">Упустив другие свойства клиента неявно занимает значения по умолчанию из предварительно определенный шаблон, представленный `template`.</span><span class="sxs-lookup"><span data-stu-id="27853-134">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="27853-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="27853-135">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
}
```

##### <a name="response"></a><span data-ttu-id="27853-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="27853-136">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="27853-137">Пример: Создание группы с установленные приложения, несколько каналов с помощью закрепленных вкладками делегированных разрешений</span><span class="sxs-lookup"><span data-stu-id="27853-137">Example - create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="27853-138">Ниже приводится запрос с полной полезных данных.</span><span class="sxs-lookup"><span data-stu-id="27853-138">Here is request with a full payload.</span></span> <span data-ttu-id="27853-139">Клиент можно переопределить значения в базовый шаблон и добавлять к элементам, поддерживающий одно значение массива в степени, предоставляемым правил проверки для `specialization`.</span><span class="sxs-lookup"><span data-stu-id="27853-139">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="27853-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="27853-140">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="27853-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="27853-141">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---application-permissions"></a><span data-ttu-id="27853-142">Пример — разрешения для приложений</span><span class="sxs-lookup"><span data-stu-id="27853-142">Example - application permissions</span></span>

<span data-ttu-id="27853-143">Ниже приведен пример минимальной запроса с использованием разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="27853-143">Here is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="27853-144">Упустив другие свойства клиента неявно занимает значения по умолчанию из предварительно определенный шаблон, представленный `template`.</span><span class="sxs-lookup"><span data-stu-id="27853-144">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span> <span data-ttu-id="27853-145">После отправки запроса с разрешениями приложения, [пользователь](../resources/user.md) должен быть указан в `owners` семейства сайтов.</span><span class="sxs-lookup"><span data-stu-id="27853-145">When issuing a request with application permissions a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="27853-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="27853-146">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="27853-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="27853-147">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="27853-148">См. также</span><span class="sxs-lookup"><span data-stu-id="27853-148">See also</span></span>

- [<span data-ttu-id="27853-149">Создание группы с группой</span><span class="sxs-lookup"><span data-stu-id="27853-149">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
