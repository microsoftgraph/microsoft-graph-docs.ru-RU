---
title: Создание канала
description: Создание нового канала в команде, как указано в теле запроса.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ac06a2898662ce13db588ea0f243f6d3eea65805
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508494"
---
# <a name="create-channel"></a><span data-ttu-id="6b472-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="6b472-103">Create channel</span></span>

<span data-ttu-id="6b472-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b472-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b472-105">Создайте новый [канал](../resources/channel.md) в команде, как указано в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="6b472-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b472-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b472-106">Permissions</span></span>

<span data-ttu-id="6b472-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b472-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b472-109">Permission type</span></span>      | <span data-ttu-id="6b472-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b472-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b472-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b472-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b472-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b472-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="6b472-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b472-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b472-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b472-114">Not supported.</span></span>    |
|<span data-ttu-id="6b472-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b472-115">Application</span></span> | <span data-ttu-id="6b472-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b472-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="6b472-117">**Примечания.** Разрешения, отмеченные \* использование [согласия, определенного для ресурсов.]( https://aka.ms/teams-rsc)</span><span class="sxs-lookup"><span data-stu-id="6b472-117">**Notes**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>
>
> <span data-ttu-id="6b472-118">Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="6b472-118">This API supports admin permissions.</span></span> <span data-ttu-id="6b472-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="6b472-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>
>
> <span data-ttu-id="6b472-120">В будущем Корпорация Майкрософт может потребовать от вас или ваших клиентов уплаты дополнительных сборов в зависимости от объема импортируемых данных с помощью API Teamwork.Migrate.All и/или [переноса.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="6b472-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported using Teamwork.Migrate.All and/or [migration APIs](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>

## <a name="http-request"></a><span data-ttu-id="6b472-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b472-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="6b472-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b472-122">Request headers</span></span>

| <span data-ttu-id="6b472-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b472-123">Header</span></span>       | <span data-ttu-id="6b472-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6b472-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b472-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b472-125">Authorization</span></span>  | <span data-ttu-id="6b472-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b472-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6b472-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b472-128">Content-Type</span></span>  | <span data-ttu-id="6b472-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b472-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b472-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b472-131">Request body</span></span>

<span data-ttu-id="6b472-132">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b472-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6b472-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b472-133">Response</span></span>

<span data-ttu-id="6b472-134">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b472-134">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b472-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b472-135">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="6b472-136">Пример 1. Создание стандартного канала</span><span class="sxs-lookup"><span data-stu-id="6b472-136">Example 1: Create a standard channel</span></span>
#### <a name="request"></a><span data-ttu-id="6b472-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b472-137">Request</span></span>

<span data-ttu-id="6b472-138">В следующем примере показан запрос на создание стандартного канала.</span><span class="sxs-lookup"><span data-stu-id="6b472-138">The following example shows a request to create a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="6b472-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b472-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```
# <a name="c"></a>[<span data-ttu-id="6b472-140">C#</span><span class="sxs-lookup"><span data-stu-id="6b472-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b472-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b472-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b472-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b472-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b472-143">Java</span><span class="sxs-lookup"><span data-stu-id="6b472-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="6b472-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b472-144">Response</span></span>

<span data-ttu-id="6b472-145">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b472-145">The following example shows the response.</span></span>

> <span data-ttu-id="6b472-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6b472-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}-->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
  "id": "19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="6b472-147">Пример 2. Создание частного канала от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="6b472-147">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="6b472-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b472-148">Request</span></span>

<span data-ttu-id="6b472-149">В следующем примере показан запрос на создание частного канала и добавление пользователя в качестве владельца группы.</span><span class="sxs-lookup"><span data-stu-id="6b472-149">The following example shows a request to create a private channel and add a user as an team owner.</span></span>



# <a name="http"></a>[<span data-ttu-id="6b472-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b472-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
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
           "user@odata.bind":"https://graph.microsoft.com/v1.0/users('62855810-484b-4823-9e01-60667f8b12ae')",
           "roles":["owner"]
        }
     ]
}
```
# <a name="c"></a>[<span data-ttu-id="6b472-151">C#</span><span class="sxs-lookup"><span data-stu-id="6b472-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b472-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b472-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b472-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b472-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b472-154">Java</span><span class="sxs-lookup"><span data-stu-id="6b472-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a><span data-ttu-id="6b472-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b472-155">Response</span></span>

<span data-ttu-id="6b472-156">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b472-156">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}-->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:33b76eea88574bd1969dca37e2b7a819@thread.skype",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/My%20First%20Private%20Channel?groupId=57fb72d0-d811-46f4-8947-305e6072eaa5&tenantId=0fddfdc5-f319-491f-a514-be1bc1bf9ddc",
    "membershipType": "private"
}
```

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="6b472-157">Пример 3. Создание канала в режиме миграции</span><span class="sxs-lookup"><span data-stu-id="6b472-157">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="6b472-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b472-158">Request</span></span>

<span data-ttu-id="6b472-159">В следующем примере показано, как создать канал, который будет использоваться для импорта сообщений.</span><span class="sxs-lookup"><span data-stu-id="6b472-159">The following example shows how to create a channel that will be used for importing messages.</span></span>



# <a name="http"></a>[<span data-ttu-id="6b472-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b472-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_for_migration"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-Type: application/json

{
  "@microsoft.graph.channelCreationMode": "migration",
  "displayName": "Import_150958_99z",
  "description": "Import_150958_99z",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```
# <a name="c"></a>[<span data-ttu-id="6b472-161">C#</span><span class="sxs-lookup"><span data-stu-id="6b472-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-for-migration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b472-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b472-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-for-migration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b472-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b472-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-for-migration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b472-164">Java</span><span class="sxs-lookup"><span data-stu-id="6b472-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-for-migration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="6b472-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b472-165">Response</span></span>

<span data-ttu-id="6b472-166">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b472-166">The following example shows the response.</span></span> <span data-ttu-id="6b472-167">Заглавный заглавный пункт Content-Location в ответе указывает путь к каналу, который будет задан.</span><span class="sxs-lookup"><span data-stu-id="6b472-167">The Content-Location header in the response specifies the path to the channel that is being provisioned.</span></span>
<span data-ttu-id="6b472-168">После предварительного использования этот канал можно использовать для [импорта сообщений.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="6b472-168">Once provisioned, this channel can be used for [importing messages](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_channel_for_migration",
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 201 Created
Location: /teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:987c7a9fbe6447ccb3ea31bcded5c75c@thread.tacv2",
    "createdDateTime": null,
    "displayName": "Import_150958_99z",
    "description": "Import_150958_99z",
    "isFavoriteByDefault": null,
    "email": null,
    "webUrl": null,
    "membershipType": null,
    "moderationSettings": null
}
```

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
