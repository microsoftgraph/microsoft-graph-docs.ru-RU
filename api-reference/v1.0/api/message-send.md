---
title: 'message: send'
description: Отправка существующего черновика сообщения.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8be54552df8acf7faa67c070e85f63f48a5c23d4
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645495"
---
# <a name="message-send"></a><span data-ttu-id="e16f9-103">message: send</span><span class="sxs-lookup"><span data-stu-id="e16f9-103">message: send</span></span>

<span data-ttu-id="e16f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e16f9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e16f9-105">Отправка существующего черновика сообщения.</span><span class="sxs-lookup"><span data-stu-id="e16f9-105">Send an existing draft message.</span></span> 

<span data-ttu-id="e16f9-106">Черновик сообщения может быть предназначен для [нового сообщения](../api/user-post-messages.md), [ответа](../api/message-createreply.md), [ответа всем пользователям](../api/message-createreplyall.md) или [пересылки](../api/message-createforward.md).</span><span class="sxs-lookup"><span data-stu-id="e16f9-106">The draft message can be a new message [draft](../api/user-post-messages.md), [reply draft](../api/message-createreply.md), [reply-all draft](../api/message-createreplyall.md), or a [forward draft](../api/message-createforward.md).</span></span>

<span data-ttu-id="e16f9-107">Этот метод сохраняет сообщение в папке **Отправленные**.</span><span class="sxs-lookup"><span data-stu-id="e16f9-107">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="e16f9-108">Другой способ — [отправка нового сообщения](../api/user-sendmail.md) за один шаг.</span><span class="sxs-lookup"><span data-stu-id="e16f9-108">Alternatively, [send a new message](../api/user-sendmail.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="e16f9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e16f9-109">Permissions</span></span>
<span data-ttu-id="e16f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e16f9-p101">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e16f9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e16f9-112">Permission type</span></span>      | <span data-ttu-id="e16f9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e16f9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e16f9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e16f9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e16f9-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e16f9-115">Mail.Send</span></span>    |
|<span data-ttu-id="e16f9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e16f9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e16f9-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e16f9-117">Mail.Send</span></span>    |
|<span data-ttu-id="e16f9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e16f9-118">Application</span></span> | <span data-ttu-id="e16f9-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e16f9-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="e16f9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e16f9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="e16f9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e16f9-121">Request headers</span></span>

| <span data-ttu-id="e16f9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e16f9-122">Name</span></span>       | <span data-ttu-id="e16f9-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e16f9-123">Type</span></span> | <span data-ttu-id="e16f9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e16f9-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e16f9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e16f9-125">Authorization</span></span>  | <span data-ttu-id="e16f9-126">string</span><span class="sxs-lookup"><span data-stu-id="e16f9-126">string</span></span>  | <span data-ttu-id="e16f9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e16f9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e16f9-129">Content-Length</span><span class="sxs-lookup"><span data-stu-id="e16f9-129">Content-Length</span></span> | <span data-ttu-id="e16f9-130">число</span><span class="sxs-lookup"><span data-stu-id="e16f9-130">number</span></span> | <span data-ttu-id="e16f9-131">0. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e16f9-131">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e16f9-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e16f9-132">Request body</span></span>
<span data-ttu-id="e16f9-133">Так как этот метод отправляет уже существующий черновик сообщения, указывать тело запроса необязательно.</span><span class="sxs-lookup"><span data-stu-id="e16f9-133">Since this method sends an already existing draft message, specifying a request body is not necessary.</span></span>

## <a name="response"></a><span data-ttu-id="e16f9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e16f9-134">Response</span></span>

<span data-ttu-id="e16f9-p103">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e16f9-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e16f9-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="e16f9-137">Examples</span></span>

### <a name="example-1-send-an-existing-draft-message"></a><span data-ttu-id="e16f9-138">Пример 1. Отправка существующего черновика сообщения</span><span class="sxs-lookup"><span data-stu-id="e16f9-138">Example 1: Send an existing draft message</span></span>

<span data-ttu-id="e16f9-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e16f9-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e16f9-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e16f9-140">Request</span></span>

<span data-ttu-id="e16f9-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e16f9-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e16f9-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e16f9-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```
# <a name="c"></a>[<span data-ttu-id="e16f9-143">C#</span><span class="sxs-lookup"><span data-stu-id="e16f9-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e16f9-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e16f9-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e16f9-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e16f9-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e16f9-146">Java</span><span class="sxs-lookup"><span data-stu-id="e16f9-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e16f9-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e16f9-147">Response</span></span>

<span data-ttu-id="e16f9-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e16f9-148">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

