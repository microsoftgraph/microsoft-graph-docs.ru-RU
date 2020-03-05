---
title: Создание ответа на chatMessage в канале
description: Создает новый объект chatMessage в ответе на существующий объект chatMessage.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 00d1f9d6d2197f1e265c59a795ef66941c0a5c60
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438304"
---
# <a name="create-chatmessage-reply-in-a-channel"></a><span data-ttu-id="2ef38-103">Создание ответа на chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="2ef38-103">Create chatMessage reply in a channel</span></span>

<span data-ttu-id="2ef38-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2ef38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef38-105">Создает новый объект [chatMessage](../resources/chatmessage.md) в ответе на существующий объект [chatMessage](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="2ef38-105">Creates a new [chatMessage](../resources/chatmessage.md) object in reply to an existing [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ef38-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef38-106">Permissions</span></span>

<span data-ttu-id="2ef38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ef38-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef38-109">Permission type</span></span>                        | <span data-ttu-id="2ef38-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ef38-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ef38-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ef38-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ef38-112">Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ef38-112">Chat.ReadWrite</span></span> |
| <span data-ttu-id="2ef38-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ef38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef38-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ef38-114">Not supported.</span></span> |
| <span data-ttu-id="2ef38-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ef38-115">Application</span></span>                            | <span data-ttu-id="2ef38-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ef38-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ef38-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ef38-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="2ef38-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ef38-118">Request headers</span></span>

| <span data-ttu-id="2ef38-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2ef38-119">Name</span></span>          | <span data-ttu-id="2ef38-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2ef38-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2ef38-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ef38-121">Authorization</span></span> | <span data-ttu-id="2ef38-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2ef38-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ef38-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ef38-123">Request body</span></span>

<span data-ttu-id="2ef38-124">В тексте запроса добавьте представление объекта [chatMessage](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ef38-124">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2ef38-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef38-125">Response</span></span>

<span data-ttu-id="2ef38-126">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ef38-126">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ef38-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ef38-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ef38-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ef38-128">Request</span></span>

<span data-ttu-id="2ef38-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ef38-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ef38-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef38-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chatmessage"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
     "content" : "Hello world"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="2ef38-131">C#</span><span class="sxs-lookup"><span data-stu-id="2ef38-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chatmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef38-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef38-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chatmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef38-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef38-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chatmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ef38-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef38-134">Response</span></span>

<span data-ttu-id="2ef38-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2ef38-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="2ef38-136">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ef38-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2ef38-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ef38-137">All the properties will be returned from an actual call.</span></span>

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
