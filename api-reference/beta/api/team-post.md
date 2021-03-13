---
title: Создание команды
description: Создание новой команды.
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ac7d879f35a9d98051650e830e7a75a94a98de5e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775383"
---
# <a name="create-team"></a><span data-ttu-id="7ff54-103">Создание команды</span><span class="sxs-lookup"><span data-stu-id="7ff54-103">Create team</span></span>

<span data-ttu-id="7ff54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ff54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ff54-105">Создание новой [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7ff54-105">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7ff54-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ff54-106">Permissions</span></span>

<span data-ttu-id="7ff54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ff54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ff54-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ff54-109">Permission type</span></span>                        | <span data-ttu-id="7ff54-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ff54-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="7ff54-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ff54-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ff54-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ff54-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="7ff54-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ff54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ff54-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ff54-114">Not supported.</span></span>                              |
| <span data-ttu-id="7ff54-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ff54-115">Application</span></span>                            | <span data-ttu-id="7ff54-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ff54-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="7ff54-117">**Примечание**. Разрешение Teamwork.Migrate.All поддерживается *только* для [миграции](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="7ff54-117">**Note**: The Teamwork.Migrate.All permission is *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>

## <a name="http-request"></a><span data-ttu-id="7ff54-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ff54-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="7ff54-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ff54-119">Request headers</span></span>

| <span data-ttu-id="7ff54-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ff54-120">Header</span></span>        | <span data-ttu-id="7ff54-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7ff54-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7ff54-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ff54-122">Authorization</span></span> | <span data-ttu-id="7ff54-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ff54-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ff54-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ff54-125">Content-Type</span></span>  | <span data-ttu-id="7ff54-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ff54-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ff54-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ff54-128">Request body</span></span>

<span data-ttu-id="7ff54-129">Предоставьте в тексте запроса описание объекта [team](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ff54-129">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7ff54-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff54-130">Response</span></span>

<span data-ttu-id="7ff54-131">В случае успешного выполнения этот API возвращает отклик `202 Accepted`, содержащий ссылку на [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="7ff54-131">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="7ff54-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="7ff54-132">Examples</span></span>

### <a name="example-1-delegated-permissions"></a><span data-ttu-id="7ff54-133">Пример 1. Делегированные разрешения</span><span class="sxs-lookup"><span data-stu-id="7ff54-133">Example 1: Delegated permissions</span></span>

<span data-ttu-id="7ff54-134">Ниже приведен пример минимального запроса.</span><span class="sxs-lookup"><span data-stu-id="7ff54-134">The following is an example of a minimal request.</span></span> <span data-ttu-id="7ff54-135">Исключив другие свойства, клиент неявно принимает значения по умолчанию из готового шаблона, представленного объектом `template`.</span><span class="sxs-lookup"><span data-stu-id="7ff54-135">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="7ff54-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff54-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7ff54-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff54-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description"
}
```
# <a name="c"></a>[<span data-ttu-id="7ff54-138">C#</span><span class="sxs-lookup"><span data-stu-id="7ff54-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ff54-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ff54-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ff54-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ff54-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ff54-141">Java</span><span class="sxs-lookup"><span data-stu-id="7ff54-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->

##### <a name="response"></a><span data-ttu-id="7ff54-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff54-142">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "create_team_post",
  "@odata.type": "microsoft.graph.team"
}-->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-2-application-permissions"></a><span data-ttu-id="7ff54-143">Пример 2. Разрешения для приложения</span><span class="sxs-lookup"><span data-stu-id="7ff54-143">Example 2: Application permissions</span></span>

<span data-ttu-id="7ff54-144">Ниже приведен пример минимального запроса с использованием разрешений для приложения.</span><span class="sxs-lookup"><span data-stu-id="7ff54-144">The following is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="7ff54-145">Исключив другие свойства, клиент неявно принимает значения по умолчанию из готового шаблона, представленного объектом `template`.</span><span class="sxs-lookup"><span data-stu-id="7ff54-145">By omitting other properties, the client is implicitly taking defaults from the predefined template represented by `template`.</span></span> <span data-ttu-id="7ff54-146">При отправке запроса с разрешениями для приложения ресурс [user](../resources/user.md) должен быть указан в коллекции `members`.</span><span class="sxs-lookup"><span data-stu-id="7ff54-146">When issuing a request with application permissions, a [user](../resources/user.md) must be specified in the `members` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="7ff54-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff54-147">Request</span></span>
<!-- markdownlint-disable MD025 -->

# <a name="http"></a>[<span data-ttu-id="7ff54-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff54-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post_minimal"
}-->

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/beta/teamsTemplates('standard')",
   "displayName":"My Sample Team",
   "description":"My Sample Team’s Description",
   "members":[
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "roles":[
            "owner"
         ],
         "user@odata.bind":"https://graph.microsoft.com/beta/users('0040b377-61d8-43db-94f5-81374122dc7e')"
      }
   ]
}
```

# <a name="c"></a>[<span data-ttu-id="7ff54-149">C#</span><span class="sxs-lookup"><span data-stu-id="7ff54-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ff54-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ff54-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ff54-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ff54-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ff54-152">Java</span><span class="sxs-lookup"><span data-stu-id="7ff54-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-post-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7ff54-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff54-153">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_minimal",
  "@odata.type": "microsoft.graph.team"
}-->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-3-create-a-team-with-multiple-channels-installed-apps-and-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="7ff54-154">Пример 3. Создание команды с несколькими каналами, установленными приложениями и закрепленными вкладками с использованием делегированных разрешений</span><span class="sxs-lookup"><span data-stu-id="7ff54-154">Example 3: Create a team with multiple channels, installed apps, and pinned tabs using delegated permissions</span></span>

<span data-ttu-id="7ff54-155">Ниже приведен запрос с указанием полного набора полезных данных.</span><span class="sxs-lookup"><span data-stu-id="7ff54-155">The following is a request with a full payload.</span></span> <span data-ttu-id="7ff54-156">Клиент может переопределить значения в базовом шаблоне и добавить элементы со значениями массива в пределах, допускаемых правилами проверки для объекта `specialization`.</span><span class="sxs-lookup"><span data-stu-id="7ff54-156">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="7ff54-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff54-157">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7ff54-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff54-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post_full_payload"
}-->

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
                    "displayName": "A Pinned Website",
                    "configuration": {
                        "contentUrl": "https://docs.microsoft.com/microsoftteams/microsoft-teams"
                    }
                },
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.youtube')",
                    "displayName": "A Pinned YouTube Video",
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
    "discoverySettings": {
        "showInTeamsSearchAndSuggestions": true
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
# <a name="c"></a>[<span data-ttu-id="7ff54-159">C#</span><span class="sxs-lookup"><span data-stu-id="7ff54-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-full-payload-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ff54-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ff54-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-full-payload-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ff54-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ff54-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-full-payload-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ff54-162">Java</span><span class="sxs-lookup"><span data-stu-id="7ff54-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-post-full-payload-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7ff54-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff54-163">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_full_payload",
  "@odata.type": "microsoft.graph.team"
}-->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-4-create-a-team-from-group"></a><span data-ttu-id="7ff54-164">Пример 4. Создание команды из группы</span><span class="sxs-lookup"><span data-stu-id="7ff54-164">Example 4: Create a team from group</span></span>

