---
title: Создание chatMessage
description: Используйте этот API для создания нового chatMessage.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 62fbbabb3ad50b00706d717dd9b4d2a7a8db97de
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437819"
---
# <a name="create-chatmessage"></a><span data-ttu-id="bb23d-103">Создание chatMessage</span><span class="sxs-lookup"><span data-stu-id="bb23d-103">Create chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb23d-104">Создайте новое [сообщение](../resources/chatmessage.md) в указанном [сеансе чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="bb23d-104">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb23d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb23d-105">Permissions</span></span>

<span data-ttu-id="bb23d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb23d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb23d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb23d-108">Permission type</span></span>                        | <span data-ttu-id="bb23d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb23d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bb23d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb23d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb23d-111">Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb23d-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="bb23d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb23d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb23d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb23d-113">Not supported.</span></span> |
| <span data-ttu-id="bb23d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb23d-114">Application</span></span>                            | <span data-ttu-id="bb23d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb23d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb23d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb23d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="bb23d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb23d-117">Request headers</span></span>

| <span data-ttu-id="bb23d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bb23d-118">Name</span></span>          | <span data-ttu-id="bb23d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bb23d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bb23d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb23d-120">Authorization</span></span> | <span data-ttu-id="bb23d-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bb23d-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb23d-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb23d-122">Request body</span></span>

<span data-ttu-id="bb23d-123">В тексте запроса добавьте представление объекта [chatMessage](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb23d-123">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bb23d-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb23d-124">Response</span></span>

<span data-ttu-id="bb23d-125">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb23d-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb23d-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="bb23d-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb23d-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb23d-127">Request</span></span>

<span data-ttu-id="bb23d-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb23d-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bb23d-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb23d-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb23d-130">C#</span><span class="sxs-lookup"><span data-stu-id="bb23d-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb23d-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb23d-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb23d-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bb23d-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bb23d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb23d-133">Response</span></span>

<span data-ttu-id="bb23d-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bb23d-134">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="bb23d-135">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bb23d-135">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bb23d-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb23d-136">All the properties will be returned from an actual call.</span></span>

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
