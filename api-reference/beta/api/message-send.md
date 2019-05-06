---
title: 'message: send'
description: Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c4a4010a69f3c6323ab624d2b1fa1f16075a519b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597769"
---
# <a name="message-send"></a><span data-ttu-id="caf4f-104">message: send</span><span class="sxs-lookup"><span data-stu-id="caf4f-104">message: send</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caf4f-p102">Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или пересылки. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="caf4f-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="caf4f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="caf4f-108">Permissions</span></span>

<span data-ttu-id="caf4f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caf4f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caf4f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="caf4f-111">Permission type</span></span>      | <span data-ttu-id="caf4f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="caf4f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="caf4f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="caf4f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="caf4f-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="caf4f-114">Mail.Send</span></span>    |
|<span data-ttu-id="caf4f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="caf4f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caf4f-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="caf4f-116">Mail.Send</span></span>    |
|<span data-ttu-id="caf4f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="caf4f-117">Application</span></span> | <span data-ttu-id="caf4f-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="caf4f-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="caf4f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caf4f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="caf4f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="caf4f-120">Request headers</span></span>

| <span data-ttu-id="caf4f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="caf4f-121">Name</span></span>       | <span data-ttu-id="caf4f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="caf4f-122">Type</span></span> | <span data-ttu-id="caf4f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="caf4f-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="caf4f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="caf4f-124">Authorization</span></span>  | <span data-ttu-id="caf4f-125">string</span><span class="sxs-lookup"><span data-stu-id="caf4f-125">string</span></span>  | <span data-ttu-id="caf4f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caf4f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="caf4f-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="caf4f-128">Content-Length</span></span> | <span data-ttu-id="caf4f-129">число</span><span class="sxs-lookup"><span data-stu-id="caf4f-129">number</span></span> | <span data-ttu-id="caf4f-130">0. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caf4f-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="caf4f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="caf4f-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="caf4f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="caf4f-132">Response</span></span>

<span data-ttu-id="caf4f-p105">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="caf4f-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caf4f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="caf4f-135">Example</span></span>

<span data-ttu-id="caf4f-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="caf4f-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="caf4f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="caf4f-137">Request</span></span>

<span data-ttu-id="caf4f-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caf4f-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="caf4f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="caf4f-139">Response</span></span>

<span data-ttu-id="caf4f-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="caf4f-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="caf4f-141">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="caf4f-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="caf4f-142">Языках</span><span class="sxs-lookup"><span data-stu-id="caf4f-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_send-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="caf4f-143">Язык</span><span class="sxs-lookup"><span data-stu-id="caf4f-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_send-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/message-send.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-send.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
