---
title: Создание канала
description: Создайте новый канал в команде Майкрософт, как указано в теле запроса.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8b2da75127868fb445bbc17f894ecf7fabb33161
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959115"
---
# <a name="create-channel"></a><span data-ttu-id="e57fa-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="e57fa-103">Create channel</span></span>

<span data-ttu-id="e57fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e57fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e57fa-105">Создайте новый [канал](../resources/channel.md) в команде, как указано в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="e57fa-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="e57fa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e57fa-106">Permissions</span></span>

<span data-ttu-id="e57fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e57fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e57fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e57fa-109">Permission type</span></span>      | <span data-ttu-id="e57fa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e57fa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e57fa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e57fa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e57fa-112">Channel. Create, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e57fa-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="e57fa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e57fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e57fa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e57fa-114">Not supported.</span></span>    |
|<span data-ttu-id="e57fa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e57fa-115">Application</span></span> | <span data-ttu-id="e57fa-116">Channel. Create. Group \*, Channel. Create, Branch. Migrate. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e57fa-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="e57fa-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="e57fa-117">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="e57fa-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="e57fa-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="e57fa-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="e57fa-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e57fa-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e57fa-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="e57fa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e57fa-121">Request headers</span></span>

| <span data-ttu-id="e57fa-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e57fa-122">Header</span></span>       | <span data-ttu-id="e57fa-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e57fa-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e57fa-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e57fa-124">Authorization</span></span>  | <span data-ttu-id="e57fa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e57fa-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e57fa-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e57fa-127">Content-Type</span></span>  | <span data-ttu-id="e57fa-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e57fa-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e57fa-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e57fa-130">Request body</span></span>

<span data-ttu-id="e57fa-131">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e57fa-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e57fa-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e57fa-132">Response</span></span>

<span data-ttu-id="e57fa-133">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e57fa-133">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

<span data-ttu-id="e57fa-134">При безуспешном запросе этот метод возвращает код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="e57fa-134">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> <span data-ttu-id="e57fa-135">Ниже перечислены распространенные причины этого отклика.</span><span class="sxs-lookup"><span data-stu-id="e57fa-135">The following are common reasons for this response:</span></span>

* <span data-ttu-id="e57fa-136">Для **createdDateTime** установлено значение в будущем.</span><span class="sxs-lookup"><span data-stu-id="e57fa-136">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="e57fa-137">Параметр **createdDateTime** указан правильно, но отсутствует атрибут экземпляра **channelCreationMode** или ему присвоено недопустимое значение.</span><span class="sxs-lookup"><span data-stu-id="e57fa-137">**createdDateTime** is correctly specified but the **channelCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="examples"></a><span data-ttu-id="e57fa-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="e57fa-138">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="e57fa-139">Пример 1: создание стандартного канала</span><span class="sxs-lookup"><span data-stu-id="e57fa-139">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="e57fa-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e57fa-140">Request</span></span>

<span data-ttu-id="e57fa-141">В приведенном ниже примере показан запрос на создание стандартного канала.</span><span class="sxs-lookup"><span data-stu-id="e57fa-141">The following example shows a request to create a standard channel.</span></span>

# <a name="http"></a>[<span data-ttu-id="e57fa-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e57fa-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```

# <a name="c"></a>[<span data-ttu-id="e57fa-143">C#</span><span class="sxs-lookup"><span data-stu-id="e57fa-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e57fa-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e57fa-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e57fa-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e57fa-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e57fa-146">Java</span><span class="sxs-lookup"><span data-stu-id="e57fa-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e57fa-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e57fa-147">Response</span></span>

<span data-ttu-id="e57fa-148">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e57fa-148">The following example shows the response.</span></span>

> <span data-ttu-id="e57fa-p106">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e57fa-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="e57fa-151">Пример 2: создание закрытого канала от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="e57fa-151">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="e57fa-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e57fa-152">Request</span></span>

<span data-ttu-id="e57fa-153">В приведенном ниже примере показан запрос на создание закрытого канала и Добавление пользователя в качестве владельца группы.</span><span class="sxs-lookup"><span data-stu-id="e57fa-153">The following example shows a request to create a private channel and add a user as an team owner.</span></span>

# <a name="http"></a>[<span data-ttu-id="e57fa-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="e57fa-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{group_id}/channels
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
           "user@odata.bind":"https://graph.microsoft.com/beta/users('{user_id}')",
           "roles":["owner"]
        }
     ]
}
```

# <a name="c"></a>[<span data-ttu-id="e57fa-155">C#</span><span class="sxs-lookup"><span data-stu-id="e57fa-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e57fa-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e57fa-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e57fa-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e57fa-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e57fa-158">Java</span><span class="sxs-lookup"><span data-stu-id="e57fa-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="e57fa-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="e57fa-159">Response</span></span>

<span data-ttu-id="e57fa-160">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e57fa-160">The following example shows the response.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('{group_id}')/channels/$entity",
    "id": "{channel_id}",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/{channel_id}/My%20First%20Private%20Channel?groupId={group_id}&tenantId={tenant_id}",
    "membershipType": "private"
}
```

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="e57fa-161">Пример 3: создание канала в режиме миграции</span><span class="sxs-lookup"><span data-stu-id="e57fa-161">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="e57fa-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="e57fa-162">Request</span></span>

<span data-ttu-id="e57fa-163">В приведенном ниже примере показано, как создать канал для импортированных сообщений.</span><span class="sxs-lookup"><span data-stu-id="e57fa-163">The following example shows how to create a channel for imported messages.</span></span>

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-Type: application/json

{
  "@microsoft.graph.channelCreationMode": "migration",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```

#### <a name="response"></a><span data-ttu-id="e57fa-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="e57fa-164">Response</span></span>

```http
HTTP/1.1 202 Accepted
Location: /teams/{teamId}/channels/{channelId}/operations/{operationId}
Content-Location: /teams/{teamId}/channels/{channelId}
```

## <a name="see-also"></a><span data-ttu-id="e57fa-165">См. также</span><span class="sxs-lookup"><span data-stu-id="e57fa-165">See also</span></span>

* [<span data-ttu-id="e57fa-166">Выполнение переноса для канала</span><span class="sxs-lookup"><span data-stu-id="e57fa-166">Complete migration for a channel</span></span>](channel-completemigration.md)
* [<span data-ttu-id="e57fa-167">Импорт сообщений из сторонних платформ в Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e57fa-167">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="e57fa-168">Создание команды</span><span class="sxs-lookup"><span data-stu-id="e57fa-168">Create team</span></span>](team-post.md)

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
