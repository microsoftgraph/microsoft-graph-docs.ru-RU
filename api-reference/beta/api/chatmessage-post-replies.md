---
title: Создание ответа chatMessage в канале
description: Создает новый объект chatMessage в ответе на существующий объект chatMessage.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 76063d5a54c778882bce0024ba35dc3831c93876
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863526"
---
# <a name="create-chatmessage-reply-in-a-channel"></a><span data-ttu-id="36fce-103">Создание ответа chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="36fce-103">Create chatMessage reply in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36fce-104">Создает новый объект [chatMessage](../resources/chatmessage.md) в ответе на существующий объект [chatMessage](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="36fce-104">Creates a new [chatMessage](../resources/chatmessage.md) object in reply to an existing [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="36fce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36fce-105">Permissions</span></span>

<span data-ttu-id="36fce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36fce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36fce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36fce-108">Permission type</span></span>                        | <span data-ttu-id="36fce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36fce-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="36fce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36fce-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="36fce-111">Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36fce-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="36fce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36fce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36fce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36fce-113">Not supported.</span></span> |
| <span data-ttu-id="36fce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36fce-114">Application</span></span>                            | <span data-ttu-id="36fce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36fce-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36fce-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36fce-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages/{id}/replies
POST /users/{id}/chats/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="36fce-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36fce-117">Request headers</span></span>

| <span data-ttu-id="36fce-118">Имя</span><span class="sxs-lookup"><span data-stu-id="36fce-118">Name</span></span>          | <span data-ttu-id="36fce-119">Описание</span><span class="sxs-lookup"><span data-stu-id="36fce-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="36fce-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36fce-120">Authorization</span></span> | <span data-ttu-id="36fce-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="36fce-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="36fce-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36fce-122">Request body</span></span>

<span data-ttu-id="36fce-123">В тексте запроса добавьте представление объекта [chatMessage](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36fce-123">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="36fce-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="36fce-124">Response</span></span>

<span data-ttu-id="36fce-125">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36fce-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36fce-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="36fce-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36fce-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="36fce-127">Request</span></span>

<span data-ttu-id="36fce-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36fce-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36fce-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="36fce-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="36fce-130">C#</span><span class="sxs-lookup"><span data-stu-id="36fce-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chatmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36fce-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="36fce-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chatmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36fce-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="36fce-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chatmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="36fce-133">Java</span><span class="sxs-lookup"><span data-stu-id="36fce-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-chatmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="36fce-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="36fce-134">Response</span></span>

<span data-ttu-id="36fce-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="36fce-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="36fce-136">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="36fce-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="36fce-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36fce-137">All the properties will be returned from an actual call.</span></span>

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
