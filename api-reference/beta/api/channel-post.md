---
title: Создание канала
description: Создание нового канала в команде, как указано в теле запроса.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 34576f37e9c635c58843c6f83ace63ced8e48643
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948331"
---
# <a name="create-channel"></a><span data-ttu-id="cc5fd-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="cc5fd-103">Create channel</span></span>

<span data-ttu-id="cc5fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc5fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc5fd-105">Создайте новый [канал](../resources/channel.md) в команде, как указано в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc5fd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc5fd-106">Permissions</span></span>

<span data-ttu-id="cc5fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc5fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc5fd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc5fd-109">Permission type</span></span>      | <span data-ttu-id="cc5fd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc5fd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc5fd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc5fd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc5fd-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc5fd-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="cc5fd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc5fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc5fd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-114">Not supported.</span></span>    |
|<span data-ttu-id="cc5fd-115">Application</span><span class="sxs-lookup"><span data-stu-id="cc5fd-115">Application</span></span> | <span data-ttu-id="cc5fd-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc5fd-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="cc5fd-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="cc5fd-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="cc5fd-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cc5fd-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

> <span data-ttu-id="cc5fd-120">**Примечание.** В будущем Корпорация Майкрософт может потребовать от вас или ваших клиентов уплаты дополнительных сборов в зависимости от количества импортируемых данных с помощью API Teamwork.Migrate.All и/или [переноса.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="cc5fd-120">**Note**: In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported using Teamwork.Migrate.All and/or [migration APIs](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>

## <a name="http-request"></a><span data-ttu-id="cc5fd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc5fd-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="cc5fd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc5fd-122">Request headers</span></span>

| <span data-ttu-id="cc5fd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc5fd-123">Header</span></span>       | <span data-ttu-id="cc5fd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cc5fd-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc5fd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc5fd-125">Authorization</span></span>  | <span data-ttu-id="cc5fd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc5fd-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc5fd-128">Content-Type</span></span>  | <span data-ttu-id="cc5fd-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc5fd-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc5fd-131">Request body</span></span>

<span data-ttu-id="cc5fd-132">В теле запроса поставляем представление JSON объекта [канала.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="cc5fd-132">In the request body, supply a JSON representation of a [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cc5fd-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc5fd-133">Response</span></span>

<span data-ttu-id="cc5fd-134">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-134">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

<span data-ttu-id="cc5fd-135">При безуспешном запросе этот метод возвращает код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-135">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> <span data-ttu-id="cc5fd-136">Ниже перечислены распространенные причины этого отклика.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-136">The following are common reasons for this response:</span></span>

* <span data-ttu-id="cc5fd-137">Для **createdDateTime** установлено значение в будущем.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-137">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="cc5fd-138">**createdDateTime** правильно указывается, но атрибут **экземпляра channelCreationMode** отсутствует или задан для значения недействительным.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-138">**createdDateTime** is correctly specified but the **channelCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="examples"></a><span data-ttu-id="cc5fd-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc5fd-139">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="cc5fd-140">Пример 1. Создание стандартного канала</span><span class="sxs-lookup"><span data-stu-id="cc5fd-140">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="cc5fd-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc5fd-141">Request</span></span>

<span data-ttu-id="cc5fd-142">В следующем примере показан запрос на создание стандартного канала.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-142">The following example shows a request to create a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc5fd-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc5fd-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cc5fd-144">C#</span><span class="sxs-lookup"><span data-stu-id="cc5fd-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc5fd-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc5fd-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc5fd-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc5fd-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc5fd-147">Java</span><span class="sxs-lookup"><span data-stu-id="cc5fd-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="cc5fd-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc5fd-148">Response</span></span>

<span data-ttu-id="cc5fd-149">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-149">The following example shows the response.</span></span>

> <span data-ttu-id="cc5fd-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-150">**Note:** The response object shown here might be shortened for readability.</span></span> 

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

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="cc5fd-151">Пример 2. Создание частного канала от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="cc5fd-151">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="cc5fd-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc5fd-152">Request</span></span>

<span data-ttu-id="cc5fd-153">В следующем примере показан запрос на создание частного канала и добавление пользователя в качестве владельца группы.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-153">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc5fd-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc5fd-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cc5fd-155">C#</span><span class="sxs-lookup"><span data-stu-id="cc5fd-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-private-channel-with-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc5fd-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc5fd-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-private-channel-with-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc5fd-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc5fd-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-private-channel-with-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc5fd-158">Java</span><span class="sxs-lookup"><span data-stu-id="cc5fd-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-private-channel-with-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="cc5fd-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc5fd-159">Response</span></span>

<span data-ttu-id="cc5fd-160">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-160">The following example shows the response.</span></span>

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

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="cc5fd-161">Пример 3. Создание канала в режиме миграции</span><span class="sxs-lookup"><span data-stu-id="cc5fd-161">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="cc5fd-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc5fd-162">Request</span></span>

<span data-ttu-id="cc5fd-163">В следующем примере показано, как создать канал, который будет использоваться для импорта сообщений.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-163">The following example shows how to create a channel that will be used for importing messages.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc5fd-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc5fd-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cc5fd-165">C#</span><span class="sxs-lookup"><span data-stu-id="cc5fd-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-for-migration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc5fd-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc5fd-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-for-migration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc5fd-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc5fd-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-for-migration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc5fd-168">Java</span><span class="sxs-lookup"><span data-stu-id="cc5fd-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-for-migration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cc5fd-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc5fd-169">Response</span></span>

<span data-ttu-id="cc5fd-170">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-170">The following example shows the response.</span></span> <span data-ttu-id="cc5fd-171">Заглавный заглавный пункт Content-Location в ответе указывает путь к каналу, который будет задан.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-171">The Content-Location header in the response specifies the path to the channel that is being provisioned.</span></span>
<span data-ttu-id="cc5fd-172">После предварительного использования этот канал можно использовать для [импорта сообщений.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="cc5fd-172">Once provisioned, this channel can be used for [importing messages](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
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

### <a name="example-4-create-standard-channel-with-moderation-settings"></a><span data-ttu-id="cc5fd-173">Пример 4. Создание стандартного канала с настройками модерации</span><span class="sxs-lookup"><span data-stu-id="cc5fd-173">Example 4: Create standard channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="cc5fd-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc5fd-174">Request</span></span>

<span data-ttu-id="cc5fd-175">В следующем примере показан запрос на создание стандартного канала с настройками модерации.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-175">The following example shows a request to create a standard channel with moderation settings.</span></span> <span data-ttu-id="cc5fd-176">Эта операция может выполняться только для стандартного канала.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-176">This operation can only be performed for a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc5fd-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc5fd-177">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cc5fd-178">C#</span><span class="sxs-lookup"><span data-stu-id="cc5fd-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-with-moderation-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc5fd-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc5fd-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-with-moderation-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc5fd-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc5fd-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-with-moderation-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc5fd-181">Java</span><span class="sxs-lookup"><span data-stu-id="cc5fd-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-with-moderation-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="cc5fd-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc5fd-182">Response</span></span>

<span data-ttu-id="cc5fd-183">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc5fd-183">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="cc5fd-184">См. также</span><span class="sxs-lookup"><span data-stu-id="cc5fd-184">See also</span></span>

* [<span data-ttu-id="cc5fd-185">Полная миграция для канала</span><span class="sxs-lookup"><span data-stu-id="cc5fd-185">Complete migration for a channel</span></span>](channel-completemigration.md)
* [<span data-ttu-id="cc5fd-186">Импорт сообщений из сторонних платформ в Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cc5fd-186">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="cc5fd-187">Создание команды</span><span class="sxs-lookup"><span data-stu-id="cc5fd-187">Create team</span></span>](team-post.md)

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
