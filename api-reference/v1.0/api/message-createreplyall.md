---
title: 'message: createReplyAll'
description: Создание черновика ответа отправителю и всем получателям указанного сообщения. После этого можно обновить черновик, чтобы добавить содержимое ответа в **текст** или изменить другие свойства сообщения, либо просто отправить черновик.
ms.openlocfilehash: a48e5bf7f3ae330ff31a2b8d2827259798186c64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028290"
---
# <a name="message-createreplyall"></a><span data-ttu-id="cb4af-104">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="cb4af-104">message: createReplyAll</span></span>

<span data-ttu-id="cb4af-105">Создание черновика ответа отправителю и всем получателям указанного [сообщения](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="cb4af-105">Create a draft to reply to the sender and all the recipients of the specified [message](../resources/message.md).</span></span> <span data-ttu-id="cb4af-106">После этого можно [обновить](../api/message-update.md) черновик, чтобы добавить содержимое ответа в **текст** или изменить другие свойства сообщения, либо просто [отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="cb4af-106">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb4af-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb4af-107">Permissions</span></span>
<span data-ttu-id="cb4af-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb4af-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb4af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb4af-110">Permission type</span></span>      | <span data-ttu-id="cb4af-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb4af-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb4af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb4af-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cb4af-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb4af-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cb4af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb4af-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb4af-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb4af-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cb4af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb4af-116">Application</span></span> | <span data-ttu-id="cb4af-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb4af-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb4af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb4af-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="cb4af-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb4af-119">Request headers</span></span>
| <span data-ttu-id="cb4af-120">Имя</span><span class="sxs-lookup"><span data-stu-id="cb4af-120">Name</span></span>       | <span data-ttu-id="cb4af-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cb4af-121">Type</span></span> | <span data-ttu-id="cb4af-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cb4af-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cb4af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb4af-123">Authorization</span></span>  | <span data-ttu-id="cb4af-124">string</span><span class="sxs-lookup"><span data-stu-id="cb4af-124">string</span></span>  | <span data-ttu-id="cb4af-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb4af-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb4af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb4af-127">Request body</span></span>
<span data-ttu-id="cb4af-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb4af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb4af-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb4af-129">Response</span></span>

<span data-ttu-id="cb4af-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb4af-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb4af-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cb4af-131">Example</span></span>
<span data-ttu-id="cb4af-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cb4af-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cb4af-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb4af-133">Request</span></span>
<span data-ttu-id="cb4af-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb4af-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```

##### <a name="response"></a><span data-ttu-id="cb4af-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb4af-135">Response</span></span>
<span data-ttu-id="cb4af-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cb4af-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
