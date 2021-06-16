---
title: Список объектов conversationMember
description: Получение списка участников чата или канала.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 678dca77b21375d4c28dd1f7768f9fec67da849b
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941461"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="f14be-103">Список объектов conversationMember</span><span class="sxs-lookup"><span data-stu-id="f14be-103">List conversationMembers</span></span>

<span data-ttu-id="f14be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f14be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f14be-105">Перечисление всех [участников беседы](../resources/conversationmember.md) в [чате](../resources/chatmessage.md) или [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="f14be-105">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chatmessage.md) or [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="f14be-106">Идентификаторы участия, возвращаемые сервером, должны рассматриваться как непрозрачные строки.</span><span class="sxs-lookup"><span data-stu-id="f14be-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="f14be-107">Клиент не должен пытаться анализировать или делать какие-либо предположения об этих идентификаторах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f14be-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="f14be-108">В дальнейшем результаты участия могут сопоставляться с пользователями из разных клиентов, как указано в отклике. Клиент не должен предполагать, что все участники относятся только к текущему клиенту.</span><span class="sxs-lookup"><span data-stu-id="f14be-108">The membership results could map to users from different tenants, as indicated in the response, in the future.The client should not assume that all members are from the current tenant only.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="f14be-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f14be-109">Permissions</span></span>

<span data-ttu-id="f14be-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f14be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f14be-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f14be-112">Permission Type</span></span>|<span data-ttu-id="f14be-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f14be-113">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="f14be-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f14be-114">Delegated (work or school account)</span></span>| <span data-ttu-id="f14be-115">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f14be-115">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="f14be-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f14be-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f14be-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f14be-117">Not supported.</span></span>|
|<span data-ttu-id="f14be-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f14be-118">Application</span></span>| <span data-ttu-id="f14be-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f14be-119">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="f14be-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f14be-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f14be-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f14be-121">Optional query parameters</span></span>

<span data-ttu-id="f14be-122">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f14be-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f14be-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f14be-123">Request headers</span></span>

| <span data-ttu-id="f14be-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f14be-124">Header</span></span>       | <span data-ttu-id="f14be-125">Значение</span><span class="sxs-lookup"><span data-stu-id="f14be-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f14be-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f14be-126">Authorization</span></span>  | <span data-ttu-id="f14be-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f14be-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f14be-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f14be-129">Request body</span></span>

<span data-ttu-id="f14be-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f14be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f14be-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f14be-131">Response</span></span>

<span data-ttu-id="f14be-132">В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f14be-132">If successful, this method returns a `200 OK` response code and a list of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f14be-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f14be-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f14be-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f14be-134">Request</span></span>

<span data-ttu-id="f14be-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f14be-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f14be-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f14be-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="f14be-137">C#</span><span class="sxs-lookup"><span data-stu-id="f14be-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f14be-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f14be-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f14be-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f14be-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f14be-140">Java</span><span class="sxs-lookup"><span data-stu-id="f14be-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-conversation-members-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f14be-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f14be-141">Response</span></span>

<span data-ttu-id="f14be-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f14be-142">The following is an example of the response.</span></span>

><span data-ttu-id="f14be-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f14be-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
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
