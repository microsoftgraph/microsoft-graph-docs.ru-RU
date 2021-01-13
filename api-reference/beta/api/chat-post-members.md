---
title: Добавление участника в чат
description: Добавление conversationMember в чат.
author: bhartono
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f3fe6c34d81e34f614f914780886902a8bf563c2
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843804"
---
# <a name="add-member-to-a-chat"></a><span data-ttu-id="c70b3-103">Добавление участника в чат</span><span class="sxs-lookup"><span data-stu-id="c70b3-103">Add member to a chat</span></span>

<span data-ttu-id="c70b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c70b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c70b3-105">Добавление [conversationMember](../resources/conversationmember.md) в [чат.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="c70b3-105">Add a [conversationMember](../resources/conversationmember.md) to a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c70b3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c70b3-106">Permissions</span></span>

<span data-ttu-id="c70b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c70b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c70b3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c70b3-109">Permission Type</span></span>|<span data-ttu-id="c70b3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c70b3-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c70b3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c70b3-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c70b3-112">ChatMember.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c70b3-112">ChatMember.ReadWrite</span></span> |
|<span data-ttu-id="c70b3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c70b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c70b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c70b3-114">Not supported.</span></span>|
|<span data-ttu-id="c70b3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c70b3-115">Application</span></span>| <span data-ttu-id="c70b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c70b3-116">Not supported.</span></span> |

<!-- { "blockType": "ignored"} -->
```http
POST /chats/{chat-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="c70b3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c70b3-117">Request headers</span></span>

| <span data-ttu-id="c70b3-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c70b3-118">Header</span></span>       | <span data-ttu-id="c70b3-119">Значение</span><span class="sxs-lookup"><span data-stu-id="c70b3-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c70b3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c70b3-120">Authorization</span></span>  | <span data-ttu-id="c70b3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c70b3-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="c70b3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c70b3-123">Content-Type</span></span>|<span data-ttu-id="c70b3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c70b3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c70b3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c70b3-126">Request body</span></span>

<span data-ttu-id="c70b3-127">В теле запроса укажите описание объекта [conversationMember](../resources/conversationmember.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c70b3-127">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c70b3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c70b3-128">Response</span></span>

<span data-ttu-id="c70b3-129">В случае успеха этот метод возвращает код отклика и заглавную ссылку Location, которая предоставляет URL-путь к `201 Created` созданному объекту-члену.</span><span class="sxs-lookup"><span data-stu-id="c70b3-129">If successful, this method returns a `201 Created` response code and a Location header that provides a URL path to the newly created member object.</span></span>

## <a name="examples"></a><span data-ttu-id="c70b3-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="c70b3-130">Examples</span></span>

### <a name="example-1-add-a-single-member-to-a-chat-and-specify-the-timespan-for-the-conversation-history"></a><span data-ttu-id="c70b3-131">Пример 1. Добавление одного участника в чат и указание времени для истории бесед</span><span class="sxs-lookup"><span data-stu-id="c70b3-131">Example 1: Add a single member to a chat and specify the timespan for the conversation history</span></span>

#### <a name="request"></a><span data-ttu-id="c70b3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c70b3-132">Request</span></span>

<span data-ttu-id="c70b3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c70b3-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c70b3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c70b3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
}
```
# <a name="javascript"></a>[<span data-ttu-id="c70b3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c70b3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-specific-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c70b3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c70b3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-specific-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c70b3-137">Java</span><span class="sxs-lookup"><span data-stu-id="c70b3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-specific-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c70b3-138">C#</span><span class="sxs-lookup"><span data-stu-id="c70b3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-specific-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="c70b3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c70b3-139">Response</span></span>

<span data-ttu-id="c70b3-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c70b3-140">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime",
  "@odata.type": "Microsoft.Teams.GraphSvc.conversationMember"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-2-adding-a-single-member-to-a-microsoft-teams-chat-sharing-no-chat-history"></a><span data-ttu-id="c70b3-141">Пример 2. Добавление одного участника в чат Microsoft Teams без общего доступа к истории чата</span><span class="sxs-lookup"><span data-stu-id="c70b3-141">Example 2: Adding a single member to a Microsoft Teams chat, sharing no chat history</span></span>

#### <a name="request"></a><span data-ttu-id="c70b3-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c70b3-142">Request</span></span>

<span data-ttu-id="c70b3-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c70b3-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c70b3-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c70b3-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```

# <a name="javascript"></a>[<span data-ttu-id="c70b3-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c70b3-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-no-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c70b3-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c70b3-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-no-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c70b3-147">Java</span><span class="sxs-lookup"><span data-stu-id="c70b3-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-no-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c70b3-148">C#</span><span class="sxs-lookup"><span data-stu-id="c70b3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-no-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="c70b3-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c70b3-149">Response</span></span>

<span data-ttu-id="c70b3-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c70b3-150">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime",
  "@odata.type": "Microsoft.Teams.GraphSvc.conversationMember"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-3-adding-a-single-member-to-a-microsoft-teams-chat-sharing-the-whole-history-of-the-chat"></a><span data-ttu-id="c70b3-151">Пример 3. Добавление одного участника в чат Microsoft Teams, общий доступ к всей истории чата</span><span class="sxs-lookup"><span data-stu-id="c70b3-151">Example 3: Adding a single member to a Microsoft Teams chat, sharing the whole history of the chat</span></span>

#### <a name="request"></a><span data-ttu-id="c70b3-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="c70b3-152">Request</span></span>

<span data-ttu-id="c70b3-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c70b3-153">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c70b3-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="c70b3-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z"
}
```
# <a name="javascript"></a>[<span data-ttu-id="c70b3-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c70b3-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-all-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c70b3-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c70b3-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-all-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c70b3-157">Java</span><span class="sxs-lookup"><span data-stu-id="c70b3-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-all-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c70b3-158">C#</span><span class="sxs-lookup"><span data-stu-id="c70b3-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-all-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="c70b3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="c70b3-159">Response</span></span>

<span data-ttu-id="c70b3-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c70b3-160">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime",
  "@odata.type": "Microsoft.Teams.GraphSvc.conversationMember"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```


