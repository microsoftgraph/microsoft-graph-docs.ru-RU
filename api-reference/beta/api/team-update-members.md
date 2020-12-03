---
title: Обновление члена группы
description: Обновление роли участника в команде.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7bafea4c6082f77e247d290b35d778f34cdd18a6
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523905"
---
# <a name="update-member-in-team"></a><span data-ttu-id="9ea58-103">Обновление члена группы</span><span class="sxs-lookup"><span data-stu-id="9ea58-103">Update member in team</span></span>

<span data-ttu-id="9ea58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ea58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ea58-105">Обновление роли [конверсатионмембер](../resources/conversationmember.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="9ea58-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ea58-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ea58-106">Permissions</span></span>

<span data-ttu-id="9ea58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ea58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ea58-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ea58-109">Permission Type</span></span>|<span data-ttu-id="9ea58-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ea58-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9ea58-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ea58-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ea58-112">Теаммембер. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="9ea58-112">TeamMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="9ea58-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ea58-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ea58-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9ea58-114">Not supported</span></span>|
|<span data-ttu-id="9ea58-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9ea58-115">Application</span></span>|<span data-ttu-id="9ea58-116">Теаммембер. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="9ea58-116">TeamMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ea58-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ea58-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="9ea58-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ea58-118">Request headers</span></span>

| <span data-ttu-id="9ea58-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ea58-119">Header</span></span>       | <span data-ttu-id="9ea58-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9ea58-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ea58-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ea58-121">Authorization</span></span>  | <span data-ttu-id="9ea58-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ea58-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9ea58-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ea58-124">Content-type</span></span> | <span data-ttu-id="9ea58-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ea58-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ea58-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ea58-127">Request body</span></span>

<span data-ttu-id="9ea58-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="9ea58-128">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="9ea58-129">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="9ea58-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9ea58-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9ea58-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9ea58-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ea58-131">Property</span></span>   | <span data-ttu-id="9ea58-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9ea58-132">Type</span></span> |<span data-ttu-id="9ea58-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9ea58-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ea58-134">roles</span><span class="sxs-lookup"><span data-stu-id="9ea58-134">roles</span></span>|<span data-ttu-id="9ea58-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9ea58-135">string collection</span></span>|<span data-ttu-id="9ea58-136">Роль пользователя.</span><span class="sxs-lookup"><span data-stu-id="9ea58-136">The role for the user.</span></span> <span data-ttu-id="9ea58-137">Должно быть `owner` или пустым.</span><span class="sxs-lookup"><span data-stu-id="9ea58-137">Must be `owner` or empty.</span></span> <span data-ttu-id="9ea58-138">Пользователи с ролью "гость" автоматически отмечаются `guest` ролью, и это значение не может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="9ea58-138">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="9ea58-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ea58-139">Response</span></span>

<span data-ttu-id="9ea58-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [конверсатионмембер](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ea58-140">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ea58-141">Пример</span><span class="sxs-lookup"><span data-stu-id="9ea58-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ea58-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ea58-142">Request</span></span>

<span data-ttu-id="9ea58-143">Ниже приведен запрос на применение `owner` роли к существующему участнику команды.</span><span class="sxs-lookup"><span data-stu-id="9ea58-143">The following is a request to apply the `owner` role to an existing member of a team.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ea58-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ea58-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9ea58-145">C#</span><span class="sxs-lookup"><span data-stu-id="9ea58-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ea58-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ea58-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ea58-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ea58-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ea58-148">Java</span><span class="sxs-lookup"><span data-stu-id="9ea58-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ea58-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ea58-149">Response</span></span>

><span data-ttu-id="9ea58-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9ea58-150">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

## <a name="see-also"></a><span data-ttu-id="9ea58-151">См. также</span><span class="sxs-lookup"><span data-stu-id="9ea58-151">See also</span></span>

- [<span data-ttu-id="9ea58-152">Обновление элемента в канале</span><span class="sxs-lookup"><span data-stu-id="9ea58-152">Update member in channel</span></span>](channel-update-members.md)

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
