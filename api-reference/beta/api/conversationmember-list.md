---
title: Список объектов conversationMember
description: Получение участника чата или канала.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f5454db8b04fee03c2c5ae27e0842df6aa0781fb
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288517"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="a9242-103">Список объектов conversationMember</span><span class="sxs-lookup"><span data-stu-id="a9242-103">List conversationMembers</span></span>

<span data-ttu-id="a9242-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9242-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9242-105">Перечисление всех [участников беседы](../resources/conversationmember.md) в [чате](../resources/chat.md) или [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="a9242-105">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9242-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9242-106">Permissions</span></span>

<span data-ttu-id="a9242-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9242-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9242-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9242-109">Permission Type</span></span>|<span data-ttu-id="a9242-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9242-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="a9242-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9242-111">Delegated (work or school account)</span></span>| <span data-ttu-id="a9242-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9242-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="a9242-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9242-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9242-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9242-114">Not supported.</span></span>|
|<span data-ttu-id="a9242-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="a9242-115">Application</span></span>| <span data-ttu-id="a9242-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9242-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="a9242-117">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="a9242-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="a9242-118">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="a9242-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="a9242-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9242-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9242-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a9242-120">Optional query parameters</span></span>

<span data-ttu-id="a9242-121">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a9242-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9242-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9242-122">Request headers</span></span>

| <span data-ttu-id="a9242-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9242-123">Header</span></span>       | <span data-ttu-id="a9242-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a9242-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a9242-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9242-125">Authorization</span></span>  | <span data-ttu-id="a9242-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9242-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a9242-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9242-128">Request body</span></span>

<span data-ttu-id="a9242-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9242-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9242-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9242-130">Response</span></span>

<span data-ttu-id="a9242-131">В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9242-131">If successful, this method returns a `200 OK` response code and a list of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9242-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a9242-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a9242-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9242-133">Request</span></span>

<span data-ttu-id="a9242-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9242-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9242-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9242-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="a9242-136">C#</span><span class="sxs-lookup"><span data-stu-id="a9242-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9242-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9242-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9242-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9242-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a9242-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9242-139">Response</span></span>

<span data-ttu-id="a9242-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a9242-140">Here is an example of the response.</span></span>

><span data-ttu-id="a9242-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9242-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "roles": [],
            "displayName": "John Doe",
            "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "email": null
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member list",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
