---
title: Список hostedContents
description: Извлечение списка объектов chatMessageHostedContent из сообщения.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 79e020bb53c995ac1afe2d53dc4b0b367d42a201
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971108"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="ad6bd-103">Список hostedContents</span><span class="sxs-lookup"><span data-stu-id="ad6bd-103">List hostedContents</span></span>

<span data-ttu-id="ad6bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad6bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad6bd-105">Извлечение списка [объектов chatMessageHostedContent](../resources/chatmessagehostedcontent.md) из сообщения.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span> <span data-ttu-id="ad6bd-106">В этом API перечислены только объекты контента, которые находятся на хостинге.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-106">This API only lists the hosted content objects.</span></span> <span data-ttu-id="ad6bd-107">Чтобы получить bytes контента, [см. в странице get chatmessage hosted content](chatmessagehostedcontent-get.md)</span><span class="sxs-lookup"><span data-stu-id="ad6bd-107">To get the content bytes, see [get chatmessage hosted content](chatmessagehostedcontent-get.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="ad6bd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad6bd-108">Permissions</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="ad6bd-109">Разрешения для канала</span><span class="sxs-lookup"><span data-stu-id="ad6bd-109">Permissions for channel</span></span>

| <span data-ttu-id="ad6bd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad6bd-110">Permission type</span></span>                        | <span data-ttu-id="ad6bd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad6bd-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="ad6bd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad6bd-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ad6bd-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="ad6bd-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="ad6bd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad6bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad6bd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-115">Not supported.</span></span>|
|<span data-ttu-id="ad6bd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad6bd-116">Application</span></span>| <span data-ttu-id="ad6bd-117">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad6bd-117">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="ad6bd-118">Разрешения для чата</span><span class="sxs-lookup"><span data-stu-id="ad6bd-118">Permissions for chat</span></span>

| <span data-ttu-id="ad6bd-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad6bd-119">Permission type</span></span>                        | <span data-ttu-id="ad6bd-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad6bd-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="ad6bd-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad6bd-121">Delegated (work or school account)</span></span>| <span data-ttu-id="ad6bd-122">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad6bd-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="ad6bd-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad6bd-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad6bd-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-124">Not supported.</span></span>|
|<span data-ttu-id="ad6bd-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="ad6bd-125">Application</span></span>| <span data-ttu-id="ad6bd-126">ChatMessage.Read.Chat\*, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad6bd-126">ChatMessage.Read.Chat\*, Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="ad6bd-127">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="ad6bd-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="ad6bd-128">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="ad6bd-129">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="ad6bd-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="ad6bd-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad6bd-130">HTTP request</span></span>

