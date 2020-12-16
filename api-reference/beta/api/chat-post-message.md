---
title: Отправка chatMessage в чате
description: Отправка нового chatMessage в чате.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7f0e18946903c2926b8c26241b7dbdd7fdbf5851
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689761"
---
# <a name="send-chatmessage-in-a-chat"></a><span data-ttu-id="9f030-103">Отправка chatMessage в чате</span><span class="sxs-lookup"><span data-stu-id="9f030-103">Send chatMessage in a chat</span></span>

<span data-ttu-id="9f030-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f030-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f030-105">Создайте новый [chatMessage](../resources/chatmessage.md) в указанном [чате.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="9f030-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="9f030-106">Этот API не может создать новый чат; Перед созданием сообщения [чата](chat-list.md) необходимо использовать метод чаты списка для получения ИД существующего чата.</span><span class="sxs-lookup"><span data-stu-id="9f030-106">This API cannot create a new chat; you must use the [list chats](chat-list.md) method to retrieve the ID of an existing chat before creating a chat message.</span></span>

> <span data-ttu-id="9f030-107">**Примечание.** Мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="9f030-107">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="9f030-108">Пропускная способность, необходимая для обычной миграции, не существует.</span><span class="sxs-lookup"><span data-stu-id="9f030-108">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="9f030-109">**Примечание.** Это нарушение условий использования Microsoft Teams в качестве файла журнала. [](/legal/microsoft-apis/terms-of-use)</span><span class="sxs-lookup"><span data-stu-id="9f030-109">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="9f030-110">Отправлять только сообщения, которые люди будут читать.</span><span class="sxs-lookup"><span data-stu-id="9f030-110">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f030-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f030-111">Permissions</span></span>

<span data-ttu-id="9f030-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f030-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f030-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f030-114">Permission type</span></span>                        | <span data-ttu-id="9f030-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f030-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9f030-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f030-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f030-117">ChatMessage.Send, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f030-117">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="9f030-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f030-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f030-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f030-119">Not supported.</span></span> |
| <span data-ttu-id="9f030-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f030-120">Application</span></span>                            | <span data-ttu-id="9f030-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f030-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f030-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f030-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="9f030-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f030-123">Request headers</span></span>

| <span data-ttu-id="9f030-124">Имя</span><span class="sxs-lookup"><span data-stu-id="9f030-124">Name</span></span>          | <span data-ttu-id="9f030-125">Описание</span><span class="sxs-lookup"><span data-stu-id="9f030-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9f030-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f030-126">Authorization</span></span> | <span data-ttu-id="9f030-127">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="9f030-127">Bearer {code}.</span></span> <span data-ttu-id="9f030-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9f030-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f030-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f030-129">Request body</span></span>

<span data-ttu-id="9f030-130">В теле запроса укажу представление объекта [chatMessage](../resources/chatmessage.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="9f030-130">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9f030-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f030-131">Response</span></span>

<span data-ttu-id="9f030-132">В случае успеха этот метод возвращает код отклика и новый объект `201 Created` [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f030-132">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f030-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="9f030-133">Examples</span></span>

<span data-ttu-id="9f030-134">Более полный список примеров см. в примере [создания chatMessage в канале или чате.](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="9f030-134">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="9f030-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f030-135">Request</span></span>

<span data-ttu-id="9f030-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f030-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f030-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f030-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chat"
}-->

```http
POST https://graph.microsoft.com/beta/chats/{id}/messages
Content-type: application/json

{
  "body": {
     "content": "Hello world"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="9f030-138">C#</span><span class="sxs-lookup"><span data-stu-id="9f030-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f030-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f030-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f030-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f030-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f030-141">Java</span><span class="sxs-lookup"><span data-stu-id="9f030-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9f030-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f030-142">Response</span></span>

<span data-ttu-id="9f030-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f030-143">The following is an example of the response.</span></span>

> <span data-ttu-id="9f030-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f030-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
