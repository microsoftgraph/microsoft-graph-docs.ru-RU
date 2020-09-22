---
title: 'message: createReplyAll'
description: Создание черновика ответа отправителю и всем получателям указанного сообщения. После этого можно обновить черновик, чтобы добавить содержимое ответа в **текст** или изменить другие свойства сообщения, либо просто отправить черновик.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 14794102c04e18105557bccc8e285d0dd1990529
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094556"
---
# <a name="message-createreplyall"></a><span data-ttu-id="1d22f-104">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="1d22f-104">message: createReplyAll</span></span>

<span data-ttu-id="1d22f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d22f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d22f-106">Создание черновика ответа отправителю и всем получателям указанного [сообщения](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="1d22f-106">Create a draft to reply to the sender and all the recipients of the specified [message](../resources/message.md).</span></span> <span data-ttu-id="1d22f-107">После этого можно [обновить](../api/message-update.md) черновик, чтобы добавить содержимое ответа в **текст** или изменить другие свойства сообщения, либо просто [отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="1d22f-107">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d22f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d22f-108">Permissions</span></span>
<span data-ttu-id="1d22f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d22f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d22f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d22f-111">Permission type</span></span>      | <span data-ttu-id="1d22f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d22f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d22f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d22f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1d22f-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d22f-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1d22f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d22f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d22f-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d22f-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1d22f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d22f-117">Application</span></span> | <span data-ttu-id="1d22f-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d22f-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d22f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d22f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="1d22f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d22f-120">Request headers</span></span>
| <span data-ttu-id="1d22f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1d22f-121">Name</span></span>       | <span data-ttu-id="1d22f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1d22f-122">Type</span></span> | <span data-ttu-id="1d22f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1d22f-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d22f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d22f-124">Authorization</span></span>  | <span data-ttu-id="1d22f-125">string</span><span class="sxs-lookup"><span data-stu-id="1d22f-125">string</span></span>  | <span data-ttu-id="1d22f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d22f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d22f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d22f-128">Request body</span></span>
<span data-ttu-id="1d22f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d22f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d22f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d22f-130">Response</span></span>

<span data-ttu-id="1d22f-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d22f-131">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d22f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1d22f-132">Example</span></span>
<span data-ttu-id="1d22f-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1d22f-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1d22f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d22f-134">Request</span></span>
<span data-ttu-id="1d22f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d22f-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d22f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d22f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```
# <a name="c"></a>[<span data-ttu-id="1d22f-137">C#</span><span class="sxs-lookup"><span data-stu-id="1d22f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d22f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d22f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d22f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d22f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d22f-140">Java</span><span class="sxs-lookup"><span data-stu-id="1d22f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1d22f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d22f-141">Response</span></span>
<span data-ttu-id="1d22f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d22f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

