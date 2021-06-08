---
title: Get chatMessageHostedContent
description: Извлечение свойств и связей объекта chatMessageHostedContent.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a2729a3c78c1931afc57b308418a86ea06c446c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786189"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="616eb-103">Get chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="616eb-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="616eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="616eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="616eb-105">Извлечение свойств и связей [объекта chatMessageHostedContent.](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="616eb-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="616eb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="616eb-106">Permissions</span></span>

<span data-ttu-id="616eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="616eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="616eb-109">Разрешения для канала</span><span class="sxs-lookup"><span data-stu-id="616eb-109">Permissions for channel</span></span>

| <span data-ttu-id="616eb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="616eb-110">Permission type</span></span>                        | <span data-ttu-id="616eb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="616eb-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="616eb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="616eb-112">Delegated (work or school account)</span></span>| <span data-ttu-id="616eb-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="616eb-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="616eb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="616eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="616eb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="616eb-115">Not supported.</span></span>|
|<span data-ttu-id="616eb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="616eb-116">Application</span></span>| <span data-ttu-id="616eb-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="616eb-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="616eb-118">Разрешения для чата</span><span class="sxs-lookup"><span data-stu-id="616eb-118">Permissions for chat</span></span>

| <span data-ttu-id="616eb-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="616eb-119">Permission type</span></span>                        | <span data-ttu-id="616eb-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="616eb-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="616eb-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="616eb-121">Delegated (work or school account)</span></span>| <span data-ttu-id="616eb-122">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="616eb-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="616eb-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="616eb-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="616eb-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="616eb-124">Not supported.</span></span>|
|<span data-ttu-id="616eb-125">Для приложения</span><span class="sxs-lookup"><span data-stu-id="616eb-125">Application</span></span>| <span data-ttu-id="616eb-126">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="616eb-126">Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="616eb-127">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="616eb-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="616eb-128">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="616eb-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="616eb-129">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="616eb-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="616eb-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="616eb-130">HTTP request</span></span>

<span data-ttu-id="616eb-131">**Получать контент в сообщении канала**</span><span class="sxs-lookup"><span data-stu-id="616eb-131">**Get hosted content in a channel message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents/{hosted-content-id}
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}/hostedContents/{hosted-content-id}
```

<span data-ttu-id="616eb-132">**Получать контент в сообщении чата**</span><span class="sxs-lookup"><span data-stu-id="616eb-132">**Get hosted content in a chat message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}/hostedContents/{hosted-content-id}
GET /users/{user-id | user-principal-name}/chats/{chat-id}/messages/{message-id}/hostedContents/{hosted-content-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="616eb-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="616eb-133">Optional query parameters</span></span>

<span data-ttu-id="616eb-134">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="616eb-134">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="616eb-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="616eb-135">Request headers</span></span>

| <span data-ttu-id="616eb-136">Имя</span><span class="sxs-lookup"><span data-stu-id="616eb-136">Name</span></span>      |<span data-ttu-id="616eb-137">Описание</span><span class="sxs-lookup"><span data-stu-id="616eb-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="616eb-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="616eb-138">Authorization</span></span> | <span data-ttu-id="616eb-139">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="616eb-139">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="616eb-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="616eb-140">Request body</span></span>

<span data-ttu-id="616eb-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="616eb-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="616eb-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="616eb-142">Response</span></span>

<span data-ttu-id="616eb-143">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="616eb-143">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="616eb-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="616eb-144">Examples</span></span>

### <a name="example-1-get-hosted-content-for-message-in-a-chat"></a><span data-ttu-id="616eb-145">Пример 1. Для получения содержимого для сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="616eb-145">Example 1: Get hosted content for message in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="616eb-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="616eb-146">Request</span></span>

<span data-ttu-id="616eb-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="616eb-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="616eb-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="616eb-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentchatmessage_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv
```
# <a name="c"></a>[<span data-ttu-id="616eb-149">C#</span><span class="sxs-lookup"><span data-stu-id="616eb-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentchatmessage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="616eb-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="616eb-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentchatmessage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="616eb-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="616eb-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentchatmessage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="616eb-152">Java</span><span class="sxs-lookup"><span data-stu-id="616eb-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentchatmessage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="616eb-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="616eb-153">Response</span></span>

<span data-ttu-id="616eb-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="616eb-154">The following is an example of the response.</span></span>

> <span data-ttu-id="616eb-155">**Примечание:** `contentBytes` и `contentType` всегда настроены на нуль.</span><span class="sxs-lookup"><span data-stu-id="616eb-155">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages('1615971548136')/hostedContents/$entity",
    "id": "aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="616eb-156">Пример 2. Получить у себя bytes контента для изображения</span><span class="sxs-lookup"><span data-stu-id="616eb-156">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="616eb-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="616eb-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="616eb-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="616eb-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentchatmessage_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv/$value
```
# <a name="c"></a>[<span data-ttu-id="616eb-159">C#</span><span class="sxs-lookup"><span data-stu-id="616eb-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentchatmessage-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="616eb-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="616eb-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentchatmessage-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="616eb-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="616eb-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentchatmessage-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="616eb-162">Java</span><span class="sxs-lookup"><span data-stu-id="616eb-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentchatmessage-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="616eb-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="616eb-163">Response</span></span>

<span data-ttu-id="616eb-164">Ответ содержит bytes для размещенного контента в теле.</span><span class="sxs-lookup"><span data-stu-id="616eb-164">Response contains bytes for the hosted content in the body.</span></span> <span data-ttu-id="616eb-165">`content-type` Заглавный заглавник указывает тип содержимого, на который установлено.</span><span class="sxs-lookup"><span data-stu-id="616eb-165">`content-type` header specifies the kind of hosted content.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201

{
  "id": "id-value"
}
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


