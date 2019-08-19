---
title: Создание chatMessage
description: Используйте этот API для создания нового chatMessage.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 96099cf2628b31a03013ae680439e97a55f952c5
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460824"
---
# <a name="create-chatmessage"></a><span data-ttu-id="3e83c-103">Создание chatMessage</span><span class="sxs-lookup"><span data-stu-id="3e83c-103">Create chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e83c-104">Создайте новое [сообщение](../resources/chatmessage.md) в указанном [сеансе чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="3e83c-104">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="3e83c-105">Этот API не может создать новый чат. для того, чтобы получить сообщение чата, необходимо использовать метод [List Chats](chat-list.md) для извлечения идентификатора существующего чата.</span><span class="sxs-lookup"><span data-stu-id="3e83c-105">This API cannot create an new chat, you must use the [list chats](chat-list.md) method to retreive the Id of an existing chat before creating a chat message.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e83c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e83c-106">Permissions</span></span>

<span data-ttu-id="3e83c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e83c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e83c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e83c-109">Permission type</span></span>                        | <span data-ttu-id="3e83c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e83c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3e83c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e83c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e83c-112">Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e83c-112">Chat.ReadWrite</span></span> |
| <span data-ttu-id="3e83c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e83c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e83c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e83c-114">Not supported.</span></span> |
| <span data-ttu-id="3e83c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e83c-115">Application</span></span>                            | <span data-ttu-id="3e83c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e83c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e83c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e83c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="3e83c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e83c-118">Request headers</span></span>

| <span data-ttu-id="3e83c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3e83c-119">Name</span></span>          | <span data-ttu-id="3e83c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3e83c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3e83c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e83c-121">Authorization</span></span> | <span data-ttu-id="3e83c-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3e83c-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e83c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e83c-123">Request body</span></span>

<span data-ttu-id="3e83c-124">В тексте запроса добавьте представление объекта [chatMessage](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e83c-124">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3e83c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e83c-125">Response</span></span>

<span data-ttu-id="3e83c-126">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e83c-126">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e83c-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="3e83c-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e83c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e83c-128">Request</span></span>

<span data-ttu-id="3e83c-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e83c-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3e83c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e83c-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e83c-131">C#</span><span class="sxs-lookup"><span data-stu-id="3e83c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e83c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e83c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e83c-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3e83c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e83c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e83c-134">Response</span></span>

<span data-ttu-id="3e83c-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3e83c-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="3e83c-136">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3e83c-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3e83c-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e83c-137">All the properties will be returned from an actual call.</span></span>

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
