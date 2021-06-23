---
title: Обновление участника в канале
description: Обновление роли участника в канале.
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f94bb69d314eba40ce4ee4c68f1c784b9685c8ad
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059921"
---
# <a name="update-member-in-channel"></a><span data-ttu-id="d7997-103">Обновление участника в канале</span><span class="sxs-lookup"><span data-stu-id="d7997-103">Update member in channel</span></span>

<span data-ttu-id="d7997-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7997-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7997-105">Обновление роли [conversationMember](../resources/conversationmember.md) в [канале.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="d7997-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="d7997-106">Эта операция разрешена только для каналов со значением **membershipType** `private` .</span><span class="sxs-lookup"><span data-stu-id="d7997-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7997-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7997-107">Permissions</span></span>

<span data-ttu-id="d7997-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7997-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7997-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7997-110">Permission Type</span></span>|<span data-ttu-id="d7997-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7997-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="d7997-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7997-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7997-113">ChannelMember.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="d7997-113">ChannelMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="d7997-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7997-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7997-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d7997-115">Not supported</span></span>|
|<span data-ttu-id="d7997-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d7997-116">Application</span></span>|<span data-ttu-id="d7997-117">ChannelMember.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="d7997-117">ChannelMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7997-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7997-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="d7997-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7997-119">Request headers</span></span>

| <span data-ttu-id="d7997-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7997-120">Header</span></span>       | <span data-ttu-id="d7997-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d7997-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d7997-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7997-122">Authorization</span></span>  | <span data-ttu-id="d7997-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7997-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d7997-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7997-125">Content-type</span></span> | <span data-ttu-id="d7997-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7997-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7997-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7997-128">Request body</span></span>

<span data-ttu-id="d7997-129">В теле запроса укажи значения для обновления соответствующих полей.</span><span class="sxs-lookup"><span data-stu-id="d7997-129">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="d7997-130">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="d7997-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d7997-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d7997-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d7997-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7997-132">Property</span></span>   | <span data-ttu-id="d7997-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d7997-133">Type</span></span> |<span data-ttu-id="d7997-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d7997-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7997-135">roles</span><span class="sxs-lookup"><span data-stu-id="d7997-135">roles</span></span>|<span data-ttu-id="d7997-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d7997-136">string collection</span></span>|<span data-ttu-id="d7997-137">Роль пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7997-137">The role for the user.</span></span> <span data-ttu-id="d7997-138">Должно быть `owner` или пусто.</span><span class="sxs-lookup"><span data-stu-id="d7997-138">Must be `owner` or empty.</span></span> <span data-ttu-id="d7997-139">Гостевой пользователь автоматически штампуется `guest` ролью, и это значение не может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="d7997-139">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="d7997-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7997-140">Response</span></span>

<span data-ttu-id="d7997-141">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект conversationMember](../resources/conversationmember.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d7997-141">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7997-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d7997-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7997-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7997-143">Request</span></span>

<span data-ttu-id="d7997-144">Ниже приводится запрос на применение роли к `owner` существующему члену канала.</span><span class="sxs-lookup"><span data-stu-id="d7997-144">The following is a request to apply the `owner` role to an existing member of a channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7997-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7997-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_member_1"
} -->
```http
PATCH https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```
# <a name="c"></a>[<span data-ttu-id="d7997-146">C#</span><span class="sxs-lookup"><span data-stu-id="d7997-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-member-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7997-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7997-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-member-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7997-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7997-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-member-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7997-149">Java</span><span class="sxs-lookup"><span data-stu-id="d7997-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-member-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d7997-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7997-150">Response</span></span>

><span data-ttu-id="d7997-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d7997-151">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 475

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a><span data-ttu-id="d7997-152">См. также</span><span class="sxs-lookup"><span data-stu-id="d7997-152">See also</span></span>

- [<span data-ttu-id="d7997-153">Обновление роли участника в команде</span><span class="sxs-lookup"><span data-stu-id="d7997-153">Update member's role in a team</span></span>](team-update-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "update role of channel member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