<span data-ttu-id="7ff54-165">В следующем примере показано, как можно создать новую [команду](../resources/team.md) из [группы](../resources/group.md) с учетом **groupId**.</span><span class="sxs-lookup"><span data-stu-id="7ff54-165">The following example shows how you can create a new [team](../resources/team.md) from a [group](../resources/group.md), given a **groupId**.</span></span>

<span data-ttu-id="7ff54-166">Обратите внимание на некоторые моменты, связанные с этим вызовом:</span><span class="sxs-lookup"><span data-stu-id="7ff54-166">A few things to note about this call:</span></span>

* <span data-ttu-id="7ff54-167">Чтобы создать команду, в группе, из которой она создается, должен быть хотя бы один владелец.</span><span class="sxs-lookup"><span data-stu-id="7ff54-167">In order to create a team, the group you're creating it from must have a least one owner.</span></span>
* <span data-ttu-id="7ff54-168">Созданная команда всегда наследует отображаемое имя, параметры видимости, специализацию и членов группы.</span><span class="sxs-lookup"><span data-stu-id="7ff54-168">The team that's created will always inherit from the group's display name, visibility, specialization, and members.</span></span> <span data-ttu-id="7ff54-169">Поэтому, когда выполняется этот вызов с использованием свойства **group@odata.bind**, включение свойств команды **displayName**, **visibility**, **specialization** или **members@odata.bind** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="7ff54-169">Therefore, when making this call with the **group@odata.bind** property, the inclusion of team **displayName**, **visibility**, **specialization**, or **members@odata.bind** properties will return an error.</span></span>
* <span data-ttu-id="7ff54-170">Если группа создана менее 15 минут назад, вызов метода "Создание команды" может завершиться ошибкой с кодом 404 из-за задержек репликации.</span><span class="sxs-lookup"><span data-stu-id="7ff54-170">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="7ff54-171">Рекомендуется повторить вызов метода "Создание команды" три раза с 10-секундной задержкой между вызовами.</span><span class="sxs-lookup"><span data-stu-id="7ff54-171">We recommend that you retry the Create team call three times, with a 10 second delay between calls.</span></span>

