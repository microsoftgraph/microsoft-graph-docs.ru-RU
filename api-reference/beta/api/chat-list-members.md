---
title: Список участников чата
description: Получение списка участников чата.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 87ac400e712101ca598c357698e2da5c1578fa62
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706367"
---
# <a name="list-members-of-a-chat"></a><span data-ttu-id="175b8-103">Список участников чата</span><span class="sxs-lookup"><span data-stu-id="175b8-103">List members of a chat</span></span>

<span data-ttu-id="175b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="175b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="175b8-105">Перечисление всех [участников беседы](../resources/conversationmember.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="175b8-105">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md).</span></span>

> [!NOTE]
> <span data-ttu-id="175b8-106">Идентификаторы членства, возвращаемые сервером, должны рассматриваться как непрозрачные строки.</span><span class="sxs-lookup"><span data-stu-id="175b8-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="175b8-107">Клиент не должен пытаться анализировать или делать какие-либо предположения об этих идентификаторах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="175b8-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="175b8-108">В дальнейшем результаты членства могут сопоставляться с пользователями различных клиентов, как указано в отклике.</span><span class="sxs-lookup"><span data-stu-id="175b8-108">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="175b8-109">Клиент не должен предполагать, что все участники относятся только к текущему клиенту.</span><span class="sxs-lookup"><span data-stu-id="175b8-109">The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="175b8-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="175b8-110">Permissions</span></span>

<span data-ttu-id="175b8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="175b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="175b8-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="175b8-113">Permission Type</span></span>|<span data-ttu-id="175b8-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="175b8-114">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="175b8-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="175b8-115">Delegated (work or school account)</span></span>| <span data-ttu-id="175b8-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="175b8-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="175b8-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="175b8-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="175b8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="175b8-118">Not supported.</span></span>|
|<span data-ttu-id="175b8-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="175b8-119">Application</span></span>| <span data-ttu-id="175b8-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="175b8-120">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="175b8-121">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="175b8-121">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="175b8-122">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="175b8-122">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="175b8-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="175b8-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members
GET /users/{user-id}/chats/{chat-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="175b8-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="175b8-124">Optional query parameters</span></span>

<span data-ttu-id="175b8-125">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="175b8-125">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="175b8-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="175b8-126">Request headers</span></span>

| <span data-ttu-id="175b8-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="175b8-127">Header</span></span>       | <span data-ttu-id="175b8-128">Значение</span><span class="sxs-lookup"><span data-stu-id="175b8-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="175b8-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="175b8-129">Authorization</span></span>  | <span data-ttu-id="175b8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="175b8-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="175b8-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="175b8-132">Request body</span></span>

<span data-ttu-id="175b8-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="175b8-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="175b8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="175b8-134">Response</span></span>

<span data-ttu-id="175b8-135">В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="175b8-135">If successful, this method returns a `200 OK` response code and a list of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="175b8-136">С этой функцией связаны некоторые известные проблемы.</span><span class="sxs-lookup"><span data-stu-id="175b8-136">There are some known issues with this functionality.</span></span> <span data-ttu-id="175b8-137">Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues.md#missing-tenantid-for-chat-members).</span><span class="sxs-lookup"><span data-stu-id="175b8-137">For details, see [known issues](/graph/known-issues.md#missing-tenantid-for-chat-members).</span></span>

## <a name="example"></a><span data-ttu-id="175b8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="175b8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="175b8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="175b8-139">Request</span></span>

<span data-ttu-id="175b8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="175b8-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="175b8-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="175b8-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d@unq.gbl.spaces/members
```

---


### <a name="response"></a><span data-ttu-id="175b8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="175b8-142">Response</span></span>

<span data-ttu-id="175b8-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="175b8-143">Here is an example of the response.</span></span>

><span data-ttu-id="175b8-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="175b8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.count": 3,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "roles": [],
            "displayName": "John Doe",
            "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "email": null,
            "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
            "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "2de87aaf-844d-4def-9dee-2c317f0be1b3",
            "roles": [],
            "displayName": "Bart Hogan",
            "userId": "2de87aaf-844d-4def-9dee-2c317f0be1b3",
            "email": null,
            "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
            "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z"
    },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
            "roles": [],
            "displayName": "Minna Pham",
            "userId": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
            "email": null,
            "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
            "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
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


