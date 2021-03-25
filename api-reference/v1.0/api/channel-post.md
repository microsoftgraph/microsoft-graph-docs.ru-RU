---
title: Создание канала
description: Создание нового канала в команде, как указано в теле запроса.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7ab9a2d0bdd204e77b9bc149860e9fdfab9d2fcf
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202697"
---
# <a name="create-channel"></a><span data-ttu-id="4d6aa-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="4d6aa-103">Create channel</span></span>

<span data-ttu-id="4d6aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d6aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4d6aa-105">Создайте новый [канал](../resources/channel.md) в команде, как указано в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d6aa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d6aa-106">Permissions</span></span>

<span data-ttu-id="4d6aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d6aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d6aa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d6aa-109">Permission type</span></span>      | <span data-ttu-id="4d6aa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d6aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d6aa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d6aa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4d6aa-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d6aa-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="4d6aa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d6aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d6aa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-114">Not supported.</span></span>    |
|<span data-ttu-id="4d6aa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d6aa-115">Application</span></span> | <span data-ttu-id="4d6aa-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d6aa-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="4d6aa-117">**Примечания.** Разрешения, отмеченные \* использование [согласия, определенного для ресурсов.]( https://aka.ms/teams-rsc)</span><span class="sxs-lookup"><span data-stu-id="4d6aa-117">**Notes**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>
>
> <span data-ttu-id="4d6aa-118">Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-118">This API supports admin permissions.</span></span> <span data-ttu-id="4d6aa-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>
>
> <span data-ttu-id="4d6aa-120">В будущем Корпорация Майкрософт может потребовать от вас или ваших клиентов уплаты дополнительных сборов в зависимости от объема импортируемых данных с помощью API Teamwork.Migrate.All и/или [переноса.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="4d6aa-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported using Teamwork.Migrate.All and/or [migration APIs](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>

## <a name="http-request"></a><span data-ttu-id="4d6aa-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d6aa-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="4d6aa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d6aa-122">Request headers</span></span>

| <span data-ttu-id="4d6aa-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d6aa-123">Header</span></span>       | <span data-ttu-id="4d6aa-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4d6aa-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d6aa-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d6aa-125">Authorization</span></span>  | <span data-ttu-id="4d6aa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4d6aa-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d6aa-128">Content-Type</span></span>  | <span data-ttu-id="4d6aa-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d6aa-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d6aa-131">Request body</span></span>

<span data-ttu-id="4d6aa-132">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4d6aa-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d6aa-133">Response</span></span>

<span data-ttu-id="4d6aa-134">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-134">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d6aa-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="4d6aa-135">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="4d6aa-136">Пример 1. Создание стандартного канала</span><span class="sxs-lookup"><span data-stu-id="4d6aa-136">Example 1: Create a standard channel</span></span>
#### <a name="request"></a><span data-ttu-id="4d6aa-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d6aa-137">Request</span></span>

<span data-ttu-id="4d6aa-138">В следующем примере показан запрос на создание стандартного канала.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-138">The following example shows a request to create a standard channel.</span></span>

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


#### <a name="response"></a><span data-ttu-id="4d6aa-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d6aa-139">Response</span></span>

<span data-ttu-id="4d6aa-140">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-140">The following example shows the response.</span></span>

> <span data-ttu-id="4d6aa-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="4d6aa-142">Пример 2. Создание частного канала от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="4d6aa-142">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="4d6aa-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d6aa-143">Request</span></span>

<span data-ttu-id="4d6aa-144">В следующем примере показан запрос на создание частного канала и добавление пользователя в качестве владельца группы.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-144">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


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



#### <a name="response"></a><span data-ttu-id="4d6aa-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d6aa-145">Response</span></span>

<span data-ttu-id="4d6aa-146">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-146">The following example shows the response.</span></span>

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

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="4d6aa-147">Пример 3. Создание канала в режиме миграции</span><span class="sxs-lookup"><span data-stu-id="4d6aa-147">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="4d6aa-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d6aa-148">Request</span></span>

<span data-ttu-id="4d6aa-149">В следующем примере показано, как создать канал, который будет использоваться для импорта сообщений.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-149">The following example shows how to create a channel that will be used for importing messages.</span></span>


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


#### <a name="response"></a><span data-ttu-id="4d6aa-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d6aa-150">Response</span></span>

<span data-ttu-id="4d6aa-151">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-151">The following example shows the response.</span></span> <span data-ttu-id="4d6aa-152">Заглавный заглавный пункт Content-Location в ответе указывает путь к каналу, который будет задан.</span><span class="sxs-lookup"><span data-stu-id="4d6aa-152">The Content-Location header in the response specifies the path to the channel that is being provisioned.</span></span>
<span data-ttu-id="4d6aa-153">После предварительного использования этот канал можно использовать для [импорта сообщений.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="4d6aa-153">Once provisioned, this channel can be used for [importing messages](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
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
