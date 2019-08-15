---
title: 'message: send'
description: Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 45d91623bf305bc5902b31cabea0625a81ea4ff9
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414975"
---
# <a name="message-send"></a><span data-ttu-id="d7534-104">message: send</span><span class="sxs-lookup"><span data-stu-id="d7534-104">message: send</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7534-p102">Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или пересылки. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="d7534-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7534-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7534-108">Permissions</span></span>

<span data-ttu-id="d7534-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7534-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7534-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7534-111">Permission type</span></span>      | <span data-ttu-id="d7534-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7534-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7534-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7534-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d7534-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d7534-114">Mail.Send</span></span>    |
|<span data-ttu-id="d7534-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7534-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7534-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d7534-116">Mail.Send</span></span>    |
|<span data-ttu-id="d7534-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7534-117">Application</span></span> | <span data-ttu-id="d7534-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d7534-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7534-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7534-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="d7534-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7534-120">Request headers</span></span>

| <span data-ttu-id="d7534-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d7534-121">Name</span></span>       | <span data-ttu-id="d7534-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d7534-122">Type</span></span> | <span data-ttu-id="d7534-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d7534-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d7534-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7534-124">Authorization</span></span>  | <span data-ttu-id="d7534-125">string</span><span class="sxs-lookup"><span data-stu-id="d7534-125">string</span></span>  | <span data-ttu-id="d7534-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7534-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7534-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="d7534-128">Content-Length</span></span> | <span data-ttu-id="d7534-129">число</span><span class="sxs-lookup"><span data-stu-id="d7534-129">number</span></span> | <span data-ttu-id="d7534-130">0. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7534-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7534-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7534-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d7534-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7534-132">Response</span></span>

<span data-ttu-id="d7534-p105">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d7534-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7534-135">Пример</span><span class="sxs-lookup"><span data-stu-id="d7534-135">Example</span></span>

<span data-ttu-id="d7534-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d7534-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7534-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7534-137">Request</span></span>

<span data-ttu-id="d7534-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7534-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d7534-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7534-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d7534-140">C#</span><span class="sxs-lookup"><span data-stu-id="d7534-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7534-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7534-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7534-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d7534-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d7534-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7534-143">Response</span></span>

<span data-ttu-id="d7534-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d7534-144">Here is an example of the response.</span></span>
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
