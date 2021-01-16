---
title: Добавление участника в канал
description: Добавление участника в канал.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0230eab4a0b07439f21dc0e44c78b707084ec47f
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882516"
---
# <a name="add-member-to-channel"></a><span data-ttu-id="2ba91-103">Добавление участника в канал</span><span class="sxs-lookup"><span data-stu-id="2ba91-103">Add member to channel</span></span>

<span data-ttu-id="2ba91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ba91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ba91-105">Добавление [conversationMember](../resources/conversationmember.md) в [канал.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="2ba91-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span> <span data-ttu-id="2ba91-106">Эта операция разрешена только для каналов со значением **membershipType.** `private`</span><span class="sxs-lookup"><span data-stu-id="2ba91-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ba91-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ba91-107">Permissions</span></span>

<span data-ttu-id="2ba91-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ba91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ba91-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ba91-110">Permission Type</span></span>|<span data-ttu-id="2ba91-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ba91-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="2ba91-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ba91-112">Delegated (work or school account)</span></span>| <span data-ttu-id="2ba91-113">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ba91-113">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="2ba91-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ba91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ba91-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ba91-115">Not supported.</span></span>|
|<span data-ttu-id="2ba91-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2ba91-116">Application</span></span>| <span data-ttu-id="2ba91-117">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ba91-117">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ba91-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ba91-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{team-id}/channels/{channel-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="2ba91-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ba91-119">Request headers</span></span>

| <span data-ttu-id="2ba91-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ba91-120">Header</span></span>       | <span data-ttu-id="2ba91-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2ba91-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ba91-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ba91-122">Authorization</span></span>  | <span data-ttu-id="2ba91-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ba91-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2ba91-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ba91-125">Content-type</span></span> | <span data-ttu-id="2ba91-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ba91-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ba91-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ba91-128">Request body</span></span>

<span data-ttu-id="2ba91-129">Включите в запрос указанные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="2ba91-129">Include the following properties in the request body.</span></span>

| <span data-ttu-id="2ba91-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ba91-130">Property</span></span>   | <span data-ttu-id="2ba91-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2ba91-131">Type</span></span> |<span data-ttu-id="2ba91-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2ba91-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ba91-133">roles</span><span class="sxs-lookup"><span data-stu-id="2ba91-133">roles</span></span>|<span data-ttu-id="2ba91-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2ba91-134">string collection</span></span>|<span data-ttu-id="2ba91-135">Роль пользователя.</span><span class="sxs-lookup"><span data-stu-id="2ba91-135">The role for the user.</span></span> <span data-ttu-id="2ba91-136">Должен быть `owner` пустым или пустым.</span><span class="sxs-lookup"><span data-stu-id="2ba91-136">Must be `owner` or empty.</span></span>|
|<span data-ttu-id="2ba91-137">user</span><span class="sxs-lookup"><span data-stu-id="2ba91-137">user</span></span>|[<span data-ttu-id="2ba91-138">user</span><span class="sxs-lookup"><span data-stu-id="2ba91-138">user</span></span>](../resources/user.md)|<span data-ttu-id="2ba91-139">Пользователь, добавляемой в канал.</span><span class="sxs-lookup"><span data-stu-id="2ba91-139">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="2ba91-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ba91-140">Response</span></span>

<span data-ttu-id="2ba91-141">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ba91-141">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ba91-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ba91-142">Examples</span></span>

### <a name="example-1-add-a-member-to-a-channel"></a><span data-ttu-id="2ba91-143">Пример 1. Добавление участника в канал</span><span class="sxs-lookup"><span data-stu-id="2ba91-143">Example 1: Add a member to a channel</span></span>

#### <a name="request"></a><span data-ttu-id="2ba91-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ba91-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2ba91-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ba91-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_add_member"
} -->
```http
POST https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members
Content-type: application/json
Content-length: 100

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": ["owner"],
    "user@odata.bind": "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
}
```
# <a name="c"></a>[<span data-ttu-id="2ba91-146">C#</span><span class="sxs-lookup"><span data-stu-id="2ba91-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-add-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ba91-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ba91-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-add-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ba91-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ba91-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-add-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ba91-149">Java</span><span class="sxs-lookup"><span data-stu-id="2ba91-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-add-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2ba91-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ba91-150">Response</span></span>

><span data-ttu-id="2ba91-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ba91-151">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

### <a name="example-2-add-a-member-with-the-owner-role-to-a-channel"></a><span data-ttu-id="2ba91-152">Пример 2. Добавление участника с ролью владельца в канал</span><span class="sxs-lookup"><span data-stu-id="2ba91-152">Example 2: Add a member with the owner role to a channel</span></span>

#### <a name="request"></a><span data-ttu-id="2ba91-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ba91-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "channel_add_member"
} -->

```http
POST https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members
Content-type: application/json
Content-length: 100

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": ["owner"],
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
}
```

#### <a name="response"></a><span data-ttu-id="2ba91-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ba91-154">Response</span></span>

<span data-ttu-id="2ba91-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2ba91-155">Here is an example of the response.</span></span>

><span data-ttu-id="2ba91-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ba91-156">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a><span data-ttu-id="2ba91-157">См. также</span><span class="sxs-lookup"><span data-stu-id="2ba91-157">See also</span></span>

- [<span data-ttu-id="2ba91-158">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="2ba91-158">Add member to team</span></span>](team-post-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add member to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
