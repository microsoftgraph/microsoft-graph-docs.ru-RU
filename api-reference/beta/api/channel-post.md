---
title: Создание канала
description: Создайте новый канал в команде, как указано в теле запроса.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 549d4a3657655c9ee8be6be6bb82fee9dc9d769e
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753859"
---
# <a name="create-channel"></a><span data-ttu-id="4b893-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="4b893-103">Create channel</span></span>

<span data-ttu-id="4b893-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b893-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b893-105">Создайте новый [канал](../resources/channel.md) в команде, как указано в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="4b893-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b893-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b893-106">Permissions</span></span>

<span data-ttu-id="4b893-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b893-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b893-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b893-109">Permission type</span></span>      | <span data-ttu-id="4b893-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b893-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b893-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b893-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4b893-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b893-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="4b893-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b893-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b893-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b893-114">Not supported.</span></span>    |
|<span data-ttu-id="4b893-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4b893-115">Application</span></span> | <span data-ttu-id="4b893-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b893-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="4b893-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="4b893-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="4b893-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="4b893-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4b893-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="4b893-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4b893-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b893-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="4b893-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b893-121">Request headers</span></span>

| <span data-ttu-id="4b893-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b893-122">Header</span></span>       | <span data-ttu-id="4b893-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4b893-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4b893-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b893-124">Authorization</span></span>  | <span data-ttu-id="4b893-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b893-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4b893-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b893-127">Content-Type</span></span>  | <span data-ttu-id="4b893-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b893-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4b893-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b893-130">Request body</span></span>

