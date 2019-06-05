---
title: Создание chatMessage
description: Используйте этот API для создания нового chatMessage.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 22ee0d1e4b2822f26a4892fb354bdc8c90663d21
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720959"
---
# <a name="create-chatmessage"></a><span data-ttu-id="a55c2-103">Создание chatMessage</span><span class="sxs-lookup"><span data-stu-id="a55c2-103">Create chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a55c2-104">Создайте новое [сообщение](../resources/chatmessage.md) в указанном [сеансе чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="a55c2-104">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a55c2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a55c2-105">Permissions</span></span>

<span data-ttu-id="a55c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a55c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a55c2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a55c2-108">Permission type</span></span>                        | <span data-ttu-id="a55c2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a55c2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a55c2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a55c2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a55c2-111">Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a55c2-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="a55c2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a55c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a55c2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a55c2-113">Not supported.</span></span> |
| <span data-ttu-id="a55c2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a55c2-114">Application</span></span>                            | <span data-ttu-id="a55c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a55c2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a55c2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a55c2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="a55c2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a55c2-117">Request headers</span></span>

| <span data-ttu-id="a55c2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a55c2-118">Name</span></span>          | <span data-ttu-id="a55c2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a55c2-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a55c2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a55c2-120">Authorization</span></span> | <span data-ttu-id="a55c2-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a55c2-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a55c2-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a55c2-122">Request body</span></span>

<span data-ttu-id="a55c2-123">В тексте запроса добавьте представление объекта [chatMessage](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a55c2-123">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a55c2-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="a55c2-124">Response</span></span>

<span data-ttu-id="a55c2-125">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a55c2-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a55c2-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="a55c2-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a55c2-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="a55c2-127">Request</span></span>

<span data-ttu-id="a55c2-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a55c2-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a55c2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a55c2-129">Response</span></span>

<span data-ttu-id="a55c2-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a55c2-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a55c2-131">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a55c2-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a55c2-132">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a55c2-132">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->