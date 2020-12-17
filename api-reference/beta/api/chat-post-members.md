---
title: Добавление участника в чат
description: Добавление conversationMember в чат.
author: bhartono
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: db4ea9a11f332f77a31ff3821610b794baeaad33
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706350"
---
# <a name="add-member-to-a-chat"></a><span data-ttu-id="9dfdc-103">Добавление участника в чат</span><span class="sxs-lookup"><span data-stu-id="9dfdc-103">Add member to a chat</span></span>

<span data-ttu-id="9dfdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dfdc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dfdc-105">Добавление [conversationMember](../resources/conversationmember.md) в [чат.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="9dfdc-105">Add a [conversationMember](../resources/conversationmember.md) to a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9dfdc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9dfdc-106">Permissions</span></span>

<span data-ttu-id="9dfdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dfdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dfdc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dfdc-109">Permission Type</span></span>|<span data-ttu-id="9dfdc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dfdc-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9dfdc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dfdc-111">Delegated (work or school account)</span></span>| <span data-ttu-id="9dfdc-112">ChatMember.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dfdc-112">ChatMember.ReadWrite</span></span> |
|<span data-ttu-id="9dfdc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dfdc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dfdc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-114">Not supported.</span></span>|
|<span data-ttu-id="9dfdc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dfdc-115">Application</span></span>| <span data-ttu-id="9dfdc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-116">Not supported.</span></span> |

<!-- { "blockType": "ignored"} -->
```http
POST /chats/{chat-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="9dfdc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dfdc-117">Request headers</span></span>

| <span data-ttu-id="9dfdc-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9dfdc-118">Header</span></span>       | <span data-ttu-id="9dfdc-119">Значение</span><span class="sxs-lookup"><span data-stu-id="9dfdc-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9dfdc-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dfdc-120">Authorization</span></span>  | <span data-ttu-id="9dfdc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="9dfdc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9dfdc-123">Content-Type</span></span>|<span data-ttu-id="9dfdc-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9dfdc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9dfdc-126">Request body</span></span>

<span data-ttu-id="9dfdc-127">В теле запроса укажите описание объекта [conversationMember](../resources/conversationmember.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-127">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9dfdc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dfdc-128">Response</span></span>

<span data-ttu-id="9dfdc-129">В случае успеха этот метод возвращает код отклика и заглавную ссылку Location, которая предоставляет URL-путь к `201 Created` созданному объекту-члену.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-129">If successful, this method returns a `201 Created` response code and a Location header that provides a url path to the newly created member object.</span></span>

## <a name="examples"></a><span data-ttu-id="9dfdc-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="9dfdc-130">Examples</span></span>

### <a name="example-1-add-a-single-member-to-a-chat-and-specify-the-timespan-for-the-conversation-history"></a><span data-ttu-id="9dfdc-131">Пример 1. Добавление одного участника в чат и указание времени для истории беседы</span><span class="sxs-lookup"><span data-stu-id="9dfdc-131">Example 1: Add a single member to a chat and specify the timespan for the conversation history</span></span>

#### <a name="request"></a><span data-ttu-id="9dfdc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dfdc-132">Request</span></span>

<span data-ttu-id="9dfdc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-133">Here is an example of the request.</span></span>

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

---


#### <a name="response"></a><span data-ttu-id="9dfdc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dfdc-134">Response</span></span>

<span data-ttu-id="9dfdc-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-135">Here is an example of the response.</span></span>

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

### <a name="example-2-adding-a-single-member-to-a-microsoft-teams-chat-sharing-no-chat-history"></a><span data-ttu-id="9dfdc-136">Пример 2. Добавление одного участника в чат Microsoft Teams без общего доступа к истории чата</span><span class="sxs-lookup"><span data-stu-id="9dfdc-136">Example 2: Adding a single member to a Microsoft Teams chat, sharing no chat history</span></span>

#### <a name="request"></a><span data-ttu-id="9dfdc-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dfdc-137">Request</span></span>

<span data-ttu-id="9dfdc-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-138">Here is an example of the request.</span></span>

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

---


#### <a name="response"></a><span data-ttu-id="9dfdc-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dfdc-139">Response</span></span>

<span data-ttu-id="9dfdc-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-140">Here is an example of the response.</span></span>

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

### <a name="example-3-adding-a-single-member-to-a-microsoft-teams-chat-sharing-the-whole-history-of-the-chat"></a><span data-ttu-id="9dfdc-141">Пример 3. Добавление одного участника в чат Microsoft Teams, общий доступ к всей истории чата</span><span class="sxs-lookup"><span data-stu-id="9dfdc-141">Example 3: Adding a single member to a Microsoft Teams chat, sharing the whole history of the chat</span></span>

#### <a name="request"></a><span data-ttu-id="9dfdc-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dfdc-142">Request</span></span>

<span data-ttu-id="9dfdc-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-143">Here is an example of the request.</span></span>

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

---


#### <a name="response"></a><span data-ttu-id="9dfdc-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dfdc-144">Response</span></span>

<span data-ttu-id="9dfdc-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9dfdc-145">Here is an example of the response.</span></span>

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


