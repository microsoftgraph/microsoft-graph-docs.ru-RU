---
title: Создание канала
description: Создание канала в Microsoft Team, как указано в тексте запроса.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 709f0f5a64dce5f4f88ba7eacc4330856cc00ea8
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43805801"
---
# <a name="create-channel"></a><span data-ttu-id="666f3-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="666f3-103">Create Channel</span></span>

<span data-ttu-id="666f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="666f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="666f3-105">Создание [канала](../resources/channel.md) в Microsoft Team, как указано в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="666f3-105">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="666f3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="666f3-106">Permissions</span></span>

<span data-ttu-id="666f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="666f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="666f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="666f3-109">Permission type</span></span>      | <span data-ttu-id="666f3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="666f3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="666f3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="666f3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="666f3-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="666f3-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="666f3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="666f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="666f3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="666f3-114">Not supported.</span></span>    |
|<span data-ttu-id="666f3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="666f3-115">Application</span></span> | <span data-ttu-id="666f3-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="666f3-116">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="666f3-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="666f3-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="666f3-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="666f3-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="666f3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="666f3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="666f3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="666f3-120">Request headers</span></span>

| <span data-ttu-id="666f3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="666f3-121">Header</span></span>       | <span data-ttu-id="666f3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="666f3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="666f3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="666f3-123">Authorization</span></span>  | <span data-ttu-id="666f3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="666f3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="666f3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="666f3-126">Content-Type</span></span>  | <span data-ttu-id="666f3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="666f3-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="666f3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="666f3-128">Request body</span></span>

<span data-ttu-id="666f3-129">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="666f3-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="666f3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="666f3-130">Response</span></span>

<span data-ttu-id="666f3-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="666f3-131">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="666f3-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="666f3-132">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="666f3-133">Пример 1: создание стандартного канала</span><span class="sxs-lookup"><span data-stu-id="666f3-133">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="666f3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="666f3-134">Request</span></span>

<span data-ttu-id="666f3-135">В приведенном ниже примере показан запрос на создание стандартного канала.</span><span class="sxs-lookup"><span data-stu-id="666f3-135">The following example shows a request to create a standard channel.</span></span>

# <a name="http"></a>[<span data-ttu-id="666f3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="666f3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```
# <a name="c"></a>[<span data-ttu-id="666f3-137">C#</span><span class="sxs-lookup"><span data-stu-id="666f3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="666f3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="666f3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="666f3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="666f3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="666f3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="666f3-140">Response</span></span>

<span data-ttu-id="666f3-141">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="666f3-141">The following example shows the response.</span></span>

> <span data-ttu-id="666f3-p104">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="666f3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="666f3-144">Пример 2: создание закрытого канала от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="666f3-144">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="666f3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="666f3-145">Request</span></span>

<span data-ttu-id="666f3-146">В приведенном ниже примере показан запрос на создание закрытого канала и Добавление пользователя в качестве владельца группы.</span><span class="sxs-lookup"><span data-stu-id="666f3-146">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="666f3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="666f3-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{group_id}/channels
Content-type: application/json

{
  "@odata.type": "#Microsoft.Teams.Core.channel",
  "membershipType": "private",
  "displayName": "My First Private Channel",
  "description": "This is my first private channels",
  "members":
     [
        {
           "@odata.type":"#microsoft.graph.aadUserConversationMember",
           "user@odata.bind":"https://graph.microsoft.com/beta/users('{user_id}')",
           "roles":["owner"]
        }
     ]
}
```
# <a name="c"></a>[<span data-ttu-id="666f3-148">C#</span><span class="sxs-lookup"><span data-stu-id="666f3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="666f3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="666f3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="666f3-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="666f3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="666f3-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="666f3-151">Response</span></span>

<span data-ttu-id="666f3-152">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="666f3-152">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('{group_id}')/channels/$entity",
    "id": "{channel_id}",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/{channel_id}/My%20First%20Private%20Channel?groupId={group_id}&tenantId={tenant_id}",
    "membershipType": "private"
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
