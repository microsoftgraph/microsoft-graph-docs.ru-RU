---
title: Получение объекта conversationMember
description: Получение участника чата или канала.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: efe599d9a1b4f7a928f9b0ae7dabfc845683af30
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491285"
---
# <a name="get-conversationmember"></a><span data-ttu-id="fa8df-103">Получение объекта conversationMember</span><span class="sxs-lookup"><span data-stu-id="fa8df-103">Get conversationMember</span></span>

<span data-ttu-id="fa8df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa8df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa8df-105">Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md) или [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="fa8df-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa8df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa8df-106">Permissions</span></span>

<span data-ttu-id="fa8df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa8df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa8df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa8df-109">Permission Type</span></span>|<span data-ttu-id="fa8df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa8df-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="fa8df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa8df-111">Delegated (work or school account)</span></span>| <span data-ttu-id="fa8df-112">Для ресурсов " **пользователь** " или " **чат** ": Chat. ReadBasic, Chat. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa8df-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="fa8df-113">Для ресурса **Channel** : Чаннелмембер. Read. ALL, Чаннелмембер. ReadWrite, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa8df-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="fa8df-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa8df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa8df-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa8df-115">Not supported.</span></span>|
|<span data-ttu-id="fa8df-116">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="fa8df-116">Application</span></span>| <span data-ttu-id="fa8df-117">Для ресурсов " **пользователь** " или " **чат** ": Chat. ReadBasic. ALL, Chat. Read. ALL, Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa8df-117">For **user** or **chat** resource: Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="fa8df-118">Для ресурса **Channel** : Member. Read. Group \*, Чаннелмембер. Read. ALL, Чаннелмембер. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa8df-118">For **channel** resource: Member.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="fa8df-119">**Note**: разрешения, помеченные как \* использовать [согласие с определенным ресурсом](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="fa8df-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="fa8df-120">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="fa8df-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="fa8df-121">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="fa8df-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="fa8df-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa8df-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa8df-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa8df-123">Optional query parameters</span></span>

<span data-ttu-id="fa8df-124">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="fa8df-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa8df-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa8df-125">Request headers</span></span>

| <span data-ttu-id="fa8df-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa8df-126">Header</span></span>       | <span data-ttu-id="fa8df-127">Значение</span><span class="sxs-lookup"><span data-stu-id="fa8df-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa8df-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa8df-128">Authorization</span></span>  | <span data-ttu-id="fa8df-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa8df-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa8df-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa8df-131">Request body</span></span>

<span data-ttu-id="fa8df-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa8df-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa8df-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa8df-133">Response</span></span>

<span data-ttu-id="fa8df-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa8df-134">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa8df-135">Пример</span><span class="sxs-lookup"><span data-stu-id="fa8df-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa8df-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa8df-136">Request</span></span>

<span data-ttu-id="fa8df-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa8df-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa8df-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa8df-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="fa8df-139">C#</span><span class="sxs-lookup"><span data-stu-id="fa8df-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa8df-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa8df-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa8df-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa8df-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fa8df-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa8df-142">Response</span></span>

<span data-ttu-id="fa8df-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa8df-143">Here is an example of the response.</span></span>

><span data-ttu-id="fa8df-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa8df-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
