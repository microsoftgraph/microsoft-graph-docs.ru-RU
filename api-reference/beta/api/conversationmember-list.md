---
title: Список объектов conversationMember
description: Получение участника чата.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d6ef2a6f0bb101b32831c24eb861e47f129103d8
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536101"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="986fc-103">Список объектов conversationMember</span><span class="sxs-lookup"><span data-stu-id="986fc-103">List conversationMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="986fc-104">Перечисление всех [участников беседы](../resources/conversationmember.md) в [чате](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="986fc-104">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="986fc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="986fc-105">Permissions</span></span>

<span data-ttu-id="986fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="986fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="986fc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="986fc-108">Permission Type</span></span>|<span data-ttu-id="986fc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="986fc-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="986fc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="986fc-110">Delegated (work or school account)</span></span>|<span data-ttu-id="986fc-111">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="986fc-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="986fc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="986fc-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="986fc-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="986fc-113">Not supported</span></span>|
|<span data-ttu-id="986fc-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="986fc-114">Application</span></span>| <span data-ttu-id="986fc-115">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="986fc-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="986fc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="986fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="986fc-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="986fc-117">Optional query parameters</span></span>

<span data-ttu-id="986fc-118">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="986fc-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="986fc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="986fc-119">Request headers</span></span>

| <span data-ttu-id="986fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="986fc-120">Header</span></span>       | <span data-ttu-id="986fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="986fc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="986fc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="986fc-122">Authorization</span></span>  | <span data-ttu-id="986fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="986fc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="986fc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="986fc-125">Request body</span></span>

<span data-ttu-id="986fc-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="986fc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="986fc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="986fc-127">Response</span></span>

<span data-ttu-id="986fc-128">В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="986fc-128">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="986fc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="986fc-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="986fc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="986fc-130">Request</span></span>

<span data-ttu-id="986fc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="986fc-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/me/chats/{id}/members
```

##### <a name="response"></a><span data-ttu-id="986fc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="986fc-132">Response</span></span>

<span data-ttu-id="986fc-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="986fc-133">Here is an example of the response.</span></span>

><span data-ttu-id="986fc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="986fc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="986fc-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="986fc-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="986fc-137">C#</span><span class="sxs-lookup"><span data-stu-id="986fc-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversation_member-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="986fc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="986fc-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversation_member-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/conversationmember-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/conversationmember-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->