<span data-ttu-id="4b893-131">В теле запроса укажу представление объекта [канала](../resources/channel.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="4b893-131">In the request body, supply a JSON representation of a [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4b893-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b893-132">Response</span></span>

<span data-ttu-id="4b893-133">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b893-133">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

<span data-ttu-id="4b893-134">При безуспешном запросе этот метод возвращает код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="4b893-134">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> <span data-ttu-id="4b893-135">Ниже перечислены распространенные причины этого отклика.</span><span class="sxs-lookup"><span data-stu-id="4b893-135">The following are common reasons for this response:</span></span>

* <span data-ttu-id="4b893-136">Для **createdDateTime** установлено значение в будущем.</span><span class="sxs-lookup"><span data-stu-id="4b893-136">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="4b893-137">**createdDateTime** правильно задан, но атрибут экземпляра **channelCreationMode** отсутствует или задан как недопустимое значение.</span><span class="sxs-lookup"><span data-stu-id="4b893-137">**createdDateTime** is correctly specified but the **channelCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="examples"></a><span data-ttu-id="4b893-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="4b893-138">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="4b893-139">Пример 1. Создание стандартного канала</span><span class="sxs-lookup"><span data-stu-id="4b893-139">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="4b893-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b893-140">Request</span></span>

<span data-ttu-id="4b893-141">В следующем примере показан запрос на создание стандартного канала.</span><span class="sxs-lookup"><span data-stu-id="4b893-141">The following example shows a request to create a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b893-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b893-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```
# <a name="c"></a>[<span data-ttu-id="4b893-143">C#</span><span class="sxs-lookup"><span data-stu-id="4b893-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b893-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b893-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b893-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b893-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b893-146">Java</span><span class="sxs-lookup"><span data-stu-id="4b893-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="4b893-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b893-147">Response</span></span>

<span data-ttu-id="4b893-148">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b893-148">The following example shows the response.</span></span>

> <span data-ttu-id="4b893-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4b893-149">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_channel_from_group",
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="4b893-150">Пример 2. Создание частного канала от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="4b893-150">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="4b893-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b893-151">Request</span></span>

<span data-ttu-id="4b893-152">В следующем примере показан запрос на создание частного канала и добавление пользователя в качестве владельца команды.</span><span class="sxs-lookup"><span data-stu-id="4b893-152">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b893-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b893-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_private_channel_with_member"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
  "@odata.type": "#Microsoft.Graph.channel",
  "membershipType": "private",
  "displayName": "My First Private Channel",
  "description": "This is my first private channels",
  "members":
     [
        {
           "@odata.type":"#microsoft.graph.aadUserConversationMember",
           "user@odata.bind":"https://graph.microsoft.com/beta/users('62855810-484b-4823-9e01-60667f8b12ae')",
           "roles":["owner"]
        }
     ]
}
```
# <a name="c"></a>[<span data-ttu-id="4b893-154">C#</span><span class="sxs-lookup"><span data-stu-id="4b893-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-private-channel-with-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b893-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b893-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-private-channel-with-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b893-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b893-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-private-channel-with-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b893-157">Java</span><span class="sxs-lookup"><span data-stu-id="4b893-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-private-channel-with-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="4b893-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b893-158">Response</span></span>

<span data-ttu-id="4b893-159">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b893-159">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_private_channel_with_member",
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:33b76eea88574bd1969dca37e2b7a819@thread.skype",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/My%20First%20Private%20Channel?groupId=57fb72d0-d811-46f4-8947-305e6072eaa5&tenantId=0fddfdc5-f319-491f-a514-be1bc1bf9ddc",
    "membershipType": "private"
}
```

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="4b893-160">Пример 3. Создание канала в режиме миграции</span><span class="sxs-lookup"><span data-stu-id="4b893-160">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="4b893-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b893-161">Request</span></span>

<span data-ttu-id="4b893-162">В следующем примере показано, как создать канал, который будет использоваться для импорта сообщений.</span><span class="sxs-lookup"><span data-stu-id="4b893-162">The following example shows how to create a channel that will be used for importing messages.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b893-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b893-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_for_migration"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-Type: application/json

{
  "@microsoft.graph.channelCreationMode": "migration",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```
# <a name="c"></a>[<span data-ttu-id="4b893-164">C#</span><span class="sxs-lookup"><span data-stu-id="4b893-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-for-migration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b893-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b893-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-for-migration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b893-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b893-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-for-migration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b893-167">Java</span><span class="sxs-lookup"><span data-stu-id="4b893-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-for-migration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b893-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b893-168">Response</span></span>

<span data-ttu-id="4b893-169">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b893-169">The following example shows the response.</span></span> <span data-ttu-id="4b893-170">Заглавная дорожка расположения содержимого в ответе указывает путь к каналу, который необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="4b893-170">The Content-Location header in the response specifies the path to the channel that is being provisioned.</span></span>
<span data-ttu-id="4b893-171">После этого этот канал можно использовать для [импорта сообщений.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="4b893-171">Once provisioned, this channel can be used for [importing messages](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_channel_for_migration",
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 202 Accepted
Location: /teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/{channelId}/operations/{operationId}
Content-Location: /teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/{channelId}
```

### <a name="example-4-create-standard-channel-with-moderation-settings"></a><span data-ttu-id="4b893-172">Пример 4. Создание стандартного канала с настройками модерации</span><span class="sxs-lookup"><span data-stu-id="4b893-172">Example 4: Create standard channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="4b893-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b893-173">Request</span></span>

<span data-ttu-id="4b893-174">В следующем примере показан запрос на создание стандартного канала с настройками модерации.</span><span class="sxs-lookup"><span data-stu-id="4b893-174">The following example shows a request to create a standard channel with moderation settings.</span></span> <span data-ttu-id="4b893-175">Эту операцию можно выполнить только для стандартного канала.</span><span class="sxs-lookup"><span data-stu-id="4b893-175">This operation can only be performed for a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b893-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b893-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_with_moderation_settings"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
    "displayName": "TestChannelModeration",
    "description": "Test channel moderation.",
    "membershipType": "standard",
    "moderationSettings": {
        "userNewMessageRestriction": "everyoneExceptGuests",
        "replyRestriction": "everyone",
        "allowNewMessageFromBots": true,
        "allowNewMessageFromConnectors": true
    }
}
```
# <a name="c"></a>[<span data-ttu-id="4b893-177">C#</span><span class="sxs-lookup"><span data-stu-id="4b893-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-with-moderation-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b893-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b893-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-with-moderation-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b893-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b893-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-with-moderation-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b893-180">Java</span><span class="sxs-lookup"><span data-stu-id="4b893-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-with-moderation-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="4b893-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b893-181">Response</span></span>

<span data-ttu-id="4b893-182">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b893-182">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:12b76eea88574bd1969dca37e2b7a819@thread.skype",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19:12b76eea88574bd1969dca37e2b7a819@thread.skype/My%20First%20Private%20Channel?groupId=57fb72d0-d811-46f4-8947-305e6072eaa5&tenantId=0fddfdc5-f319-491f-a514-be1bc1bf9ddc",
    "membershipType": "private"
}
```

## <a name="see-also"></a><span data-ttu-id="4b893-183">См. также</span><span class="sxs-lookup"><span data-stu-id="4b893-183">See also</span></span>

* [<span data-ttu-id="4b893-184">Завершение миграции для канала</span><span class="sxs-lookup"><span data-stu-id="4b893-184">Complete migration for a channel</span></span>](channel-completemigration.md)
* [<span data-ttu-id="4b893-185">Импорт сообщений из сторонних платформ в Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4b893-185">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="4b893-186">Создание команды</span><span class="sxs-lookup"><span data-stu-id="4b893-186">Create team</span></span>](team-post.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
