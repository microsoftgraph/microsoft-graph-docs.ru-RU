---
title: Обновление участника в команде
description: Обнови роль участника в команде.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 41896d37cd8c73d61fac04c3a4386b54f38a2d7a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954071"
---
# <a name="update-member-in-team"></a><span data-ttu-id="c3f03-103">Обновление участника в команде</span><span class="sxs-lookup"><span data-stu-id="c3f03-103">Update member in team</span></span>

<span data-ttu-id="c3f03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3f03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3f03-105">Обновление роли [conversationMember](../resources/conversationmember.md) в [команде.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="c3f03-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3f03-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3f03-106">Permissions</span></span>

<span data-ttu-id="c3f03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3f03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3f03-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3f03-109">Permission Type</span></span>|<span data-ttu-id="c3f03-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3f03-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c3f03-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3f03-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3f03-112">TeamMember.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="c3f03-112">TeamMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="c3f03-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3f03-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3f03-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c3f03-114">Not supported</span></span>|
|<span data-ttu-id="c3f03-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c3f03-115">Application</span></span>|<span data-ttu-id="c3f03-116">TeamMember.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="c3f03-116">TeamMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3f03-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3f03-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="c3f03-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3f03-118">Request headers</span></span>

| <span data-ttu-id="c3f03-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3f03-119">Header</span></span>       | <span data-ttu-id="c3f03-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c3f03-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c3f03-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3f03-121">Authorization</span></span>  | <span data-ttu-id="c3f03-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3f03-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c3f03-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3f03-124">Content-type</span></span> | <span data-ttu-id="c3f03-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3f03-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3f03-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3f03-127">Request body</span></span>

<span data-ttu-id="c3f03-128">В теле запроса укажи значения для обновления соответствующих полей.</span><span class="sxs-lookup"><span data-stu-id="c3f03-128">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="c3f03-129">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="c3f03-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c3f03-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c3f03-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c3f03-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3f03-131">Property</span></span>   | <span data-ttu-id="c3f03-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c3f03-132">Type</span></span> |<span data-ttu-id="c3f03-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c3f03-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3f03-134">roles</span><span class="sxs-lookup"><span data-stu-id="c3f03-134">roles</span></span>|<span data-ttu-id="c3f03-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c3f03-135">string collection</span></span>|<span data-ttu-id="c3f03-136">Роль пользователя.</span><span class="sxs-lookup"><span data-stu-id="c3f03-136">The role for the user.</span></span> <span data-ttu-id="c3f03-137">Должно быть `owner` или пусто.</span><span class="sxs-lookup"><span data-stu-id="c3f03-137">Must be `owner` or empty.</span></span> <span data-ttu-id="c3f03-138">Гостевой пользователь автоматически штампуется `guest` ролью, и это значение не может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="c3f03-138">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="c3f03-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3f03-139">Response</span></span>

<span data-ttu-id="c3f03-140">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект conversationMember](../resources/conversationmember.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c3f03-140">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3f03-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c3f03-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3f03-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3f03-142">Request</span></span>

<span data-ttu-id="c3f03-143">Ниже приводится запрос на применение роли `owner` к существующему члену группы.</span><span class="sxs-lookup"><span data-stu-id="c3f03-143">The following is a request to apply the `owner` role to an existing member of a team.</span></span>


# <a name="http"></a>[<span data-ttu-id="c3f03-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3f03-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_member_2"
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
# <a name="c"></a>[<span data-ttu-id="c3f03-145">C#</span><span class="sxs-lookup"><span data-stu-id="c3f03-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-member-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3f03-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3f03-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-member-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3f03-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3f03-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-member-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3f03-148">Java</span><span class="sxs-lookup"><span data-stu-id="c3f03-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-member-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c3f03-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3f03-149">Response</span></span>

><span data-ttu-id="c3f03-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c3f03-150">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

## <a name="see-also"></a><span data-ttu-id="c3f03-151">См. также</span><span class="sxs-lookup"><span data-stu-id="c3f03-151">See also</span></span>

- [<span data-ttu-id="c3f03-152">Обновление участника в канале</span><span class="sxs-lookup"><span data-stu-id="c3f03-152">Update member in channel</span></span>](channel-update-members.md)

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