#### <a name="request"></a><span data-ttu-id="7ff54-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff54-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7ff54-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff54-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_from_group"
}-->

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')"
}
```

# <a name="c"></a>[<span data-ttu-id="7ff54-174">C#</span><span class="sxs-lookup"><span data-stu-id="7ff54-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ff54-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ff54-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ff54-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ff54-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ff54-177">Java</span><span class="sxs-lookup"><span data-stu-id="7ff54-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7ff54-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff54-178">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-5-create-a-team-from-a-group-with-multiple-channels-installed-apps-and-pinned-tabs"></a><span data-ttu-id="7ff54-179">Пример 5. Создание команды из группы с несколькими каналами, установленными приложениями и закрепленными вкладками</span><span class="sxs-lookup"><span data-stu-id="7ff54-179">Example 5: Create a team from a group with multiple channels, installed apps, and pinned tabs</span></span>

<span data-ttu-id="7ff54-180">Ниже указан запрос, преобразующий существующую группу с расширенными свойствами, в результате чего создается команда с несколькими каналами, установленными приложениями и закрепленными вкладками.</span><span class="sxs-lookup"><span data-stu-id="7ff54-180">The following is a request that converts an existing group with extended properties which will create the team with multiple channels, installed apps, and pinned tabs.</span></span>

<span data-ttu-id="7ff54-181">Дополнительные сведения о поддерживаемых базовых типах шаблонов и свойствах см. в статье [Начало работы с шаблонами Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="7ff54-181">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="7ff54-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff54-182">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7ff54-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff54-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_group"
}-->

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/beta/teamsTemplates('standard')",
   "group@odata.bind":"https://graph.microsoft.com/v1.0/groups('groupId')",
   "channels":[
      {
         "displayName":"Class Announcements 📢",
         "isFavoriteByDefault":true
      },
      {
         "displayName":"Homework 🏋️",
         "isFavoriteByDefault":true
      }
   ],
   "memberSettings":{
      "allowCreateUpdateChannels":false,
      "allowDeleteChannels":false,
      "allowAddRemoveApps":false,
      "allowCreateUpdateRemoveTabs":false,
      "allowCreateUpdateRemoveConnectors":false
   },
   "installedApps":[
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
      },
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
      }
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="7ff54-184">C#</span><span class="sxs-lookup"><span data-stu-id="7ff54-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ff54-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ff54-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ff54-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ff54-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ff54-187">Java</span><span class="sxs-lookup"><span data-stu-id="7ff54-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7ff54-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff54-188">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-6-create-a-team-with-a-non-standard-base-template-type"></a><span data-ttu-id="7ff54-189">Пример 6. Создание команды с использованием нестандартного базового типа шаблона</span><span class="sxs-lookup"><span data-stu-id="7ff54-189">Example 6: Create a team with a non-standard base template type</span></span>

<span data-ttu-id="7ff54-190">Базовые типы шаблонов — это специальные шаблоны, созданные корпорацией Майкрософт для определенных отраслей.</span><span class="sxs-lookup"><span data-stu-id="7ff54-190">Base template types are special templates that Microsoft created for specific industries.</span></span> <span data-ttu-id="7ff54-191">Эти базовые шаблоны зачастую содержат защищаемые приложения, недоступные в свойствах хранилища и команды, которые еще не поддерживаются по отдельности в шаблонах Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7ff54-191">These base templates often contain proprietary apps that aren't available in the store and team properties that are not yet supported individually in Microsoft Teams templates.</span></span>

<span data-ttu-id="7ff54-192">Чтобы создать команду на основе нестандартного базового шаблона, потребуется изменить значение свойства `template@odata.bind` со `standard` на название этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="7ff54-192">To create a team from a non-standard base template, you’ll want to change the `template@odata.bind` property in the request body from `standard` to point to the specific base template you’d like to create.</span></span>

<span data-ttu-id="7ff54-193">Дополнительные сведения о поддерживаемых базовых типах шаблонов см. в статье [Начало работы с шаблонами Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="7ff54-193">To learn more about supported base template types, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="7ff54-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff54-194">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7ff54-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff54-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard"
}-->

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description"
}
```
# <a name="c"></a>[<span data-ttu-id="7ff54-196">C#</span><span class="sxs-lookup"><span data-stu-id="7ff54-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-non-standard-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ff54-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ff54-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-non-standard-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ff54-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ff54-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-non-standard-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ff54-199">Java</span><span class="sxs-lookup"><span data-stu-id="7ff54-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-non-standard-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7ff54-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff54-200">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-7-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a><span data-ttu-id="7ff54-201">Пример 7. Создание команды с использованием нестандартного базового типа шаблона с расширенными свойствами</span><span class="sxs-lookup"><span data-stu-id="7ff54-201">Example 7: Create a team with a non-standard base template type with extended properties</span></span>

