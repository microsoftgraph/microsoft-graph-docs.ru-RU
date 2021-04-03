---
title: Get chatMessageHostedContent
description: Извлечение свойств и связей объекта chatMessageHostedContent.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c2de6f182904a13d2fc36f2bf398a3784fed3d1f
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582615"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="ac0a6-103">Get chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="ac0a6-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="ac0a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac0a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac0a6-105">Извлечение свойств и связей [объекта chatMessageHostedContent.](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="ac0a6-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac0a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac0a6-106">Permissions</span></span>

<span data-ttu-id="ac0a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac0a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="ac0a6-109">Разрешения для канала</span><span class="sxs-lookup"><span data-stu-id="ac0a6-109">Permissions for channel</span></span>

| <span data-ttu-id="ac0a6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac0a6-110">Permission type</span></span>                        | <span data-ttu-id="ac0a6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac0a6-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="ac0a6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac0a6-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ac0a6-113">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac0a6-113">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="ac0a6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac0a6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac0a6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-115">Not supported.</span></span>|
|<span data-ttu-id="ac0a6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac0a6-116">Application</span></span>| <span data-ttu-id="ac0a6-117">ChannelMessage.Read.Group, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac0a6-117">ChannelMessage.Read.Group, ChannelMessage.Read.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="ac0a6-118">Разрешения для чата</span><span class="sxs-lookup"><span data-stu-id="ac0a6-118">Permissions for chat</span></span>

| <span data-ttu-id="ac0a6-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac0a6-119">Permission type</span></span>                        | <span data-ttu-id="ac0a6-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac0a6-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="ac0a6-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac0a6-121">Delegated (work or school account)</span></span>| <span data-ttu-id="ac0a6-122">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac0a6-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="ac0a6-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac0a6-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac0a6-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-124">Not supported.</span></span>|
|<span data-ttu-id="ac0a6-125">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ac0a6-125">Application</span></span>| <span data-ttu-id="ac0a6-126">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac0a6-126">Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="ac0a6-127">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="ac0a6-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="ac0a6-128">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="ac0a6-129">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="ac0a6-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="ac0a6-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac0a6-130">HTTP request</span></span>

<span data-ttu-id="ac0a6-131">**Получать контент в сообщении канала**</span><span class="sxs-lookup"><span data-stu-id="ac0a6-131">**Get hosted content in a channel message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents/{hosted-content-id}
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}/hostedContents/{hosted-content-id}
```

<span data-ttu-id="ac0a6-132">**Получать контент в сообщении чата**</span><span class="sxs-lookup"><span data-stu-id="ac0a6-132">**Get hosted content in a chat message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}/hostedContents/{hosted-content-id}
GET /users/{user-id}/chats/{chat-id}/messages/{message-id}/hostedContents/{hosted-content-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac0a6-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ac0a6-133">Optional query parameters</span></span>

<span data-ttu-id="ac0a6-134">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-134">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac0a6-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac0a6-135">Request headers</span></span>

| <span data-ttu-id="ac0a6-136">Имя</span><span class="sxs-lookup"><span data-stu-id="ac0a6-136">Name</span></span>      |<span data-ttu-id="ac0a6-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ac0a6-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ac0a6-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac0a6-138">Authorization</span></span> | <span data-ttu-id="ac0a6-139">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ac0a6-139">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac0a6-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac0a6-140">Request body</span></span>

<span data-ttu-id="ac0a6-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac0a6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac0a6-142">Response</span></span>

<span data-ttu-id="ac0a6-143">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-143">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac0a6-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="ac0a6-144">Examples</span></span>

### <a name="example-1-get-hosted-content-for-message-in-a-chat"></a><span data-ttu-id="ac0a6-145">Пример 1. Для получения содержимого для сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="ac0a6-145">Example 1: Get hosted content for message in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="ac0a6-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac0a6-146">Request</span></span>

<span data-ttu-id="ac0a6-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hostedcontentchatmessage_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv
```
#### <a name="response"></a><span data-ttu-id="ac0a6-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac0a6-148">Response</span></span>

<span data-ttu-id="ac0a6-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-149">The following is an example of the response.</span></span>

> <span data-ttu-id="ac0a6-150">**Примечание:** `contentBytes` и `contentType` всегда настроены на нуль.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-150">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages('1615971548136')/hostedContents/$entity",
    "id": "aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="ac0a6-151">Пример 2. Получить у себя bytes контента для изображения</span><span class="sxs-lookup"><span data-stu-id="ac0a6-151">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="ac0a6-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac0a6-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hostedcontentchatmessage_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv/$value
```

#### <a name="response"></a><span data-ttu-id="ac0a6-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac0a6-153">Response</span></span>

<span data-ttu-id="ac0a6-154">Ответ содержит bytes для размещенного контента в теле.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-154">Response contains bytes for the hosted content in the body.</span></span> <span data-ttu-id="ac0a6-155">`content-type` Заглавный заглавник указывает тип содержимого, на который установлено.</span><span class="sxs-lookup"><span data-stu-id="ac0a6-155">`content-type` header specifies the kind of hosted content.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
content-type: image/png
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


