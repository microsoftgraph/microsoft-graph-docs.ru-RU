---
title: 'message: createReplyAll'
description: Создание черновика ответа отправителю и всем получателям указанного сообщения. После этого можно обновить черновик, чтобы добавить содержимое ответа в **текст** или изменить другие свойства сообщения, либо просто отправить черновик.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3fd133848bf90ab211a2edab3eb383ff0342de80
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049508"
---
# <a name="message-createreplyall"></a><span data-ttu-id="57a45-104">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="57a45-104">message: createReplyAll</span></span>

<span data-ttu-id="57a45-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57a45-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57a45-106">Создание черновика ответа отправителю и всем получателям указанного [сообщения](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="57a45-106">Create a draft to reply to the sender and all the recipients of the specified [message](../resources/message.md).</span></span> <span data-ttu-id="57a45-107">После этого можно [обновить](../api/message-update.md) черновик, чтобы добавить содержимое ответа в **текст** или изменить другие свойства сообщения, либо просто [отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="57a45-107">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="57a45-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57a45-108">Permissions</span></span>
<span data-ttu-id="57a45-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57a45-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57a45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57a45-111">Permission type</span></span>      | <span data-ttu-id="57a45-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57a45-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57a45-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57a45-113">Delegated (work or school account)</span></span> | <span data-ttu-id="57a45-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57a45-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="57a45-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57a45-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57a45-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57a45-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="57a45-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57a45-117">Application</span></span> | <span data-ttu-id="57a45-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57a45-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="57a45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57a45-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="57a45-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57a45-120">Request headers</span></span>
| <span data-ttu-id="57a45-121">Имя</span><span class="sxs-lookup"><span data-stu-id="57a45-121">Name</span></span>       | <span data-ttu-id="57a45-122">Тип</span><span class="sxs-lookup"><span data-stu-id="57a45-122">Type</span></span> | <span data-ttu-id="57a45-123">Описание</span><span class="sxs-lookup"><span data-stu-id="57a45-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="57a45-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="57a45-124">Authorization</span></span>  | <span data-ttu-id="57a45-125">string</span><span class="sxs-lookup"><span data-stu-id="57a45-125">string</span></span>  | <span data-ttu-id="57a45-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57a45-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57a45-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57a45-128">Request body</span></span>
<span data-ttu-id="57a45-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57a45-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57a45-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="57a45-130">Response</span></span>

<span data-ttu-id="57a45-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57a45-131">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57a45-132">Пример</span><span class="sxs-lookup"><span data-stu-id="57a45-132">Example</span></span>
<span data-ttu-id="57a45-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="57a45-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="57a45-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="57a45-134">Request</span></span>
<span data-ttu-id="57a45-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57a45-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57a45-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="57a45-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```
# <a name="c"></a>[<span data-ttu-id="57a45-137">C#</span><span class="sxs-lookup"><span data-stu-id="57a45-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57a45-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57a45-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57a45-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57a45-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57a45-140">Java</span><span class="sxs-lookup"><span data-stu-id="57a45-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="57a45-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="57a45-141">Response</span></span>
<span data-ttu-id="57a45-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57a45-142">Here is an example of the response.</span></span> <span data-ttu-id="57a45-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57a45-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

