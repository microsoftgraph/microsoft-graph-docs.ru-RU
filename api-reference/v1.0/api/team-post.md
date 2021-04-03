---
title: Создание команды
description: Создание новой команды.
author: anandjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 77aa0a93e175138d978af98e55388bb124ccf58c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509308"
---
# <a name="create-team"></a><span data-ttu-id="c7056-103">Создание команды</span><span class="sxs-lookup"><span data-stu-id="c7056-103">Create team</span></span>

<span data-ttu-id="c7056-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7056-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7056-105">Создание новой [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c7056-105">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7056-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7056-106">Permissions</span></span>

<span data-ttu-id="c7056-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7056-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7056-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7056-109">Permission type</span></span>                        | <span data-ttu-id="c7056-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7056-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c7056-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7056-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7056-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7056-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="c7056-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7056-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7056-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7056-114">Not supported.</span></span>                              |
| <span data-ttu-id="c7056-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7056-115">Application</span></span>                            | <span data-ttu-id="c7056-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7056-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="c7056-117">**Примечание**. Разрешение Teamwork.Migrate.All поддерживается *только* для [миграции](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="c7056-117">**Note**: The Teamwork.Migrate.All permission is *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="c7056-118">В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на основе количества импортированных данных.</span><span class="sxs-lookup"><span data-stu-id="c7056-118">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="c7056-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7056-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="c7056-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7056-120">Request headers</span></span>

| <span data-ttu-id="c7056-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7056-121">Header</span></span>        | <span data-ttu-id="c7056-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7056-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="c7056-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7056-123">Authorization</span></span> | <span data-ttu-id="c7056-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7056-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7056-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7056-126">Content-Type</span></span>  | <span data-ttu-id="c7056-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7056-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7056-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7056-129">Request body</span></span>

<span data-ttu-id="c7056-130">Предоставьте в тексте запроса описание объекта [team](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7056-130">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c7056-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7056-131">Response</span></span>

<span data-ttu-id="c7056-132">В случае успешного выполнения этот API возвращает отклик `202 Accepted`, содержащий ссылку на [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="c7056-132">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="c7056-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="c7056-133">Examples</span></span>

### <a name="example-1-delegated-permissions"></a><span data-ttu-id="c7056-134">Пример 1. Делегированные разрешения</span><span class="sxs-lookup"><span data-stu-id="c7056-134">Example 1: Delegated permissions</span></span>

<span data-ttu-id="c7056-135">Ниже приведен пример минимального запроса.</span><span class="sxs-lookup"><span data-stu-id="c7056-135">The following is an example of a minimal request.</span></span> <span data-ttu-id="c7056-136">Исключив другие свойства, клиент неявно принимает значения по умолчанию из готового шаблона, представленного объектом `template`.</span><span class="sxs-lookup"><span data-stu-id="c7056-136">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="c7056-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7056-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c7056-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7056-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description"
}
```
# <a name="c"></a>[<span data-ttu-id="c7056-139">C#</span><span class="sxs-lookup"><span data-stu-id="c7056-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7056-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7056-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7056-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7056-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7056-142">Java</span><span class="sxs-lookup"><span data-stu-id="c7056-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


##### <a name="response"></a><span data-ttu-id="c7056-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7056-143">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-2-application-permissions"></a><span data-ttu-id="c7056-144">Пример 2. Разрешения для приложения</span><span class="sxs-lookup"><span data-stu-id="c7056-144">Example 2: Application permissions</span></span>

<span data-ttu-id="c7056-145">Ниже приведен пример минимального запроса с использованием разрешений для приложения.</span><span class="sxs-lookup"><span data-stu-id="c7056-145">The following is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="c7056-146">Исключив другие свойства, клиент неявно принимает значения по умолчанию из готового шаблона, представленного объектом `template`.</span><span class="sxs-lookup"><span data-stu-id="c7056-146">By omitting other properties, the client is implicitly taking defaults from the predefined template represented by `template`.</span></span> <span data-ttu-id="c7056-147">При отправке запроса с разрешениями для приложения ресурс [user](../resources/user.md) должен быть указан в коллекции `members`.</span><span class="sxs-lookup"><span data-stu-id="c7056-147">When issuing a request with application permissions, a [user](../resources/user.md) must be specified in the `members` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="c7056-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7056-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c7056-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7056-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post_minimal"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
   "displayName":"My Sample Team",
   "description":"My Sample Team’s Description",
   "members":[
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "roles":[
            "owner"
         ],
         "user@odata.bind":"https://graph.microsoft.com/v1.0/users('0040b377-61d8-43db-94f5-81374122dc7e')"
      }
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="c7056-150">C#</span><span class="sxs-lookup"><span data-stu-id="c7056-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7056-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7056-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7056-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7056-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7056-153">Java</span><span class="sxs-lookup"><span data-stu-id="c7056-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-post-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


#### <a name="response"></a><span data-ttu-id="c7056-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7056-154">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_minimal",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-3-create-a-team-with-multiple-channels-installed-apps-and-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="c7056-155">Пример 3. Создание команды с несколькими каналами, установленными приложениями и закрепленными вкладками с использованием делегированных разрешений</span><span class="sxs-lookup"><span data-stu-id="c7056-155">Example 3: Create a team with multiple channels, installed apps, and pinned tabs using delegated permissions</span></span>

<span data-ttu-id="c7056-156">Ниже приведен запрос с указанием полного набора полезных данных.</span><span class="sxs-lookup"><span data-stu-id="c7056-156">The following is a request with a full payload.</span></span> <span data-ttu-id="c7056-157">Клиент может переопределить значения в базовом шаблоне и добавить элементы со значениями массива в пределах, допускаемых правилами проверки для объекта `specialization`.</span><span class="sxs-lookup"><span data-stu-id="c7056-157">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="c7056-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7056-158">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c7056-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7056-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post_full_payload"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
    "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
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
# <a name="c"></a>[<span data-ttu-id="c7056-160">C#</span><span class="sxs-lookup"><span data-stu-id="c7056-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-full-payload-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7056-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7056-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-full-payload-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c7056-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7056-162">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_full_payload",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('958e8cf8-169a-42aa-8599-5c1c5479c0ca')/operations('00000000-0000-0000-0000-000000000000')
Content-Location: /teams('958e8cf8-169a-42aa-8599-5c1c5479c0ca')
Content-Length: 0
```

### <a name="example-4-create-a-team-from-group"></a><span data-ttu-id="c7056-163">Пример 4. Создание команды из группы</span><span class="sxs-lookup"><span data-stu-id="c7056-163">Example 4: Create a team from group</span></span>

<span data-ttu-id="c7056-164">В следующем примере показано, как можно создать новую [команду](../resources/team.md) из [группы](../resources/group.md) с учетом **groupId**.</span><span class="sxs-lookup"><span data-stu-id="c7056-164">The following example shows how you can create a new [team](../resources/team.md) from a [group](../resources/group.md), given a **groupId**.</span></span>

<span data-ttu-id="c7056-165">Обратите внимание на некоторые моменты, связанные с этим вызовом:</span><span class="sxs-lookup"><span data-stu-id="c7056-165">A few things to note about this call:</span></span>

* <span data-ttu-id="c7056-166">Чтобы создать команду, в группе, из которой она создается, должен быть хотя бы один владелец.</span><span class="sxs-lookup"><span data-stu-id="c7056-166">In order to create a team, the group you're creating it from must have a least one owner.</span></span>
* <span data-ttu-id="c7056-167">Созданная команда всегда наследует отображаемое имя, параметры видимости, специализацию и членов группы.</span><span class="sxs-lookup"><span data-stu-id="c7056-167">The team that's created will always inherit from the group's display name, visibility, specialization, and members.</span></span> <span data-ttu-id="c7056-168">Поэтому, когда выполняется этот вызов с использованием свойства **group@odata.bind**, включение свойств команды **displayName**, **visibility**, **specialization** или **members@odata.bind** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="c7056-168">Therefore, when making this call with the **group@odata.bind** property, the inclusion of team **displayName**, **visibility**, **specialization**, or **members@odata.bind** properties will return an error.</span></span>
* <span data-ttu-id="c7056-169">Если группа создана менее 15 минут назад, вызов метода "Создание команды" может завершиться ошибкой с кодом 404 из-за задержек репликации.</span><span class="sxs-lookup"><span data-stu-id="c7056-169">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="c7056-170">Рекомендуется повторить вызов метода "Создание команды" три раза с 10-секундной задержкой между вызовами.</span><span class="sxs-lookup"><span data-stu-id="c7056-170">We recommend that you retry the Create team call three times, with a 10 second delay between calls.</span></span>

#### <a name="request"></a><span data-ttu-id="c7056-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7056-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c7056-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7056-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')"
}
```
# <a name="c"></a>[<span data-ttu-id="c7056-173">C#</span><span class="sxs-lookup"><span data-stu-id="c7056-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7056-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7056-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7056-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7056-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7056-176">Java</span><span class="sxs-lookup"><span data-stu-id="c7056-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

---
#### <a name="response"></a><span data-ttu-id="c7056-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7056-177">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('71392b2f-1765-406e-86af-5907d9bdb2ab')/operations('9698b2b8-9636-4f49-b7a8-10dadfa7062a')
Content-Location: /teams('71392b2f-1765-406e-86af-5907d9bdb2ab')
Content-Length: 0
```

### <a name="example-5-create-a-team-from-a-group-with-multiple-channels-installed-apps-and-pinned-tabs"></a><span data-ttu-id="c7056-178">Пример 5. Создание команды из группы с несколькими каналами, установленными приложениями и закрепленными вкладками</span><span class="sxs-lookup"><span data-stu-id="c7056-178">Example 5: Create a team from a group with multiple channels, installed apps, and pinned tabs</span></span>

<span data-ttu-id="c7056-179">Ниже указан запрос, преобразующий существующую группу с расширенными свойствами, в результате чего создается команда с несколькими каналами, установленными приложениями и закрепленными вкладками.</span><span class="sxs-lookup"><span data-stu-id="c7056-179">The following is a request that converts an existing group with extended properties which will create the team with multiple channels, installed apps, and pinned tabs.</span></span>

<span data-ttu-id="c7056-180">Дополнительные сведения о поддерживаемых базовых типах шаблонов и свойствах см. в статье [Начало работы с шаблонами Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="c7056-180">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="c7056-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7056-181">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c7056-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7056-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
   "group@odata.bind":"https://graph.microsoft.com/v1.0/groups('dbd8de4f-5d47-48da-87f1-594bed003375')",
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
# <a name="c"></a>[<span data-ttu-id="c7056-183">C#</span><span class="sxs-lookup"><span data-stu-id="c7056-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7056-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7056-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7056-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7056-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7056-186">Java</span><span class="sxs-lookup"><span data-stu-id="c7056-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---

---
#### <a name="response"></a><span data-ttu-id="c7056-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7056-187">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-6-create-a-team-with-a-non-standard-base-template-type"></a><span data-ttu-id="c7056-188">Пример 6. Создание команды с использованием нестандартного базового типа шаблона</span><span class="sxs-lookup"><span data-stu-id="c7056-188">Example 6: Create a team with a non-standard base template type</span></span>

<span data-ttu-id="c7056-189">Базовые типы шаблонов — это специальные шаблоны, созданные корпорацией Майкрософт для определенных отраслей.</span><span class="sxs-lookup"><span data-stu-id="c7056-189">Base template types are special templates that Microsoft created for specific industries.</span></span> <span data-ttu-id="c7056-190">Эти базовые шаблоны зачастую содержат защищаемые приложения, недоступные в свойствах хранилища и команды, которые еще не поддерживаются по отдельности в шаблонах Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c7056-190">These base templates often contain proprietary apps that aren't available in the store and team properties that are not yet supported individually in Microsoft Teams templates.</span></span>

<span data-ttu-id="c7056-191">Чтобы создать команду на основе нестандартного базового шаблона, потребуется изменить значение свойства `template@odata.bind` со `standard` на название этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="c7056-191">To create a team from a non-standard base template, you’ll want to change the `template@odata.bind` property in the request body from `standard` to point to the specific base template you’d like to create.</span></span>

<span data-ttu-id="c7056-192">Дополнительные сведения о поддерживаемых базовых типах шаблонов см. в статье [Начало работы с шаблонами Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="c7056-192">To learn more about supported base template types, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="c7056-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7056-193">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c7056-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7056-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description"
}
```
# <a name="c"></a>[<span data-ttu-id="c7056-195">C#</span><span class="sxs-lookup"><span data-stu-id="c7056-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-non-standard-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7056-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7056-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-non-standard-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7056-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7056-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-non-standard-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7056-198">Java</span><span class="sxs-lookup"><span data-stu-id="c7056-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-non-standard-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---

---

#### <a name="response"></a><span data-ttu-id="c7056-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7056-199">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-7-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a><span data-ttu-id="c7056-200">Пример 7. Создание команды с использованием нестандартного базового типа шаблона с расширенными свойствами</span><span class="sxs-lookup"><span data-stu-id="c7056-200">Example 7: Create a team with a non-standard base template type with extended properties</span></span>

<span data-ttu-id="c7056-201">Базовые типы шаблонов могут быть расширены с помощью дополнительных свойств. Это позволяет дополнить существующий базовый шаблон дополнительными каналами, приложениями, вкладками и параметрами команды.</span><span class="sxs-lookup"><span data-stu-id="c7056-201">Base template types can be extended with additional properties, enabling you to build on an existing base template with additional team settings, channels, apps, or tabs.</span></span>

<span data-ttu-id="c7056-202">Дополнительные сведения о поддерживаемых базовых типах шаблонов и свойствах см. в статье [Начало работы с шаблонами Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="c7056-202">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="c7056-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7056-203">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c7056-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7056-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard2"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')",
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
# <a name="c"></a>[<span data-ttu-id="c7056-205">C#</span><span class="sxs-lookup"><span data-stu-id="c7056-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-non-standard2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7056-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7056-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-non-standard2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7056-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7056-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-non-standard2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7056-208">Java</span><span class="sxs-lookup"><span data-stu-id="c7056-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-non-standard2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---

---
#### <a name="response"></a><span data-ttu-id="c7056-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7056-209">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard2",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-8-create-a-team-in-migration-mode"></a><span data-ttu-id="c7056-210">Пример 8. Создание команды в режиме миграции</span><span class="sxs-lookup"><span data-stu-id="c7056-210">Example 8: Create a team in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="c7056-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7056-211">Request</span></span>

<span data-ttu-id="c7056-212">В следующем примере показано, как создать команду для импортированных сообщений.</span><span class="sxs-lookup"><span data-stu-id="c7056-212">The following example shows how to create a team for imported messages.</span></span>

><span data-ttu-id="c7056-213">**Примечание**. В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на основе количества импортированных данных.|</span><span class="sxs-lookup"><span data-stu-id="c7056-213">**Note:** In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.|</span></span>

><span data-ttu-id="c7056-214">**Примечание.** Команды, созданные в режиме миграции, поддерживают только шаблон `standard`.</span><span class="sxs-lookup"><span data-stu-id="c7056-214">**Note:** Teams created in migration mode only support the `standard` template.</span></span>

```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "@microsoft.graph.teamCreationMode": "migration",
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```

#### <a name="response"></a><span data-ttu-id="c7056-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7056-215">Response</span></span>

```http
HTTP/1.1 202 Accepted
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
```

#### <a name="error-response"></a><span data-ttu-id="c7056-216">Отклик с ошибкой</span><span class="sxs-lookup"><span data-stu-id="c7056-216">Error response</span></span>

<span data-ttu-id="c7056-217">При безуспешном запросе этот метод возвращает код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="c7056-217">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> 

```http
400 Bad Request
```

<span data-ttu-id="c7056-218">Ниже перечислены распространенные причины этого отклика.</span><span class="sxs-lookup"><span data-stu-id="c7056-218">The following are common reasons for this response:</span></span>

* <span data-ttu-id="c7056-219">Для **createdDateTime** установлено значение в будущем.</span><span class="sxs-lookup"><span data-stu-id="c7056-219">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="c7056-220">Параметр **createdDateTime** указан правильно, но отсутствует атрибут экземпляра **teamCreationMode** или ему присвоено недопустимое значение.</span><span class="sxs-lookup"><span data-stu-id="c7056-220">**createdDateTime** is correctly specified but the **teamCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="see-also"></a><span data-ttu-id="c7056-221">См. также</span><span class="sxs-lookup"><span data-stu-id="c7056-221">See also</span></span>

* [<span data-ttu-id="c7056-222">Завершение миграции для команды</span><span class="sxs-lookup"><span data-stu-id="c7056-222">Complete migration for a team</span></span>](team-completemigration.md)
* [<span data-ttu-id="c7056-223">Импорт сообщений из сторонних платформ в Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c7056-223">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="c7056-224">Создание канала</span><span class="sxs-lookup"><span data-stu-id="c7056-224">Create channel</span></span>](channel-post.md)
* [<span data-ttu-id="c7056-225">Доступные шаблоны</span><span class="sxs-lookup"><span data-stu-id="c7056-225">Available templates</span></span>](/MicrosoftTeams/get-started-with-teams-templates)
* [<span data-ttu-id="c7056-226">Начало работы с шаблонами команд розничной торговли</span><span class="sxs-lookup"><span data-stu-id="c7056-226">Getting started with Retail Teams templates</span></span>](/MicrosoftTeams/get-started-with-retail-teams-templates)
* [<span data-ttu-id="c7056-227">Начало работы с шаблонами команд здравоохранения</span><span class="sxs-lookup"><span data-stu-id="c7056-227">Getting started with Healthcare Teams templates</span></span>](/MicrosoftTeams/healthcare/healthcare-templates)
* [<span data-ttu-id="c7056-228">Создание группы с командой</span><span class="sxs-lookup"><span data-stu-id="c7056-228">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