<span data-ttu-id="7ff54-202">Базовые типы шаблонов могут быть расширены с помощью дополнительных свойств. Это позволяет дополнить существующий базовый шаблон дополнительными каналами, приложениями, вкладками и параметрами команды.</span><span class="sxs-lookup"><span data-stu-id="7ff54-202">Base template types can be extended with additional properties, enabling you to build on an existing base template with additional team settings, channels, apps, or tabs.</span></span>

<span data-ttu-id="7ff54-203">Дополнительные сведения о поддерживаемых базовых типах шаблонов и свойствах см. в статье [Начало работы с шаблонами Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="7ff54-203">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="7ff54-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff54-204">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7ff54-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff54-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard2"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
   "displayName":"My Class Team",
   "description":"My Class Team’s Description",
   "channels":[
      {
         "displayName":"Class Announcements 📢",
         "isFavoriteByDefault":true
      },
      {
         "displayName":"Homework 🏋️",
         "isFavoriteByDefault":true
      }
   ],
   "memberSettings":{
      "allowCreateUpdateChannels":false,
      "allowDeleteChannels":false,
      "allowAddRemoveApps":false,
      "allowCreateUpdateRemoveTabs":false,
      "allowCreateUpdateRemoveConnectors":false
   },
   "installedApps":[
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
      },
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
      }
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="7ff54-206">C#</span><span class="sxs-lookup"><span data-stu-id="7ff54-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-non-standard2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ff54-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ff54-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-non-standard2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ff54-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ff54-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-non-standard2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ff54-209">Java</span><span class="sxs-lookup"><span data-stu-id="7ff54-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-non-standard2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7ff54-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff54-210">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard2",
  "@odata.type": "microsoft.graph.team"
}-->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-8-create-a-team-in-migration-mode"></a><span data-ttu-id="7ff54-211">Пример 8. Создание команды в режиме миграции</span><span class="sxs-lookup"><span data-stu-id="7ff54-211">Example 8: Create a team in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="7ff54-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff54-212">Request</span></span>

