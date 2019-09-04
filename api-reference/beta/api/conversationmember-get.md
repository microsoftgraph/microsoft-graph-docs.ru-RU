---
title: Получение объекта conversationMember
description: Получение участника чата или канала.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c2c4a0ef03b6c190c53374516704007cc6757e1c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718354"
---
# <a name="get-conversationmember"></a><span data-ttu-id="8988c-103">Получение объекта conversationMember</span><span class="sxs-lookup"><span data-stu-id="8988c-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8988c-104">Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md) или [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="8988c-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8988c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8988c-105">Permissions</span></span>

<span data-ttu-id="8988c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8988c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8988c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8988c-108">Permission Type</span></span>|<span data-ttu-id="8988c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8988c-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="8988c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8988c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="8988c-111">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="8988c-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="8988c-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8988c-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="8988c-113">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="8988c-113">For **channel** resource:</span></span><br/><span data-ttu-id="8988c-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8988c-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="8988c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8988c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8988c-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8988c-116">Not supported</span></span>|
|<span data-ttu-id="8988c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8988c-117">Application</span></span>| <span data-ttu-id="8988c-118">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="8988c-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="8988c-119">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8988c-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="8988c-120">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="8988c-120">For **channel** resource:</span></span><br/><span data-ttu-id="8988c-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8988c-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8988c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8988c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8988c-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8988c-123">Optional query parameters</span></span>

<span data-ttu-id="8988c-124">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8988c-124">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8988c-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8988c-125">Request headers</span></span>

| <span data-ttu-id="8988c-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8988c-126">Header</span></span>       | <span data-ttu-id="8988c-127">Значение</span><span class="sxs-lookup"><span data-stu-id="8988c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8988c-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8988c-128">Authorization</span></span>  | <span data-ttu-id="8988c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8988c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8988c-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8988c-131">Request body</span></span>

<span data-ttu-id="8988c-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8988c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8988c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8988c-133">Response</span></span>

<span data-ttu-id="8988c-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8988c-134">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8988c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="8988c-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="8988c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="8988c-136">Request</span></span>

<span data-ttu-id="8988c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8988c-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8988c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8988c-138">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8988c-139">C#</span><span class="sxs-lookup"><span data-stu-id="8988c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8988c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8988c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8988c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8988c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8988c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8988c-142">Response</span></span>

<span data-ttu-id="8988c-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8988c-143">Here is an example of the response.</span></span>

><span data-ttu-id="8988c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8988c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "displayName": "display-name-value"
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
