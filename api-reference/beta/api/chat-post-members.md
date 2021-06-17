---
title: Добавление участника в чат
description: Добавьте conversationMember в чат.
author: bhartono
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3c9ca7557be5c0458354565fb3a54388b43defc1
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971090"
---
# <a name="add-member-to-a-chat"></a><span data-ttu-id="9b6e5-103">Добавление участника в чат</span><span class="sxs-lookup"><span data-stu-id="9b6e5-103">Add member to a chat</span></span>

<span data-ttu-id="9b6e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b6e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b6e5-105">Добавление [conversationMember](../resources/conversationmember.md) в [чат.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="9b6e5-105">Add a [conversationMember](../resources/conversationmember.md) to a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b6e5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b6e5-106">Permissions</span></span>

<span data-ttu-id="9b6e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b6e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b6e5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b6e5-109">Permission Type</span></span>|<span data-ttu-id="9b6e5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b6e5-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9b6e5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b6e5-111">Delegated (work or school account)</span></span>| <span data-ttu-id="9b6e5-112">ChatMember.ReadWrite, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b6e5-112">ChatMember.ReadWrite, Chat.ReadWrite</span></span> |
|<span data-ttu-id="9b6e5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b6e5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b6e5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b6e5-114">Not supported.</span></span>|
|<span data-ttu-id="9b6e5-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9b6e5-115">Application</span></span>| <span data-ttu-id="9b6e5-116">Chat.Manage.Chat\*, ChatMember.ReadWrite.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b6e5-116">Chat.Manage.Chat\*, ChatMember.ReadWrite.All, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="9b6e5-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="9b6e5-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

<!-- { "blockType": "ignored"} -->
```http
POST /chats/{chat-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="9b6e5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b6e5-118">Request headers</span></span>

| <span data-ttu-id="9b6e5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b6e5-119">Header</span></span>       | <span data-ttu-id="9b6e5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9b6e5-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9b6e5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b6e5-121">Authorization</span></span>  | <span data-ttu-id="9b6e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b6e5-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="9b6e5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b6e5-124">Content-Type</span></span>|<span data-ttu-id="9b6e5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b6e5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b6e5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b6e5-127">Request body</span></span>

<span data-ttu-id="9b6e5-128">В теле запроса укажите описание объекта [conversationMember](../resources/conversationmember.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b6e5-128">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9b6e5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b6e5-129">Response</span></span>

<span data-ttu-id="9b6e5-130">В случае успешной работы этот метод возвращает код отклика и заглавную ссылку Location, которая предоставляет URL-адрес вновь созданному `201 Created` объекту-члену.</span><span class="sxs-lookup"><span data-stu-id="9b6e5-130">If successful, this method returns a `201 Created` response code and a Location header that provides a URL path to the newly created member object.</span></span>

## <a name="examples"></a><span data-ttu-id="9b6e5-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="9b6e5-131">Examples</span></span>

### <a name="example-1-add-a-single-member-to-a-chat-and-specify-the-timespan-for-the-conversation-history"></a><span data-ttu-id="9b6e5-132">Пример 1. Добавление одного участника в чат и указание времени для истории беседы</span><span class="sxs-lookup"><span data-stu-id="9b6e5-132">Example 1: Add a single member to a chat and specify the timespan for the conversation history</span></span>

#### <a name="request"></a><span data-ttu-id="9b6e5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b6e5-133">Request</span></span>

<span data-ttu-id="9b6e5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b6e5-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9b6e5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b6e5-135">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="9b6e5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b6e5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-specific-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b6e5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b6e5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-specific-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b6e5-138">Java</span><span class="sxs-lookup"><span data-stu-id="9b6e5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-specific-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9b6e5-139">C#</span><span class="sxs-lookup"><span data-stu-id="9b6e5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-specific-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="9b6e5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b6e5-140">Response</span></span>

<span data-ttu-id="9b6e5-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b6e5-141">Here is an example of the response.</span></span>

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

### <a name="example-2-adding-a-single-member-to-a-microsoft-teams-chat-sharing-no-chat-history"></a><span data-ttu-id="9b6e5-142">Пример 2. Добавление одного члена в чат Microsoft Teams, не делясь историей чата</span><span class="sxs-lookup"><span data-stu-id="9b6e5-142">Example 2: Adding a single member to a Microsoft Teams chat, sharing no chat history</span></span>

#### <a name="request"></a><span data-ttu-id="9b6e5-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b6e5-143">Request</span></span>

<span data-ttu-id="9b6e5-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b6e5-144">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9b6e5-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b6e5-145">HTTP</span></span>](#tab/http)
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

# <a name="javascript"></a>[<span data-ttu-id="9b6e5-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b6e5-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-no-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b6e5-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b6e5-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-no-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b6e5-148">Java</span><span class="sxs-lookup"><span data-stu-id="9b6e5-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-no-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9b6e5-149">C#</span><span class="sxs-lookup"><span data-stu-id="9b6e5-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-no-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="9b6e5-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b6e5-150">Response</span></span>

<span data-ttu-id="9b6e5-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b6e5-151">Here is an example of the response.</span></span>

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

### <a name="example-3-adding-a-single-member-to-a-microsoft-teams-chat-sharing-the-whole-history-of-the-chat"></a><span data-ttu-id="9b6e5-152">Пример 3. Добавление одного члена в Microsoft Teams чат, общий доступ к всей истории чата</span><span class="sxs-lookup"><span data-stu-id="9b6e5-152">Example 3: Adding a single member to a Microsoft Teams chat, sharing the whole history of the chat</span></span>

#### <a name="request"></a><span data-ttu-id="9b6e5-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b6e5-153">Request</span></span>

<span data-ttu-id="9b6e5-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b6e5-154">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9b6e5-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b6e5-155">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="9b6e5-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b6e5-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-all-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b6e5-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b6e5-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-all-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b6e5-158">Java</span><span class="sxs-lookup"><span data-stu-id="9b6e5-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-all-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9b6e5-159">C#</span><span class="sxs-lookup"><span data-stu-id="9b6e5-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-all-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="9b6e5-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b6e5-160">Response</span></span>

<span data-ttu-id="9b6e5-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b6e5-161">Here is an example of the response.</span></span>

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


