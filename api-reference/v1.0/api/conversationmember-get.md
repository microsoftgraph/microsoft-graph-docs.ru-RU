---
title: Получение объекта conversationMember
description: Получение участника чата или канала.
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8467e8ba0b32179da555f04cf94421bf0ea44a5d
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060609"
---
# <a name="get-conversationmember"></a><span data-ttu-id="c0490-103">Получение объекта conversationMember</span><span class="sxs-lookup"><span data-stu-id="c0490-103">Get conversationMember</span></span>

<span data-ttu-id="c0490-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0490-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0490-105">Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chatmessage.md) или [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="c0490-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chatmessage.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0490-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0490-106">Permissions</span></span>

<span data-ttu-id="c0490-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0490-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0490-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0490-109">Permission Type</span></span>|<span data-ttu-id="c0490-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0490-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c0490-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0490-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c0490-112">Для ресурса **user** или **chat**: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0490-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="c0490-113">Для ресурса **channel**: ChannelMember.Read.All, ChannelMember.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0490-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite</span></span> |
|<span data-ttu-id="c0490-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0490-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0490-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0490-115">Not supported.</span></span>|
|<span data-ttu-id="c0490-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c0490-116">Application</span></span>| <span data-ttu-id="c0490-117">Для ресурса **user** или **chat**: не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0490-117">For **user** or **chat** resource: Not supported.</span></span><br/><br/><span data-ttu-id="c0490-118">Для ресурса **channel**: TeamMember.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0490-118">For **channel** resource: TeamMember.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |

> <span data-ttu-id="c0490-119">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="c0490-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>


## <a name="http-request"></a><span data-ttu-id="c0490-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0490-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0490-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0490-121">Optional query parameters</span></span>

<span data-ttu-id="c0490-122">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c0490-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0490-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0490-123">Request headers</span></span>

| <span data-ttu-id="c0490-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0490-124">Header</span></span>       | <span data-ttu-id="c0490-125">Значение</span><span class="sxs-lookup"><span data-stu-id="c0490-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0490-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0490-126">Authorization</span></span>  | <span data-ttu-id="c0490-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0490-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0490-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0490-129">Request body</span></span>

<span data-ttu-id="c0490-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0490-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0490-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0490-131">Response</span></span>

<span data-ttu-id="c0490-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0490-132">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0490-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c0490-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0490-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0490-134">Request</span></span>

<span data-ttu-id="c0490-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0490-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c0490-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0490-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/V1.0/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="c0490-137">C#</span><span class="sxs-lookup"><span data-stu-id="c0490-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0490-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0490-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0490-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0490-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0490-140">Java</span><span class="sxs-lookup"><span data-stu-id="c0490-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0490-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0490-141">Response</span></span>

<span data-ttu-id="c0490-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c0490-142">Here is an example of the response.</span></span>

><span data-ttu-id="c0490-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c0490-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!--
{
  "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member_2",
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
