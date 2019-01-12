---
title: 'message: send'
description: Отправьте сообщение в папке «Черновики». Черновик сообщения могут быть новый черновик сообщения, ответ черновиков, ответить всем черновиков или
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 937c2da1bab83c412097f4207f32d07dc98d2ff8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940675"
---
# <a name="message-send"></a><span data-ttu-id="579bd-104">message: send</span><span class="sxs-lookup"><span data-stu-id="579bd-104">message: send</span></span>

> <span data-ttu-id="579bd-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="579bd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="579bd-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="579bd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="579bd-p103">Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или пересылки. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="579bd-p103">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="579bd-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="579bd-110">Permissions</span></span>

<span data-ttu-id="579bd-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="579bd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="579bd-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="579bd-113">Permission type</span></span>      | <span data-ttu-id="579bd-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="579bd-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="579bd-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="579bd-115">Delegated (work or school account)</span></span> | <span data-ttu-id="579bd-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="579bd-116">Mail.Send</span></span>    |
|<span data-ttu-id="579bd-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="579bd-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="579bd-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="579bd-118">Mail.Send</span></span>    |
|<span data-ttu-id="579bd-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="579bd-119">Application</span></span> | <span data-ttu-id="579bd-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="579bd-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="579bd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="579bd-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="579bd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="579bd-122">Request headers</span></span>

| <span data-ttu-id="579bd-123">Имя</span><span class="sxs-lookup"><span data-stu-id="579bd-123">Name</span></span>       | <span data-ttu-id="579bd-124">Тип</span><span class="sxs-lookup"><span data-stu-id="579bd-124">Type</span></span> | <span data-ttu-id="579bd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="579bd-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="579bd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="579bd-126">Authorization</span></span>  | <span data-ttu-id="579bd-127">string</span><span class="sxs-lookup"><span data-stu-id="579bd-127">string</span></span>  | <span data-ttu-id="579bd-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="579bd-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="579bd-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="579bd-130">Content-Length</span></span> | <span data-ttu-id="579bd-131">число</span><span class="sxs-lookup"><span data-stu-id="579bd-131">number</span></span> | <span data-ttu-id="579bd-132">0. требуется.</span><span class="sxs-lookup"><span data-stu-id="579bd-132">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="579bd-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="579bd-133">Request body</span></span>

## <a name="response"></a><span data-ttu-id="579bd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="579bd-134">Response</span></span>

<span data-ttu-id="579bd-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="579bd-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="579bd-137">Пример</span><span class="sxs-lookup"><span data-stu-id="579bd-137">Example</span></span>

<span data-ttu-id="579bd-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="579bd-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="579bd-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="579bd-139">Request</span></span>

<span data-ttu-id="579bd-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="579bd-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="579bd-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="579bd-141">Response</span></span>

<span data-ttu-id="579bd-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="579bd-142">Here is an example of the response.</span></span>
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
