---
title: Получение объекта conversationMember
description: Получение участника чата или канала.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 05708a121b5cdedecc62c0b23678bf126cfd0662
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436505"
---
# <a name="get-conversationmember"></a><span data-ttu-id="c642b-103">Получение объекта conversationMember</span><span class="sxs-lookup"><span data-stu-id="c642b-103">Get conversationMember</span></span>

<span data-ttu-id="c642b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c642b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c642b-105">Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md) или [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="c642b-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c642b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c642b-106">Permissions</span></span>

<span data-ttu-id="c642b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c642b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c642b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c642b-109">Permission Type</span></span>|<span data-ttu-id="c642b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c642b-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c642b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c642b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c642b-112">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="c642b-112">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="c642b-113">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c642b-113">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="c642b-114">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="c642b-114">For **channel** resource:</span></span><br/><span data-ttu-id="c642b-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c642b-115">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="c642b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c642b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c642b-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c642b-117">Not supported</span></span>|
|<span data-ttu-id="c642b-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="c642b-118">Application</span></span>| <span data-ttu-id="c642b-119">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="c642b-119">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="c642b-120">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c642b-120">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="c642b-121">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="c642b-121">For **channel** resource:</span></span><br/><span data-ttu-id="c642b-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c642b-122">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="c642b-123">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="c642b-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="c642b-124">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="c642b-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="c642b-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c642b-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c642b-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c642b-126">Optional query parameters</span></span>

<span data-ttu-id="c642b-127">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c642b-127">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c642b-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c642b-128">Request headers</span></span>

| <span data-ttu-id="c642b-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c642b-129">Header</span></span>       | <span data-ttu-id="c642b-130">Значение</span><span class="sxs-lookup"><span data-stu-id="c642b-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c642b-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c642b-131">Authorization</span></span>  | <span data-ttu-id="c642b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c642b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c642b-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c642b-134">Request body</span></span>

<span data-ttu-id="c642b-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c642b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c642b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c642b-136">Response</span></span>

<span data-ttu-id="c642b-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c642b-137">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c642b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c642b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c642b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c642b-139">Request</span></span>

<span data-ttu-id="c642b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c642b-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c642b-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c642b-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="c642b-142">C#</span><span class="sxs-lookup"><span data-stu-id="c642b-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c642b-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c642b-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c642b-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c642b-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c642b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c642b-145">Response</span></span>

<span data-ttu-id="c642b-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c642b-146">Here is an example of the response.</span></span>

><span data-ttu-id="c642b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c642b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
