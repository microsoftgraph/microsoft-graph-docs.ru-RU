---
title: Обновление элемента в канале
description: Обновление роли участника в канале.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 20c6acd623d3ca4a352902fd57a0bd8b1074134c
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387796"
---
# <a name="update-member-in-channel"></a><span data-ttu-id="504a5-103">Обновление элемента в канале</span><span class="sxs-lookup"><span data-stu-id="504a5-103">Update member in channel</span></span>

<span data-ttu-id="504a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="504a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="504a5-105">Обновление роли [конверсатионмембер](../resources/conversationmember.md) в [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="504a5-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="504a5-106">Эта операция разрешена только для каналов со значением **мембершиптипе** `private` .</span><span class="sxs-lookup"><span data-stu-id="504a5-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>

## <a name="permissions"></a><span data-ttu-id="504a5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="504a5-107">Permissions</span></span>

<span data-ttu-id="504a5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="504a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="504a5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="504a5-110">Permission Type</span></span>|<span data-ttu-id="504a5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="504a5-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="504a5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="504a5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="504a5-113">Чаннелмембер. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="504a5-113">ChannelMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="504a5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="504a5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="504a5-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="504a5-115">Not supported</span></span>|
|<span data-ttu-id="504a5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="504a5-116">Application</span></span>|<span data-ttu-id="504a5-117">Чаннелмембер. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="504a5-117">ChannelMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="504a5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="504a5-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="504a5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="504a5-119">Request headers</span></span>

| <span data-ttu-id="504a5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="504a5-120">Header</span></span>       | <span data-ttu-id="504a5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="504a5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="504a5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="504a5-122">Authorization</span></span>  | <span data-ttu-id="504a5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="504a5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="504a5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="504a5-125">Content-type</span></span> | <span data-ttu-id="504a5-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="504a5-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="504a5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="504a5-128">Request body</span></span>

<span data-ttu-id="504a5-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="504a5-129">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="504a5-130">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="504a5-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="504a5-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="504a5-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="504a5-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="504a5-132">Property</span></span>   | <span data-ttu-id="504a5-133">Тип</span><span class="sxs-lookup"><span data-stu-id="504a5-133">Type</span></span> |<span data-ttu-id="504a5-134">Описание</span><span class="sxs-lookup"><span data-stu-id="504a5-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="504a5-135">roles</span><span class="sxs-lookup"><span data-stu-id="504a5-135">roles</span></span>|<span data-ttu-id="504a5-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="504a5-136">string collection</span></span>|<span data-ttu-id="504a5-137">Роль пользователя.</span><span class="sxs-lookup"><span data-stu-id="504a5-137">The role for the user.</span></span> <span data-ttu-id="504a5-138">Должно быть `owner` или пустым.</span><span class="sxs-lookup"><span data-stu-id="504a5-138">Must be `owner` or empty.</span></span> <span data-ttu-id="504a5-139">Пользователи с ролью "гость" автоматически отмечаются `guest` ролью, и это значение не может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="504a5-139">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="504a5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="504a5-140">Response</span></span>

<span data-ttu-id="504a5-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [конверсатионмембер](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="504a5-141">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="504a5-142">Пример</span><span class="sxs-lookup"><span data-stu-id="504a5-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="504a5-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="504a5-143">Request</span></span>

<span data-ttu-id="504a5-144">Ниже приведен запрос на применение `owner` роли к существующему участнику канала.</span><span class="sxs-lookup"><span data-stu-id="504a5-144">The following is a request to apply the `owner` role to an existing member of a channel.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_member"
} -->
```http
PATCH https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```

### <a name="response"></a><span data-ttu-id="504a5-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="504a5-145">Response</span></span>

><span data-ttu-id="504a5-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="504a5-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
## <a name="see-also"></a><span data-ttu-id="504a5-147">См. также</span><span class="sxs-lookup"><span data-stu-id="504a5-147">See also</span></span>

- [<span data-ttu-id="504a5-148">Изменение роли участника в команде</span><span class="sxs-lookup"><span data-stu-id="504a5-148">Update member's role in a team</span></span>](team-update-members.md)
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
