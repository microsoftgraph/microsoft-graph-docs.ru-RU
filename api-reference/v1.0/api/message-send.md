---
title: 'message: send'
description: Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 3f9740f74238012571abcfa7f406fd12ed58c9e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463595"
---
# <a name="message-send"></a><span data-ttu-id="bf0c1-104">message: send</span><span class="sxs-lookup"><span data-stu-id="bf0c1-104">message: send</span></span>

<span data-ttu-id="bf0c1-p102">Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или пересылки. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="bf0c1-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf0c1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf0c1-108">Permissions</span></span>

<span data-ttu-id="bf0c1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf0c1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf0c1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf0c1-111">Permission type</span></span>      | <span data-ttu-id="bf0c1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf0c1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf0c1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf0c1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bf0c1-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="bf0c1-114">Mail.Send</span></span>    |
|<span data-ttu-id="bf0c1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf0c1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf0c1-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="bf0c1-116">Mail.Send</span></span>    |
|<span data-ttu-id="bf0c1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf0c1-117">Application</span></span> | <span data-ttu-id="bf0c1-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="bf0c1-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf0c1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf0c1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="bf0c1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf0c1-120">Request headers</span></span>

| <span data-ttu-id="bf0c1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bf0c1-121">Name</span></span>       | <span data-ttu-id="bf0c1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="bf0c1-122">Type</span></span> | <span data-ttu-id="bf0c1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bf0c1-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bf0c1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf0c1-124">Authorization</span></span>  | <span data-ttu-id="bf0c1-125">string</span><span class="sxs-lookup"><span data-stu-id="bf0c1-125">string</span></span>  | <span data-ttu-id="bf0c1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf0c1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf0c1-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="bf0c1-128">Content-Length</span></span> | <span data-ttu-id="bf0c1-129">число</span><span class="sxs-lookup"><span data-stu-id="bf0c1-129">number</span></span> | <span data-ttu-id="bf0c1-130">0. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf0c1-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf0c1-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf0c1-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bf0c1-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf0c1-132">Response</span></span>

<span data-ttu-id="bf0c1-p105">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bf0c1-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf0c1-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bf0c1-135">Example</span></span>

<span data-ttu-id="bf0c1-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="bf0c1-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="bf0c1-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf0c1-137">Request</span></span>

<span data-ttu-id="bf0c1-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf0c1-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="bf0c1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf0c1-139">Response</span></span>

<span data-ttu-id="bf0c1-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bf0c1-140">Here is an example of the response.</span></span>
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
