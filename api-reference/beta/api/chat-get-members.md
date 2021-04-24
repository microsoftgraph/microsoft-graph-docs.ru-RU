---
title: Получение объекта conversationMember в чате
description: Получение участника чата.
author: bhartono
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 067575ac3fa19ed1763c88923f97b20a0126a25e
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961340"
---
# <a name="get-conversationmember-in-a-chat"></a><span data-ttu-id="f0904-103">Получение объекта conversationMember в чате</span><span class="sxs-lookup"><span data-stu-id="f0904-103">Get conversationMember in a chat</span></span>

<span data-ttu-id="f0904-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0904-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0904-105">Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="f0904-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

> [!NOTE]
> <span data-ttu-id="f0904-106">Идентификаторы членства, возвращаемые сервером, должны рассматриваться как непрозрачные строки.</span><span class="sxs-lookup"><span data-stu-id="f0904-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="f0904-107">Клиент не должен пытаться анализировать или делать какие-либо предположения об этих идентификаторах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f0904-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="f0904-108">В дальнейшем результаты членства могут сопоставляться с пользователями различных клиентов, как указано в отклике.</span><span class="sxs-lookup"><span data-stu-id="f0904-108">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="f0904-109">Клиент не должен предполагать, что все участники относятся только к текущему клиенту.</span><span class="sxs-lookup"><span data-stu-id="f0904-109">The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0904-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0904-110">Permissions</span></span>

<span data-ttu-id="f0904-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0904-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0904-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0904-113">Permission Type</span></span>|<span data-ttu-id="f0904-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0904-114">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="f0904-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0904-115">Delegated (work or school account)</span></span>| <span data-ttu-id="f0904-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0904-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="f0904-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0904-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0904-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0904-118">Not supported.</span></span>|
|<span data-ttu-id="f0904-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="f0904-119">Application</span></span>| <span data-ttu-id="f0904-120">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="f0904-120">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All.</span></span> |

> <span data-ttu-id="f0904-121">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="f0904-121">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="f0904-122">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="f0904-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="f0904-123">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="f0904-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="f0904-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0904-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members/{membership-id}
GET /users/{user-id}/chats/{chat-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0904-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f0904-125">Optional query parameters</span></span>

<span data-ttu-id="f0904-126">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f0904-126">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0904-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0904-127">Request headers</span></span>

| <span data-ttu-id="f0904-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0904-128">Header</span></span>       | <span data-ttu-id="f0904-129">Значение</span><span class="sxs-lookup"><span data-stu-id="f0904-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f0904-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0904-130">Authorization</span></span>  | <span data-ttu-id="f0904-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0904-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f0904-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0904-133">Request body</span></span>

<span data-ttu-id="f0904-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0904-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0904-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0904-135">Response</span></span>

<span data-ttu-id="f0904-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0904-136">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0904-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f0904-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0904-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0904-138">Request</span></span>

<span data-ttu-id="f0904-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0904-139">Here is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzJjOGQyYjVjLTE4NDktNDA2Ni1iNTdkLWU3YTBlOWU0NGVjOA==
```

### <a name="response"></a><span data-ttu-id="f0904-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0904-140">Response</span></span>

<span data-ttu-id="f0904-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f0904-141">Here is an example of the response.</span></span>

<!-- 
{
  "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member",
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ab8577894a63548969c5c92bb9c80c5e1%40thread.v2')/members/$entity",
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzJjOGQyYjVjLTE4NDktNDA2Ni1iNTdkLWU3YTBlOWU0NGVjOA==",
    "roles": [
        "owner"
    ],
    "displayName": "John Doe",
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
    "userId": "2c8d2b5c-1849-4066-b57d-e7a0e9e44ec8",
    "email": "johndoe@contoso.onmicrosoft.com",
    "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member get",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


