---
title: Добавление участника в чат
description: Добавьте conversationMember в чат.
author: bhartono
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2bf40e04e4d25b3fb4c8f97ebd61e18893f1b17d
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787480"
---
# <a name="add-member-to-a-chat"></a><span data-ttu-id="03632-103">Добавление участника в чат</span><span class="sxs-lookup"><span data-stu-id="03632-103">Add member to a chat</span></span>

<span data-ttu-id="03632-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03632-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03632-105">Добавление [conversationMember](../resources/conversationmember.md) в [чат.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="03632-105">Add a [conversationMember](../resources/conversationmember.md) to a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="03632-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03632-106">Permissions</span></span>

<span data-ttu-id="03632-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03632-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03632-109">Permission Type</span></span>|<span data-ttu-id="03632-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03632-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="03632-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03632-111">Delegated (work or school account)</span></span>| <span data-ttu-id="03632-112">ChatMember.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03632-112">ChatMember.ReadWrite</span></span> |
|<span data-ttu-id="03632-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03632-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03632-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03632-114">Not supported.</span></span>|
|<span data-ttu-id="03632-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03632-115">Application</span></span>| <span data-ttu-id="03632-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03632-116">Not supported.</span></span> |

<!-- { "blockType": "ignored"} -->
```http
POST /chats/{chat-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="03632-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03632-117">Request headers</span></span>

| <span data-ttu-id="03632-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03632-118">Header</span></span>       | <span data-ttu-id="03632-119">Значение</span><span class="sxs-lookup"><span data-stu-id="03632-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="03632-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03632-120">Authorization</span></span>  | <span data-ttu-id="03632-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03632-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="03632-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03632-123">Content-Type</span></span>|<span data-ttu-id="03632-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03632-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03632-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03632-126">Request body</span></span>

<span data-ttu-id="03632-127">В теле запроса укажите описание объекта [conversationMember](../resources/conversationmember.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03632-127">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="03632-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="03632-128">Response</span></span>

<span data-ttu-id="03632-129">В случае успешной работы этот метод возвращает код отклика и заглавную ссылку Location, которая предоставляет URL-адрес вновь созданному `201 Created` объекту-члену.</span><span class="sxs-lookup"><span data-stu-id="03632-129">If successful, this method returns a `201 Created` response code and a Location header that provides a URL path to the newly created member object.</span></span>

## <a name="examples"></a><span data-ttu-id="03632-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="03632-130">Examples</span></span>

### <a name="example-1-add-a-single-member-to-a-chat-and-specify-the-timespan-for-the-conversation-history"></a><span data-ttu-id="03632-131">Пример 1. Добавление одного участника в чат и указание времени для истории беседы</span><span class="sxs-lookup"><span data-stu-id="03632-131">Example 1: Add a single member to a chat and specify the timespan for the conversation history</span></span>

#### <a name="request"></a><span data-ttu-id="03632-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="03632-132">Request</span></span>

<span data-ttu-id="03632-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03632-133">Here is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="03632-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="03632-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
}
```
# <a name="c"></a>[<span data-ttu-id="03632-135">C#</span><span class="sxs-lookup"><span data-stu-id="03632-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-specific-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03632-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03632-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-specific-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03632-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03632-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-specific-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03632-138">Java</span><span class="sxs-lookup"><span data-stu-id="03632-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-specific-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="03632-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="03632-139">Response</span></span>

<span data-ttu-id="03632-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03632-140">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-2-adding-a-single-member-to-a-microsoft-teams-chat-sharing-no-chat-history"></a><span data-ttu-id="03632-141">Пример 2. Добавление одного члена в чат Microsoft Teams, не делясь историей чата</span><span class="sxs-lookup"><span data-stu-id="03632-141">Example 2: Adding a single member to a Microsoft Teams chat, sharing no chat history</span></span>

#### <a name="request"></a><span data-ttu-id="03632-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="03632-142">Request</span></span>

<span data-ttu-id="03632-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03632-143">Here is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="03632-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="03632-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="c"></a>[<span data-ttu-id="03632-145">C#</span><span class="sxs-lookup"><span data-stu-id="03632-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-no-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03632-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03632-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-no-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03632-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03632-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-no-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03632-148">Java</span><span class="sxs-lookup"><span data-stu-id="03632-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-no-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="03632-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="03632-149">Response</span></span>

<span data-ttu-id="03632-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03632-150">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-3-adding-a-single-member-to-a-microsoft-teams-chat-sharing-the-whole-history-of-the-chat"></a><span data-ttu-id="03632-151">Пример 3. Добавление одного члена в Microsoft Teams чат, общий доступ к всей истории чата</span><span class="sxs-lookup"><span data-stu-id="03632-151">Example 3: Adding a single member to a Microsoft Teams chat, sharing the whole history of the chat</span></span>

#### <a name="request"></a><span data-ttu-id="03632-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="03632-152">Request</span></span>

<span data-ttu-id="03632-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03632-153">Here is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="03632-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="03632-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z"
}
```
# <a name="c"></a>[<span data-ttu-id="03632-155">C#</span><span class="sxs-lookup"><span data-stu-id="03632-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-all-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03632-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03632-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-all-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03632-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03632-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-all-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03632-158">Java</span><span class="sxs-lookup"><span data-stu-id="03632-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-all-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="03632-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="03632-159">Response</span></span>

<span data-ttu-id="03632-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03632-160">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```


