---
title: 'message: createReply'
description: Создание черновика ответа на указанное сообщение. После этого можно обновить черновик, чтобы добавить содержимое ответа в **текст** или изменить другие свойства сообщения, либо просто отправить черновик.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9b45669b14bbeb0977e1437eb611074857193d04
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444178"
---
# <a name="message-createreply"></a><span data-ttu-id="9ad5b-104">message: createReply</span><span class="sxs-lookup"><span data-stu-id="9ad5b-104">message: createReply</span></span>

<span data-ttu-id="9ad5b-105">Создание черновика ответа на указанное [сообщение](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="9ad5b-105">Create a draft of the reply to the specified [message](../resources/message.md).</span></span> <span data-ttu-id="9ad5b-106">После этого можно [обновить](../api/message-update.md) черновик, чтобы добавить содержимое ответа в **текст** или изменить другие свойства сообщения, либо просто [отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="9ad5b-106">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ad5b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ad5b-107">Permissions</span></span>
<span data-ttu-id="9ad5b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ad5b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ad5b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ad5b-110">Permission type</span></span>      | <span data-ttu-id="9ad5b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ad5b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ad5b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ad5b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9ad5b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ad5b-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9ad5b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ad5b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ad5b-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ad5b-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9ad5b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ad5b-116">Application</span></span> | <span data-ttu-id="9ad5b-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ad5b-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ad5b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ad5b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="9ad5b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ad5b-119">Request headers</span></span>
| <span data-ttu-id="9ad5b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9ad5b-120">Name</span></span>       | <span data-ttu-id="9ad5b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9ad5b-121">Type</span></span> | <span data-ttu-id="9ad5b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9ad5b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9ad5b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ad5b-123">Authorization</span></span>  | <span data-ttu-id="9ad5b-124">string</span><span class="sxs-lookup"><span data-stu-id="9ad5b-124">string</span></span>  | <span data-ttu-id="9ad5b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ad5b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ad5b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9ad5b-127">Request body</span></span>
<span data-ttu-id="9ad5b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ad5b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ad5b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ad5b-129">Response</span></span>

<span data-ttu-id="9ad5b-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ad5b-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ad5b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9ad5b-131">Example</span></span>
<span data-ttu-id="9ad5b-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9ad5b-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9ad5b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ad5b-133">Request</span></span>
<span data-ttu-id="9ad5b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ad5b-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ad5b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ad5b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReply
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ad5b-136">C#</span><span class="sxs-lookup"><span data-stu-id="9ad5b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ad5b-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="9ad5b-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ad5b-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9ad5b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9ad5b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ad5b-139">Response</span></span>
<span data-ttu-id="9ad5b-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ad5b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
