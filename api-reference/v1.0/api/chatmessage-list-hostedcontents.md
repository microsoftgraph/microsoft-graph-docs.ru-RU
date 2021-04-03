---
title: Список hostedContents
description: Извлечение списка объектов chatMessageHostedContent из сообщения.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 40a3f5c3613b5dc590c97a9854b859267cb4dedf
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582932"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="79f79-103">Список hostedContents</span><span class="sxs-lookup"><span data-stu-id="79f79-103">List hostedContents</span></span>

<span data-ttu-id="79f79-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79f79-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79f79-105">Извлечение списка [объектов chatMessageHostedContent](../resources/chatmessagehostedcontent.md) из сообщения.</span><span class="sxs-lookup"><span data-stu-id="79f79-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span> <span data-ttu-id="79f79-106">В этом API перечислены только объекты контента, которые находятся на хостинге.</span><span class="sxs-lookup"><span data-stu-id="79f79-106">This API only lists the hosted content objects.</span></span> <span data-ttu-id="79f79-107">Чтобы получить bytes контента, [см. в странице get chatmessage hosted content](chatmessagehostedcontent-get.md)</span><span class="sxs-lookup"><span data-stu-id="79f79-107">To get the content bytes, see [get chatmessage hosted content](chatmessagehostedcontent-get.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="79f79-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79f79-108">Permissions</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="79f79-109">Разрешения для канала</span><span class="sxs-lookup"><span data-stu-id="79f79-109">Permissions for channel</span></span>

| <span data-ttu-id="79f79-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79f79-110">Permission type</span></span>                        | <span data-ttu-id="79f79-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79f79-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="79f79-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79f79-112">Delegated (work or school account)</span></span>| <span data-ttu-id="79f79-113">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="79f79-113">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="79f79-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79f79-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79f79-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79f79-115">Not supported.</span></span>|
|<span data-ttu-id="79f79-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79f79-116">Application</span></span>| <span data-ttu-id="79f79-117">ChannelMessage.Read.Group, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="79f79-117">ChannelMessage.Read.Group, ChannelMessage.Read.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="79f79-118">Разрешения для чата</span><span class="sxs-lookup"><span data-stu-id="79f79-118">Permissions for chat</span></span>

| <span data-ttu-id="79f79-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79f79-119">Permission type</span></span>                        | <span data-ttu-id="79f79-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79f79-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="79f79-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79f79-121">Delegated (work or school account)</span></span>| <span data-ttu-id="79f79-122">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79f79-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="79f79-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79f79-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79f79-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79f79-124">Not supported.</span></span>|
|<span data-ttu-id="79f79-125">Для приложения</span><span class="sxs-lookup"><span data-stu-id="79f79-125">Application</span></span>| <span data-ttu-id="79f79-126">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79f79-126">Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="79f79-127">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="79f79-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="79f79-128">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="79f79-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="79f79-129">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="79f79-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="79f79-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79f79-130">HTTP request</span></span>

<span data-ttu-id="79f79-131">**Получить hostedContents в сообщении канала**</span><span class="sxs-lookup"><span data-stu-id="79f79-131">**Get hostedContents in a channel message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}/hostedContents
```

<span data-ttu-id="79f79-132">**Получить hostedContents в сообщении чата**</span><span class="sxs-lookup"><span data-stu-id="79f79-132">**Get hostedContents in a chat message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}/hostedContents
GET /users/{user-id}/chats/{chat-id}/messages/{message-id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79f79-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="79f79-133">Optional query parameters</span></span>

<span data-ttu-id="79f79-134">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="79f79-134">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79f79-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79f79-135">Request headers</span></span>

| <span data-ttu-id="79f79-136">Имя</span><span class="sxs-lookup"><span data-stu-id="79f79-136">Name</span></span>      |<span data-ttu-id="79f79-137">Описание</span><span class="sxs-lookup"><span data-stu-id="79f79-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="79f79-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79f79-138">Authorization</span></span> | <span data-ttu-id="79f79-139">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="79f79-139">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="79f79-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79f79-140">Request body</span></span>

<span data-ttu-id="79f79-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79f79-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79f79-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="79f79-142">Response</span></span>

<span data-ttu-id="79f79-143">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="79f79-143">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79f79-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="79f79-144">Examples</span></span>

### <a name="example-1-list-hosted-content-for-a-channel-message"></a><span data-ttu-id="79f79-145">Пример 1. Список содержимого для сообщения канала</span><span class="sxs-lookup"><span data-stu-id="79f79-145">Example 1: List hosted content for a channel message</span></span>

#### <a name="request"></a><span data-ttu-id="79f79-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="79f79-146">Request</span></span>

<span data-ttu-id="79f79-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79f79-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschannelmessage_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents
```

#### <a name="response"></a><span data-ttu-id="79f79-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="79f79-148">Response</span></span>

<span data-ttu-id="79f79-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="79f79-149">The following is an example of the response.</span></span>

> <span data-ttu-id="79f79-150">**Примечание:** `contentBytes` и `contentType` всегда настроены на нуль.</span><span class="sxs-lookup"><span data-stu-id="79f79-150">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616963377068')/hostedContents",
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

### <a name="example-2-list-hosted-content-for-reply-to-a-channel-message"></a><span data-ttu-id="79f79-151">Пример 2. Список содержимого для ответа на сообщение канала</span><span class="sxs-lookup"><span data-stu-id="79f79-151">Example 2: List hosted content for reply to a channel message</span></span>

#### <a name="request"></a><span data-ttu-id="79f79-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="79f79-152">Request</span></span>

<span data-ttu-id="79f79-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79f79-153">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschannelmessage_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/replies/1616963389737/hostedContents
```

#### <a name="response"></a><span data-ttu-id="79f79-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="79f79-154">Response</span></span>

<span data-ttu-id="79f79-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="79f79-155">The following is an example of the response.</span></span>

> <span data-ttu-id="79f79-156">**Примечание:** `contentBytes` и `contentType` всегда настроены на нуль.</span><span class="sxs-lookup"><span data-stu-id="79f79-156">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616963377068')/replies('1616963389737')/hostedContents",
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

### <a name="example-2--list-hosted-content-for-message-in-a-chat"></a><span data-ttu-id="79f79-157">Пример 2. Список содержимого для сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="79f79-157">Example 2 : List hosted content for message in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="79f79-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="79f79-158">Request</span></span>

<span data-ttu-id="79f79-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79f79-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschatmessage_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents
```

#### <a name="response"></a><span data-ttu-id="79f79-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="79f79-160">Response</span></span>

<span data-ttu-id="79f79-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="79f79-161">The following is an example of the response.</span></span>

> <span data-ttu-id="79f79-162">**Примечание:** `contentBytes` и `contentType` всегда настроены на нуль.</span><span class="sxs-lookup"><span data-stu-id="79f79-162">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages('1615971548136')/hostedContents",
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


