---
title: 'message: send'
description: Отправка существующего черновика сообщения.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ea24ae69c3888e31124df758bc22199bde1048ea
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645523"
---
# <a name="message-send"></a><span data-ttu-id="e1a41-103">message: send</span><span class="sxs-lookup"><span data-stu-id="e1a41-103">message: send</span></span>

<span data-ttu-id="e1a41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1a41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1a41-105">Отправка существующего черновика сообщения.</span><span class="sxs-lookup"><span data-stu-id="e1a41-105">Send an existing draft message.</span></span> 

<span data-ttu-id="e1a41-106">Черновик сообщения может быть новым черновиком [сообщения,](../api/user-post-messages.md)черновиком [ответа,](../api/message-createreply.md) [черновиком](../api/message-createreplyall.md)для всех ответов или [проектом вперед.](../api/message-createforward.md)</span><span class="sxs-lookup"><span data-stu-id="e1a41-106">The draft message can be a new message [draft](../api/user-post-messages.md), [reply draft](../api/message-createreply.md), [reply-all draft](../api/message-createreplyall.md), or a [forward draft](../api/message-createforward.md).</span></span> 

<span data-ttu-id="e1a41-107">Этот метод сохраняет сообщение в папке **Отправленные** элементы.</span><span class="sxs-lookup"><span data-stu-id="e1a41-107">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="e1a41-108">Кроме того, [отправьте новое сообщение](../api/user-sendmail.md) в одной операции.</span><span class="sxs-lookup"><span data-stu-id="e1a41-108">Alternatively, [send a new message](../api/user-sendmail.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1a41-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1a41-109">Permissions</span></span>
<span data-ttu-id="e1a41-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="e1a41-110">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="e1a41-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1a41-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1a41-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1a41-112">Permission type</span></span>      | <span data-ttu-id="e1a41-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1a41-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1a41-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1a41-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e1a41-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e1a41-115">Mail.Send</span></span>    |
|<span data-ttu-id="e1a41-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1a41-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1a41-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e1a41-117">Mail.Send</span></span>    |
|<span data-ttu-id="e1a41-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1a41-118">Application</span></span> | <span data-ttu-id="e1a41-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e1a41-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1a41-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1a41-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="e1a41-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1a41-121">Request headers</span></span>

| <span data-ttu-id="e1a41-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e1a41-122">Name</span></span>       | <span data-ttu-id="e1a41-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e1a41-123">Type</span></span> | <span data-ttu-id="e1a41-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e1a41-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e1a41-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1a41-125">Authorization</span></span>  | <span data-ttu-id="e1a41-126">string</span><span class="sxs-lookup"><span data-stu-id="e1a41-126">string</span></span>  | <span data-ttu-id="e1a41-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1a41-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1a41-129">Content-Length</span><span class="sxs-lookup"><span data-stu-id="e1a41-129">Content-Length</span></span> | <span data-ttu-id="e1a41-130">число</span><span class="sxs-lookup"><span data-stu-id="e1a41-130">number</span></span> | <span data-ttu-id="e1a41-131">0. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1a41-131">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1a41-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1a41-132">Request body</span></span>
<span data-ttu-id="e1a41-133">Так как этот метод отправляет уже существующее черновик сообщения, указывать текст запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="e1a41-133">Since this method sends an already existing draft message, specifying a request body is not necessary.</span></span>

## <a name="response"></a><span data-ttu-id="e1a41-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1a41-134">Response</span></span>

<span data-ttu-id="e1a41-p103">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e1a41-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1a41-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="e1a41-137">Examples</span></span>
### <a name="example-1-send-an-existing-draft-message"></a><span data-ttu-id="e1a41-138">Пример 1. Отправка существующего черновика сообщения</span><span class="sxs-lookup"><span data-stu-id="e1a41-138">Example 1: Send an existing draft message</span></span>

<span data-ttu-id="e1a41-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e1a41-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e1a41-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1a41-140">Request</span></span>

<span data-ttu-id="e1a41-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1a41-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1a41-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1a41-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```
# <a name="c"></a>[<span data-ttu-id="e1a41-143">C#</span><span class="sxs-lookup"><span data-stu-id="e1a41-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1a41-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1a41-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1a41-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1a41-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1a41-146">Java</span><span class="sxs-lookup"><span data-stu-id="e1a41-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e1a41-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1a41-147">Response</span></span>

<span data-ttu-id="e1a41-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1a41-148">Here is an example of the response.</span></span>

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