<span data-ttu-id="ad6bd-131">**Получить hostedContents в сообщении канала**</span><span class="sxs-lookup"><span data-stu-id="ad6bd-131">**Get hostedContents in a channel message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}/hostedContents
```

<span data-ttu-id="ad6bd-132">**Получить hostedContents в сообщении чата**</span><span class="sxs-lookup"><span data-stu-id="ad6bd-132">**Get hostedContents in a chat message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}/hostedContents
GET /users/{user-id | user-principal-name}/chats/{chat-id}/messages/{message-id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad6bd-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ad6bd-133">Optional query parameters</span></span>

<span data-ttu-id="ad6bd-134">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-134">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad6bd-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad6bd-135">Request headers</span></span>

| <span data-ttu-id="ad6bd-136">Имя</span><span class="sxs-lookup"><span data-stu-id="ad6bd-136">Name</span></span>      |<span data-ttu-id="ad6bd-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ad6bd-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad6bd-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad6bd-138">Authorization</span></span> | <span data-ttu-id="ad6bd-139">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ad6bd-139">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad6bd-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad6bd-140">Request body</span></span>

<span data-ttu-id="ad6bd-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad6bd-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad6bd-142">Response</span></span>

<span data-ttu-id="ad6bd-143">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-143">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad6bd-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="ad6bd-144">Examples</span></span>

### <a name="example-1-list-hosted-content-for-a-channel-message"></a><span data-ttu-id="ad6bd-145">Пример 1. Список содержимого для сообщения канала</span><span class="sxs-lookup"><span data-stu-id="ad6bd-145">Example 1: List hosted content for a channel message</span></span>

#### <a name="request"></a><span data-ttu-id="ad6bd-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad6bd-146">Request</span></span>

<span data-ttu-id="ad6bd-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad6bd-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad6bd-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschannelmessage_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="ad6bd-149">C#</span><span class="sxs-lookup"><span data-stu-id="ad6bd-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentschannelmessage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad6bd-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad6bd-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentschannelmessage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad6bd-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad6bd-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentschannelmessage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad6bd-152">Java</span><span class="sxs-lookup"><span data-stu-id="ad6bd-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentschannelmessage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ad6bd-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad6bd-153">Response</span></span>

<span data-ttu-id="ad6bd-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-154">The following is an example of the response.</span></span>

> <span data-ttu-id="ad6bd-155">**Примечание:** `contentBytes` и `contentType` всегда настроены на нуль.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-155">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616963377068')/hostedContents",
    "@odata.count": 2,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZC92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        },
        {
            "id": "aWQ9eF8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNC92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

### <a name="example-2-list-hosted-content-for-reply-to-a-channel-message"></a><span data-ttu-id="ad6bd-156">Пример 2. Список содержимого для ответа на сообщение канала</span><span class="sxs-lookup"><span data-stu-id="ad6bd-156">Example 2: List hosted content for reply to a channel message</span></span>

#### <a name="request"></a><span data-ttu-id="ad6bd-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad6bd-157">Request</span></span>

<span data-ttu-id="ad6bd-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-158">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad6bd-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad6bd-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschannelmessage_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/replies/1616963389737/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="ad6bd-160">C#</span><span class="sxs-lookup"><span data-stu-id="ad6bd-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentschannelmessage-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad6bd-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad6bd-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentschannelmessage-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad6bd-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad6bd-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentschannelmessage-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad6bd-163">Java</span><span class="sxs-lookup"><span data-stu-id="ad6bd-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentschannelmessage-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ad6bd-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad6bd-164">Response</span></span>

<span data-ttu-id="ad6bd-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-165">The following is an example of the response.</span></span>

> <span data-ttu-id="ad6bd-166">**Примечание:** `contentBytes` и `contentType` всегда настроены на нуль.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-166">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616963377068')/replies('1616963389737')/hostedContents",
    "@odata.count": 2,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kMy1hMDE3MmZiYjVkYzcxNGM4NWU5NDQwNWE5ZjNkNThmYyx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kMy1hMDE3MmZiYjVkYzcxNGM4NWU5NDQwNWE5ZjNkNThmYy92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        },
        {
            "id": "aWQ9eF8wLXd1cy1kOS03ZDlmOGVlMzk4ZGQ3YTZkMDdhMDg4OGI5ODZlNDdkYyx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS03ZDlmOGVlMzk4ZGQ3YTZkMDdhMDg4OGI5ODZlNDdkYy92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

### <a name="example-2--list-hosted-content-for-message-in-a-chat"></a><span data-ttu-id="ad6bd-167">Пример 2. Список содержимого для сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="ad6bd-167">Example 2 : List hosted content for message in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="ad6bd-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad6bd-168">Request</span></span>

<span data-ttu-id="ad6bd-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad6bd-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad6bd-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschatmessage_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="ad6bd-171">C#</span><span class="sxs-lookup"><span data-stu-id="ad6bd-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentschatmessage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad6bd-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad6bd-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentschatmessage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad6bd-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad6bd-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentschatmessage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad6bd-174">Java</span><span class="sxs-lookup"><span data-stu-id="ad6bd-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentschatmessage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ad6bd-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad6bd-175">Response</span></span>

<span data-ttu-id="ad6bd-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-176">The following is an example of the response.</span></span>

> <span data-ttu-id="ad6bd-177">**Примечание:** `contentBytes` и `contentType` всегда настроены на нуль.</span><span class="sxs-lookup"><span data-stu-id="ad6bd-177">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages('1615971548136')/hostedContents",
    "@odata.count": 1,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List hostedContents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


