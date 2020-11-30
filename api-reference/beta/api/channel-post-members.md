---
title: Добавление участника в канал
description: Добавление участника в канал.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d5d16691b859955b11292c1f9997be3cc4b366e3
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387919"
---
# <a name="add-member-to-channel"></a><span data-ttu-id="fd94e-103">Добавление участника в канал</span><span class="sxs-lookup"><span data-stu-id="fd94e-103">Add member to channel</span></span>

<span data-ttu-id="fd94e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd94e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd94e-105">Добавление [конверсатионмембер](../resources/conversationmember.md) к [каналу](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="fd94e-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span> <span data-ttu-id="fd94e-106">Эта операция разрешена только для каналов со значением **мембершиптипе** `private` .</span><span class="sxs-lookup"><span data-stu-id="fd94e-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd94e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd94e-107">Permissions</span></span>

<span data-ttu-id="fd94e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd94e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd94e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd94e-110">Permission Type</span></span>|<span data-ttu-id="fd94e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd94e-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="fd94e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd94e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="fd94e-113">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd94e-113">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="fd94e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd94e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd94e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd94e-115">Not supported.</span></span>|
|<span data-ttu-id="fd94e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fd94e-116">Application</span></span>| <span data-ttu-id="fd94e-117">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd94e-117">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd94e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd94e-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{team-id}/channels/{channel-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="fd94e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd94e-119">Request headers</span></span>

| <span data-ttu-id="fd94e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd94e-120">Header</span></span>       | <span data-ttu-id="fd94e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fd94e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd94e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd94e-122">Authorization</span></span>  | <span data-ttu-id="fd94e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd94e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fd94e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd94e-125">Content-type</span></span> | <span data-ttu-id="fd94e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd94e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd94e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd94e-128">Request body</span></span>

<span data-ttu-id="fd94e-129">Включите в запрос указанные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="fd94e-129">Include the following properties in the request body.</span></span>

| <span data-ttu-id="fd94e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd94e-130">Property</span></span>   | <span data-ttu-id="fd94e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fd94e-131">Type</span></span> |<span data-ttu-id="fd94e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fd94e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd94e-133">roles</span><span class="sxs-lookup"><span data-stu-id="fd94e-133">roles</span></span>|<span data-ttu-id="fd94e-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fd94e-134">string collection</span></span>|<span data-ttu-id="fd94e-135">Роль пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd94e-135">The role for the user.</span></span> <span data-ttu-id="fd94e-136">Должно быть `owner` или пустым.</span><span class="sxs-lookup"><span data-stu-id="fd94e-136">Must be `owner` or empty.</span></span>|
|<span data-ttu-id="fd94e-137">user</span><span class="sxs-lookup"><span data-stu-id="fd94e-137">user</span></span>|[<span data-ttu-id="fd94e-138">user</span><span class="sxs-lookup"><span data-stu-id="fd94e-138">user</span></span>](../resources/user.md)|<span data-ttu-id="fd94e-139">Пользователь, добавляемый в канал.</span><span class="sxs-lookup"><span data-stu-id="fd94e-139">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="fd94e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd94e-140">Response</span></span>

<span data-ttu-id="fd94e-141">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd94e-141">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd94e-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="fd94e-142">Examples</span></span>

### <a name="example-1-add-a-member-to-a-channel"></a><span data-ttu-id="fd94e-143">Пример 1: Добавление участника в канал</span><span class="sxs-lookup"><span data-stu-id="fd94e-143">Example 1: Add a member to a channel</span></span>

#### <a name="request"></a><span data-ttu-id="fd94e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd94e-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "channel_add_member"
} -->
```http
POST https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members
```

#### <a name="response"></a><span data-ttu-id="fd94e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd94e-145">Response</span></span>

><span data-ttu-id="fd94e-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fd94e-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

### <a name="example-2-add-a-member-with-the-owner-role-to-a-channel"></a><span data-ttu-id="fd94e-147">Пример 2: Добавление члена с ролью "владелец" в канал</span><span class="sxs-lookup"><span data-stu-id="fd94e-147">Example 2: Add a member with the owner role to a channel</span></span>

#### <a name="request"></a><span data-ttu-id="fd94e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd94e-148">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="fd94e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd94e-149">Response</span></span>

<span data-ttu-id="fd94e-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd94e-150">Here is an example of the response.</span></span>

><span data-ttu-id="fd94e-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fd94e-151">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

## <a name="see-also"></a><span data-ttu-id="fd94e-152">См. также</span><span class="sxs-lookup"><span data-stu-id="fd94e-152">See also</span></span>

- [<span data-ttu-id="fd94e-153">Добавление участника в группу</span><span class="sxs-lookup"><span data-stu-id="fd94e-153">Add member to team</span></span>](team-post-members.md)

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
