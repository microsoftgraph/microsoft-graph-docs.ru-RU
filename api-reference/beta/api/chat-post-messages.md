---
title: Создание chatMessage
description: Используйте этот API для создания нового chatMessage.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 917b5ec5ac140079f30f6c03db485de849d6b56b
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287516"
---
# <a name="create-chatmessage"></a><span data-ttu-id="d5039-103">Создание chatMessage</span><span class="sxs-lookup"><span data-stu-id="d5039-103">Create chatMessage</span></span>

<span data-ttu-id="d5039-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5039-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5039-105">Создайте новое [сообщение](../resources/chatmessage.md) в указанном [сеансе чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="d5039-105">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="d5039-106">Этот API не может создать новый чат. для того, чтобы получить сообщение чата, необходимо использовать метод [List Chats](chat-list.md) для извлечения идентификатора существующего чата.</span><span class="sxs-lookup"><span data-stu-id="d5039-106">This API cannot create an new chat, you must use the [list chats](chat-list.md) method to retreive the Id of an existing chat before creating a chat message.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5039-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5039-107">Permissions</span></span>

<span data-ttu-id="d5039-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5039-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5039-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5039-110">Permission type</span></span>                        | <span data-ttu-id="d5039-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5039-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d5039-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5039-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5039-113">ChatMessage. Send, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5039-113">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="d5039-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5039-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5039-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5039-115">Not supported.</span></span> |
| <span data-ttu-id="d5039-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5039-116">Application</span></span>                            | <span data-ttu-id="d5039-117">Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d5039-117">Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5039-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5039-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="d5039-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5039-119">Request headers</span></span>

| <span data-ttu-id="d5039-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d5039-120">Name</span></span>          | <span data-ttu-id="d5039-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d5039-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d5039-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5039-122">Authorization</span></span> | <span data-ttu-id="d5039-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d5039-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5039-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5039-124">Request body</span></span>

<span data-ttu-id="d5039-125">В тексте запроса добавьте представление объекта [chatMessage](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5039-125">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d5039-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5039-126">Response</span></span>

<span data-ttu-id="d5039-127">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5039-127">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5039-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d5039-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5039-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5039-129">Request</span></span>

<span data-ttu-id="d5039-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5039-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5039-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5039-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chat"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
     "content" : "Hello world"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="d5039-132">C#</span><span class="sxs-lookup"><span data-stu-id="d5039-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5039-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5039-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5039-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5039-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d5039-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5039-135">Response</span></span>

<span data-ttu-id="d5039-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d5039-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d5039-137">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d5039-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d5039-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5039-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "replyToId": "replyToId-value",
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "87ea812c-8816-40e9-b770-5c165fa31397",
      "displayName": "Test User"
    }
  },
  "messageType": "message",
  "body": {
     "content": "Hello world",
     "contentType": "text"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
