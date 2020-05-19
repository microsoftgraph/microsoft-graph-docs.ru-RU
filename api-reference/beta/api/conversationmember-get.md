---
title: Получение объекта conversationMember
description: Получение участника чата или канала.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cfb6649709cce80b7936ddab80f18bf6f3493924
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288531"
---
# <a name="get-conversationmember"></a><span data-ttu-id="bc2e9-103">Получение объекта conversationMember</span><span class="sxs-lookup"><span data-stu-id="bc2e9-103">Get conversationMember</span></span>

<span data-ttu-id="bc2e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc2e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc2e9-105">Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md) или [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="bc2e9-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bc2e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc2e9-106">Permissions</span></span>

<span data-ttu-id="bc2e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc2e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc2e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc2e9-109">Permission Type</span></span>|<span data-ttu-id="bc2e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc2e9-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="bc2e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc2e9-111">Delegated (work or school account)</span></span>| <span data-ttu-id="bc2e9-112">Для ресурсов " **пользователь** " или " **чат** ": Chat. ReadBasic, Chat. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc2e9-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="bc2e9-113">Для ресурса **Channel** : Чаннелмембер. Read. ALL, Чаннелмембер. ReadWrite, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bc2e9-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="bc2e9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc2e9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc2e9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc2e9-115">Not supported.</span></span>|
|<span data-ttu-id="bc2e9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc2e9-116">Application</span></span>| <span data-ttu-id="bc2e9-117">Для ресурсов " **пользователь** " или " **чат** ": Chat. ReadBasic. ALL, Chat. Read. ALL, Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bc2e9-117">For **user** or **chat** resource: Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="bc2e9-118">Для ресурса **Channel** : Member. Read. Group ([RSC](https://aka.ms/teams-rsc)), Чаннелмембер. Read. ALL, Чаннелмембер. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bc2e9-118">For **channel** resource: Member.Read.Group ([RSC](https://aka.ms/teams-rsc)), ChannelMember.Read.All, ChannelMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="bc2e9-119">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="bc2e9-119">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="bc2e9-120">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="bc2e9-120">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="bc2e9-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc2e9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc2e9-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bc2e9-122">Optional query parameters</span></span>

<span data-ttu-id="bc2e9-123">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bc2e9-123">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc2e9-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc2e9-124">Request headers</span></span>

| <span data-ttu-id="bc2e9-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc2e9-125">Header</span></span>       | <span data-ttu-id="bc2e9-126">Значение</span><span class="sxs-lookup"><span data-stu-id="bc2e9-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bc2e9-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc2e9-127">Authorization</span></span>  | <span data-ttu-id="bc2e9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc2e9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc2e9-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bc2e9-130">Request body</span></span>

<span data-ttu-id="bc2e9-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc2e9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc2e9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc2e9-132">Response</span></span>

<span data-ttu-id="bc2e9-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc2e9-133">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc2e9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="bc2e9-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc2e9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc2e9-135">Request</span></span>

<span data-ttu-id="bc2e9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc2e9-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc2e9-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc2e9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="bc2e9-138">C#</span><span class="sxs-lookup"><span data-stu-id="bc2e9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc2e9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc2e9-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc2e9-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc2e9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="bc2e9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc2e9-141">Response</span></span>

<span data-ttu-id="bc2e9-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc2e9-142">Here is an example of the response.</span></span>

><span data-ttu-id="bc2e9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc2e9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
