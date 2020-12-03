---
title: Добавление участника в канал
description: Добавление участника в канал.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 66a3d8358ffe6a968f6f7f681e64236c7ecd665e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523319"
---
# <a name="add-member-to-channel"></a><span data-ttu-id="95163-103">Добавление участника в канал</span><span class="sxs-lookup"><span data-stu-id="95163-103">Add member to channel</span></span>

<span data-ttu-id="95163-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95163-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95163-105">Добавление [конверсатионмембер](../resources/conversationmember.md) к [каналу](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="95163-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span> <span data-ttu-id="95163-106">Эта операция разрешена только для каналов со значением **мембершиптипе** `private` .</span><span class="sxs-lookup"><span data-stu-id="95163-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>

## <a name="permissions"></a><span data-ttu-id="95163-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95163-107">Permissions</span></span>

<span data-ttu-id="95163-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95163-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95163-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95163-110">Permission Type</span></span>|<span data-ttu-id="95163-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95163-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="95163-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95163-112">Delegated (work or school account)</span></span>| <span data-ttu-id="95163-113">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95163-113">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="95163-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95163-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95163-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95163-115">Not supported.</span></span>|
|<span data-ttu-id="95163-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="95163-116">Application</span></span>| <span data-ttu-id="95163-117">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95163-117">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95163-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95163-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{team-id}/channels/{channel-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="95163-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95163-119">Request headers</span></span>

| <span data-ttu-id="95163-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95163-120">Header</span></span>       | <span data-ttu-id="95163-121">Значение</span><span class="sxs-lookup"><span data-stu-id="95163-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95163-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95163-122">Authorization</span></span>  | <span data-ttu-id="95163-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95163-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="95163-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95163-125">Content-type</span></span> | <span data-ttu-id="95163-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95163-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95163-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95163-128">Request body</span></span>

<span data-ttu-id="95163-129">Включите в запрос указанные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="95163-129">Include the following properties in the request body.</span></span>

| <span data-ttu-id="95163-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="95163-130">Property</span></span>   | <span data-ttu-id="95163-131">Тип</span><span class="sxs-lookup"><span data-stu-id="95163-131">Type</span></span> |<span data-ttu-id="95163-132">Описание</span><span class="sxs-lookup"><span data-stu-id="95163-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95163-133">roles</span><span class="sxs-lookup"><span data-stu-id="95163-133">roles</span></span>|<span data-ttu-id="95163-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="95163-134">string collection</span></span>|<span data-ttu-id="95163-135">Роль пользователя.</span><span class="sxs-lookup"><span data-stu-id="95163-135">The role for the user.</span></span> <span data-ttu-id="95163-136">Должно быть `owner` или пустым.</span><span class="sxs-lookup"><span data-stu-id="95163-136">Must be `owner` or empty.</span></span>|
|<span data-ttu-id="95163-137">user</span><span class="sxs-lookup"><span data-stu-id="95163-137">user</span></span>|[<span data-ttu-id="95163-138">user</span><span class="sxs-lookup"><span data-stu-id="95163-138">user</span></span>](../resources/user.md)|<span data-ttu-id="95163-139">Пользователь, добавляемый в канал.</span><span class="sxs-lookup"><span data-stu-id="95163-139">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="95163-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="95163-140">Response</span></span>

<span data-ttu-id="95163-141">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95163-141">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95163-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="95163-142">Examples</span></span>

### <a name="example-1-add-a-member-to-a-channel"></a><span data-ttu-id="95163-143">Пример 1: Добавление участника в канал</span><span class="sxs-lookup"><span data-stu-id="95163-143">Example 1: Add a member to a channel</span></span>

#### <a name="request"></a><span data-ttu-id="95163-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="95163-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="95163-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="95163-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_add_member"
} -->
```http
POST https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members
Content-type: application/json
Content-length: 100

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": ["owner"],
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
}
```
# <a name="javascript"></a>[<span data-ttu-id="95163-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95163-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-add-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95163-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95163-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-add-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="95163-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="95163-148">Response</span></span>

><span data-ttu-id="95163-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="95163-149">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

### <a name="example-2-add-a-member-with-the-owner-role-to-a-channel"></a><span data-ttu-id="95163-150">Пример 2: Добавление члена с ролью "владелец" в канал</span><span class="sxs-lookup"><span data-stu-id="95163-150">Example 2: Add a member with the owner role to a channel</span></span>

#### <a name="request"></a><span data-ttu-id="95163-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="95163-151">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "channel_add_member"
} -->

```http
POST https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members
```

#### <a name="response"></a><span data-ttu-id="95163-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="95163-152">Response</span></span>

<span data-ttu-id="95163-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="95163-153">Here is an example of the response.</span></span>

><span data-ttu-id="95163-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="95163-154">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a><span data-ttu-id="95163-155">См. также</span><span class="sxs-lookup"><span data-stu-id="95163-155">See also</span></span>

- [<span data-ttu-id="95163-156">Добавление участника в группу</span><span class="sxs-lookup"><span data-stu-id="95163-156">Add member to team</span></span>](team-post-members.md)

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
