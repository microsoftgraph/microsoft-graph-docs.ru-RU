---
title: 'message: send'
description: Отправьте сообщение в папке «Черновики». Черновик сообщения могут быть новый черновик сообщения, ответ черновиков, ответить всем черновиков или
ms.openlocfilehash: 8fe04db6a7fe4a469374cd54a00f308e01341274
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028021"
---
# <a name="message-send"></a><span data-ttu-id="12db7-104">message: send</span><span class="sxs-lookup"><span data-stu-id="12db7-104">message: send</span></span>

<span data-ttu-id="12db7-p102">Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или пересылки. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="12db7-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="12db7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12db7-108">Permissions</span></span>

<span data-ttu-id="12db7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12db7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12db7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12db7-111">Permission type</span></span>      | <span data-ttu-id="12db7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12db7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12db7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12db7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="12db7-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="12db7-114">Mail.Send</span></span>    |
|<span data-ttu-id="12db7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12db7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12db7-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="12db7-116">Mail.Send</span></span>    |
|<span data-ttu-id="12db7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12db7-117">Application</span></span> | <span data-ttu-id="12db7-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="12db7-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="12db7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12db7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="12db7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12db7-120">Request headers</span></span>

| <span data-ttu-id="12db7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="12db7-121">Name</span></span>       | <span data-ttu-id="12db7-122">Тип</span><span class="sxs-lookup"><span data-stu-id="12db7-122">Type</span></span> | <span data-ttu-id="12db7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="12db7-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12db7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="12db7-124">Authorization</span></span>  | <span data-ttu-id="12db7-125">string</span><span class="sxs-lookup"><span data-stu-id="12db7-125">string</span></span>  | <span data-ttu-id="12db7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12db7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12db7-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="12db7-128">Content-Length</span></span> | <span data-ttu-id="12db7-129">number</span><span class="sxs-lookup"><span data-stu-id="12db7-129">number</span></span> | <span data-ttu-id="12db7-130">0. требуется.</span><span class="sxs-lookup"><span data-stu-id="12db7-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12db7-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12db7-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="12db7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="12db7-132">Response</span></span>

<span data-ttu-id="12db7-p105">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="12db7-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12db7-135">Пример</span><span class="sxs-lookup"><span data-stu-id="12db7-135">Example</span></span>

<span data-ttu-id="12db7-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="12db7-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="12db7-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="12db7-137">Request</span></span>

<span data-ttu-id="12db7-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12db7-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="12db7-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="12db7-139">Response</span></span>

<span data-ttu-id="12db7-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="12db7-140">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