<span data-ttu-id="7ff54-213">В следующем примере показано, как создать команду для импортированных сообщений.</span><span class="sxs-lookup"><span data-stu-id="7ff54-213">The following example shows how to create a team for imported messages.</span></span>

><span data-ttu-id="7ff54-214">**Примечание.** Команды, созданные в режиме миграции, поддерживают только шаблон `standard`.</span><span class="sxs-lookup"><span data-stu-id="7ff54-214">**Note:** Teams created in migration mode only support the `standard` template.</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "@microsoft.graph.teamCreationMode": "migration",
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```

#### <a name="response"></a><span data-ttu-id="7ff54-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff54-215">Response</span></span>

```http
HTTP/1.1 202 Accepted
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
```

#### <a name="error-response"></a><span data-ttu-id="7ff54-216">Отклик с ошибкой</span><span class="sxs-lookup"><span data-stu-id="7ff54-216">Error response</span></span>

<span data-ttu-id="7ff54-217">При безуспешном запросе этот метод возвращает код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="7ff54-217">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> 

```http
400 Bad Request
```

<span data-ttu-id="7ff54-218">Ниже перечислены распространенные причины этого отклика.</span><span class="sxs-lookup"><span data-stu-id="7ff54-218">The following are common reasons for this response:</span></span>

* <span data-ttu-id="7ff54-219">Для **createdDateTime** установлено значение в будущем.</span><span class="sxs-lookup"><span data-stu-id="7ff54-219">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="7ff54-220">Параметр **createdDateTime** указан правильно, но отсутствует атрибут экземпляра **teamCreationMode** или ему присвоено недопустимое значение.</span><span class="sxs-lookup"><span data-stu-id="7ff54-220">**createdDateTime** is correctly specified but the **teamCreationMode** instance attribute is missing or set to an invalid value.</span></span>


## <a name="see-also"></a><span data-ttu-id="7ff54-221">См. также</span><span class="sxs-lookup"><span data-stu-id="7ff54-221">See also</span></span>

* [<span data-ttu-id="7ff54-222">Завершение миграции для команды</span><span class="sxs-lookup"><span data-stu-id="7ff54-222">Complete migration for a team</span></span>](team-completemigration.md)
* [<span data-ttu-id="7ff54-223">Импорт сообщений из сторонних платформ в Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7ff54-223">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="7ff54-224">Создание канала</span><span class="sxs-lookup"><span data-stu-id="7ff54-224">Create channel</span></span>](channel-post.md)
* [<span data-ttu-id="7ff54-225">Доступные шаблоны</span><span class="sxs-lookup"><span data-stu-id="7ff54-225">Available templates</span></span>](/MicrosoftTeams/get-started-with-teams-templates)
* [<span data-ttu-id="7ff54-226">Начало работы с шаблонами команд розничной торговли</span><span class="sxs-lookup"><span data-stu-id="7ff54-226">Getting started with Retail Teams templates</span></span>](/MicrosoftTeams/get-started-with-retail-teams-templates)
* [<span data-ttu-id="7ff54-227">Начало работы с шаблонами команд здравоохранения</span><span class="sxs-lookup"><span data-stu-id="7ff54-227">Getting started with Healthcare Teams templates</span></span>](/MicrosoftTeams/healthcare/healthcare-templates)
* [<span data-ttu-id="7ff54-228">Создание группы с командой</span><span class="sxs-lookup"><span data-stu-id="7ff54-228">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
