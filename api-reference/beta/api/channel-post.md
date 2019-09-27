---
title: Создание канала
description: Создание канала в Microsoft Team, как указано в тексте запроса.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d8a93e130e839fcd8bb6c332331d0b8dd390c147
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275687"
---
# <a name="create-channel"></a><span data-ttu-id="6b6cc-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="6b6cc-103">Create Channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b6cc-104">Создание [канала](../resources/channel.md) в Microsoft Team, как указано в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b6cc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b6cc-105">Permissions</span></span>

<span data-ttu-id="6b6cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b6cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b6cc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b6cc-108">Permission type</span></span>      | <span data-ttu-id="6b6cc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b6cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b6cc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b6cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6b6cc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b6cc-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b6cc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b6cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b6cc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-113">Not supported.</span></span>    |
|<span data-ttu-id="6b6cc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b6cc-114">Application</span></span> | <span data-ttu-id="6b6cc-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b6cc-115">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="6b6cc-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6b6cc-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6b6cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b6cc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="6b6cc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b6cc-119">Request headers</span></span>

| <span data-ttu-id="6b6cc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b6cc-120">Header</span></span>       | <span data-ttu-id="6b6cc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6b6cc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b6cc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b6cc-122">Authorization</span></span>  | <span data-ttu-id="6b6cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6b6cc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b6cc-125">Content-Type</span></span>  | <span data-ttu-id="6b6cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b6cc-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b6cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b6cc-127">Request body</span></span>

<span data-ttu-id="6b6cc-128">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-128">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6b6cc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b6cc-129">Response</span></span>

<span data-ttu-id="6b6cc-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-130">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b6cc-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b6cc-131">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="6b6cc-132">Пример 1: создание стандартного канала</span><span class="sxs-lookup"><span data-stu-id="6b6cc-132">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="6b6cc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b6cc-133">Request</span></span>

<span data-ttu-id="6b6cc-134">В приведенном ниже примере показан запрос на создание стандартного канала.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-134">The following example shows a request to create a standard channel.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6b6cc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b6cc-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b6cc-136">C#</span><span class="sxs-lookup"><span data-stu-id="6b6cc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b6cc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b6cc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b6cc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b6cc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6b6cc-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b6cc-139">Response</span></span>

<span data-ttu-id="6b6cc-140">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-140">The following example shows the response.</span></span>

> <span data-ttu-id="6b6cc-p104">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="6b6cc-143">Пример 2: создание закрытого канала от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="6b6cc-143">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="6b6cc-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b6cc-144">Request</span></span>

<span data-ttu-id="6b6cc-145">В приведенном ниже примере показан запрос на создание закрытого канала и Добавление пользователя в качестве владельца группы.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-145">The following example shows a request to create a private channel and add a user as an team owner.</span></span>

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

#### <a name="response"></a><span data-ttu-id="6b6cc-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b6cc-146">Response</span></span>

<span data-ttu-id="6b6cc-147">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b6cc-147">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 200 OK
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
