---
title: 'message: send'
description: Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 60441163dacebe8ca5b15e0571100c4b87f50ef7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976489"
---
# <a name="message-send"></a><span data-ttu-id="55677-104">message: send</span><span class="sxs-lookup"><span data-stu-id="55677-104">message: send</span></span>

<span data-ttu-id="55677-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55677-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55677-p102">Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или пересылки. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="55677-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="55677-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55677-109">Permissions</span></span>

<span data-ttu-id="55677-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55677-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55677-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55677-112">Permission type</span></span>      | <span data-ttu-id="55677-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55677-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55677-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55677-114">Delegated (work or school account)</span></span> | <span data-ttu-id="55677-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="55677-115">Mail.Send</span></span>    |
|<span data-ttu-id="55677-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55677-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55677-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="55677-117">Mail.Send</span></span>    |
|<span data-ttu-id="55677-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55677-118">Application</span></span> | <span data-ttu-id="55677-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="55677-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="55677-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55677-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="55677-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55677-121">Request headers</span></span>

| <span data-ttu-id="55677-122">Имя</span><span class="sxs-lookup"><span data-stu-id="55677-122">Name</span></span>       | <span data-ttu-id="55677-123">Тип</span><span class="sxs-lookup"><span data-stu-id="55677-123">Type</span></span> | <span data-ttu-id="55677-124">Описание</span><span class="sxs-lookup"><span data-stu-id="55677-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55677-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="55677-125">Authorization</span></span>  | <span data-ttu-id="55677-126">string</span><span class="sxs-lookup"><span data-stu-id="55677-126">string</span></span>  | <span data-ttu-id="55677-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55677-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="55677-129">Content-Length</span><span class="sxs-lookup"><span data-stu-id="55677-129">Content-Length</span></span> | <span data-ttu-id="55677-130">число</span><span class="sxs-lookup"><span data-stu-id="55677-130">number</span></span> | <span data-ttu-id="55677-131">0. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55677-131">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55677-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55677-132">Request body</span></span>

## <a name="response"></a><span data-ttu-id="55677-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="55677-133">Response</span></span>

<span data-ttu-id="55677-p105">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="55677-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55677-136">Пример</span><span class="sxs-lookup"><span data-stu-id="55677-136">Example</span></span>

<span data-ttu-id="55677-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="55677-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="55677-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="55677-138">Request</span></span>

<span data-ttu-id="55677-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55677-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55677-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="55677-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```
# <a name="c"></a>[<span data-ttu-id="55677-141">C#</span><span class="sxs-lookup"><span data-stu-id="55677-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55677-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55677-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55677-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55677-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55677-144">Java</span><span class="sxs-lookup"><span data-stu-id="55677-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="55677-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="55677-145">Response</span></span>

<span data-ttu-id="55677-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55677-146">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


