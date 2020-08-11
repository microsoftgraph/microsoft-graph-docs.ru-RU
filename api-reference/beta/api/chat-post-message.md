---
title: Отправка chatMessage в чате
description: Отправка нового chatMessage в чате.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4d7660d1360216e4bc648d98e2899ead2aff0064
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630465"
---
# <a name="send-chatmessage-in-a-chat"></a><span data-ttu-id="d4e8e-103">Отправка chatMessage в чате</span><span class="sxs-lookup"><span data-stu-id="d4e8e-103">Send chatMessage in a chat</span></span>

<span data-ttu-id="d4e8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4e8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4e8e-105">Создание нового [chatMessage](../resources/chatmessage.md) в указанном [сеансе чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="d4e8e-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="d4e8e-106">Этот API не может создать новый чат; чтобы получить идентификатор существующего чата, прежде чем создавать сообщение чата, необходимо использовать метод [List Chats](chat-list.md) .</span><span class="sxs-lookup"><span data-stu-id="d4e8e-106">This API cannot create an new chat; you must use the [list chats](chat-list.md) method to retreive the ID of an existing chat before creating a chat message.</span></span>

> <span data-ttu-id="d4e8e-107">**Note**: мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-107">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="d4e8e-108">Пропускная способность, необходимая для обычной миграции, отсутствует.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-108">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="d4e8e-109">**Note**: нарушение [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) Microsoft Teams в качестве файла журнала.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-109">**Note**: It is a violation of the [terms of use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="d4e8e-110">Отправлять только сообщения, которые пользователи смогут читать.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-110">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4e8e-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4e8e-111">Permissions</span></span>

<span data-ttu-id="d4e8e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4e8e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4e8e-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4e8e-114">Permission type</span></span>                        | <span data-ttu-id="d4e8e-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4e8e-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4e8e-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4e8e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4e8e-117">ChatMessage. Send, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4e8e-117">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="d4e8e-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4e8e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4e8e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-119">Not supported.</span></span> |
| <span data-ttu-id="d4e8e-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4e8e-120">Application</span></span>                            | <span data-ttu-id="d4e8e-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4e8e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4e8e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="d4e8e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4e8e-123">Request headers</span></span>

| <span data-ttu-id="d4e8e-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d4e8e-124">Name</span></span>          | <span data-ttu-id="d4e8e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d4e8e-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d4e8e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4e8e-126">Authorization</span></span> | <span data-ttu-id="d4e8e-127">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-127">Bearer {code}.</span></span> <span data-ttu-id="d4e8e-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4e8e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4e8e-129">Request body</span></span>

<span data-ttu-id="d4e8e-130">В тексте запроса добавьте представление объекта [chatMessage](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-130">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d4e8e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4e8e-131">Response</span></span>

<span data-ttu-id="d4e8e-132">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-132">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4e8e-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4e8e-133">Examples</span></span>

<span data-ttu-id="d4e8e-134">Более полный список примеров приведен [в статье Создание chatMessage в канале или чате](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="d4e8e-134">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="d4e8e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4e8e-135">Request</span></span>

<span data-ttu-id="d4e8e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4e8e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4e8e-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d4e8e-138">C#</span><span class="sxs-lookup"><span data-stu-id="d4e8e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4e8e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4e8e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4e8e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4e8e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d4e8e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4e8e-141">Response</span></span>

<span data-ttu-id="d4e8e-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-142">The following is an example of the response.</span></span>

> <span data-ttu-id="d4e8e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4e8e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
