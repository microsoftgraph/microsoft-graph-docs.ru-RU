---
title: Обновление члена группы
description: Обновление роли участника в команде.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4183e4389e99a824237a1b239be94124c9cd9d1c
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387923"
---
# <a name="update-member-in-team"></a><span data-ttu-id="b415a-103">Обновление члена группы</span><span class="sxs-lookup"><span data-stu-id="b415a-103">Update member in team</span></span>

<span data-ttu-id="b415a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b415a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b415a-105">Обновление роли [конверсатионмембер](../resources/conversationmember.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b415a-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b415a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b415a-106">Permissions</span></span>

<span data-ttu-id="b415a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b415a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b415a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b415a-109">Permission Type</span></span>|<span data-ttu-id="b415a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b415a-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="b415a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b415a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b415a-112">Теаммембер. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="b415a-112">TeamMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="b415a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b415a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b415a-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b415a-114">Not supported</span></span>|
|<span data-ttu-id="b415a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b415a-115">Application</span></span>|<span data-ttu-id="b415a-116">Теаммембер. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="b415a-116">TeamMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b415a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b415a-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="b415a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b415a-118">Request headers</span></span>

| <span data-ttu-id="b415a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b415a-119">Header</span></span>       | <span data-ttu-id="b415a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b415a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b415a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b415a-121">Authorization</span></span>  | <span data-ttu-id="b415a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b415a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b415a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b415a-124">Content-type</span></span> | <span data-ttu-id="b415a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b415a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b415a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b415a-127">Request body</span></span>

<span data-ttu-id="b415a-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b415a-128">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="b415a-129">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="b415a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b415a-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b415a-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b415a-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="b415a-131">Property</span></span>   | <span data-ttu-id="b415a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b415a-132">Type</span></span> |<span data-ttu-id="b415a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b415a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b415a-134">roles</span><span class="sxs-lookup"><span data-stu-id="b415a-134">roles</span></span>|<span data-ttu-id="b415a-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b415a-135">string collection</span></span>|<span data-ttu-id="b415a-136">Роль пользователя.</span><span class="sxs-lookup"><span data-stu-id="b415a-136">The role for the user.</span></span> <span data-ttu-id="b415a-137">Должно быть `owner` или пустым.</span><span class="sxs-lookup"><span data-stu-id="b415a-137">Must be `owner` or empty.</span></span> <span data-ttu-id="b415a-138">Пользователи с ролью "гость" автоматически отмечаются `guest` ролью, и это значение не может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="b415a-138">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="b415a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b415a-139">Response</span></span>

<span data-ttu-id="b415a-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [конверсатионмембер](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b415a-140">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b415a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="b415a-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b415a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b415a-142">Request</span></span>

<span data-ttu-id="b415a-143">Ниже приведен запрос на применение `owner` роли к существующему участнику команды.</span><span class="sxs-lookup"><span data-stu-id="b415a-143">The following is a request to apply the `owner` role to an existing member of a team.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_member"
} -->
```http
PATCH https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```

### <a name="response"></a><span data-ttu-id="b415a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b415a-144">Response</span></span>

><span data-ttu-id="b415a-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b415a-145">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a><span data-ttu-id="b415a-146">См. также</span><span class="sxs-lookup"><span data-stu-id="b415a-146">See also</span></span>

- [<span data-ttu-id="b415a-147">Обновление элемента в канале</span><span class="sxs-lookup"><span data-stu-id="b415a-147">Update member in channel</span></span>](channel-update-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "update role of team member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
