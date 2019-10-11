---
title: Получение объекта conversationMember
description: Получение участника чата или канала.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bd1d7cc150ade0a9c50083d9b9833ae682599b95
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439815"
---
# <a name="get-conversationmember"></a><span data-ttu-id="cee0a-103">Получение объекта conversationMember</span><span class="sxs-lookup"><span data-stu-id="cee0a-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cee0a-104">Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md) или [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="cee0a-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cee0a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cee0a-105">Permissions</span></span>

<span data-ttu-id="cee0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cee0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cee0a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cee0a-108">Permission Type</span></span>|<span data-ttu-id="cee0a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cee0a-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="cee0a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cee0a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="cee0a-111">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="cee0a-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="cee0a-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cee0a-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="cee0a-113">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="cee0a-113">For **channel** resource:</span></span><br/><span data-ttu-id="cee0a-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cee0a-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="cee0a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cee0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cee0a-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cee0a-116">Not supported</span></span>|
|<span data-ttu-id="cee0a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cee0a-117">Application</span></span>| <span data-ttu-id="cee0a-118">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="cee0a-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="cee0a-119">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cee0a-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="cee0a-120">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="cee0a-120">For **channel** resource:</span></span><br/><span data-ttu-id="cee0a-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cee0a-121">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="cee0a-122">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="cee0a-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="cee0a-123">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="cee0a-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="cee0a-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cee0a-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cee0a-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cee0a-125">Optional query parameters</span></span>

<span data-ttu-id="cee0a-126">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cee0a-126">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cee0a-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cee0a-127">Request headers</span></span>

| <span data-ttu-id="cee0a-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cee0a-128">Header</span></span>       | <span data-ttu-id="cee0a-129">Значение</span><span class="sxs-lookup"><span data-stu-id="cee0a-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cee0a-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cee0a-130">Authorization</span></span>  | <span data-ttu-id="cee0a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cee0a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cee0a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cee0a-133">Request body</span></span>

<span data-ttu-id="cee0a-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cee0a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cee0a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cee0a-135">Response</span></span>

<span data-ttu-id="cee0a-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cee0a-136">If successful, this method returns a `200 OK` response code and a [channel](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cee0a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="cee0a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="cee0a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="cee0a-138">Request</span></span>

<span data-ttu-id="cee0a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cee0a-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cee0a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="cee0a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cee0a-141">C#</span><span class="sxs-lookup"><span data-stu-id="cee0a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cee0a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cee0a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cee0a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cee0a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="cee0a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="cee0a-144">Response</span></span>

<span data-ttu-id="cee0a-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cee0a-145">Here is an example of the response.</span></span>

><span data-ttu-id="cee0a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cee0a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
