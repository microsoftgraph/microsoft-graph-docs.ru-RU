---
title: 'message: send'
description: Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f9a43439da379550ff65a1edd86e72cff7959ffe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448488"
---
# <a name="message-send"></a><span data-ttu-id="7729a-104">message: send</span><span class="sxs-lookup"><span data-stu-id="7729a-104">message: send</span></span>

<span data-ttu-id="7729a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7729a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7729a-p102">Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или пересылки. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="7729a-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="7729a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7729a-109">Permissions</span></span>

<span data-ttu-id="7729a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7729a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7729a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7729a-112">Permission type</span></span>      | <span data-ttu-id="7729a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7729a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7729a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7729a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7729a-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7729a-115">Mail.Send</span></span>    |
|<span data-ttu-id="7729a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7729a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7729a-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7729a-117">Mail.Send</span></span>    |
|<span data-ttu-id="7729a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7729a-118">Application</span></span> | <span data-ttu-id="7729a-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7729a-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="7729a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7729a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="7729a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7729a-121">Request headers</span></span>

| <span data-ttu-id="7729a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7729a-122">Name</span></span>       | <span data-ttu-id="7729a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7729a-123">Type</span></span> | <span data-ttu-id="7729a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7729a-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7729a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7729a-125">Authorization</span></span>  | <span data-ttu-id="7729a-126">string</span><span class="sxs-lookup"><span data-stu-id="7729a-126">string</span></span>  | <span data-ttu-id="7729a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7729a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7729a-129">Content-Length</span><span class="sxs-lookup"><span data-stu-id="7729a-129">Content-Length</span></span> | <span data-ttu-id="7729a-130">число</span><span class="sxs-lookup"><span data-stu-id="7729a-130">number</span></span> | <span data-ttu-id="7729a-131">0. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7729a-131">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7729a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7729a-132">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7729a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7729a-133">Response</span></span>

<span data-ttu-id="7729a-p105">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7729a-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7729a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="7729a-136">Example</span></span>

<span data-ttu-id="7729a-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7729a-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7729a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7729a-138">Request</span></span>

<span data-ttu-id="7729a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7729a-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7729a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="7729a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```
# <a name="c"></a>[<span data-ttu-id="7729a-141">C#</span><span class="sxs-lookup"><span data-stu-id="7729a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7729a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7729a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7729a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7729a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7729a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7729a-144">Response</span></span>

<span data-ttu-id="7729a-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7729a-145">Here is an example of the response.</span></span>
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
