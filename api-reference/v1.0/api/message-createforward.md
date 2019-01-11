---
title: 'message: createForward'
description: Создание черновика для пересылки указанного ресурса message. После этого можно обновить черновик, чтобы добавить содержимое в **текст** или изменить другие свойства сообщения, либо просто отправить черновик.
localization_priority: Normal
ms.openlocfilehash: 230fdfd4a1700e5bcbe2e1cb364de08d86c7be39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888265"
---
# <a name="message-createforward"></a><span data-ttu-id="7f525-104">message: createForward</span><span class="sxs-lookup"><span data-stu-id="7f525-104">message: createForward</span></span>

<span data-ttu-id="7f525-105">Создание черновика для пересылки указанного ресурса [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="7f525-105">Create a draft to forward the specified [message](../resources/message.md).</span></span> <span data-ttu-id="7f525-106">После этого можно [обновить](../api/message-update.md) черновик, чтобы добавить содержимое в **текст** или изменить другие свойства сообщения, либо просто [отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="7f525-106">You can then [update](../api/message-update.md) the draft to add content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f525-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f525-107">Permissions</span></span>

<span data-ttu-id="7f525-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f525-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f525-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f525-110">Permission type</span></span>      | <span data-ttu-id="7f525-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f525-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f525-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f525-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f525-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f525-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7f525-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f525-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f525-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f525-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7f525-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f525-116">Application</span></span> | <span data-ttu-id="7f525-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f525-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f525-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f525-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```

## <a name="request-headers"></a><span data-ttu-id="7f525-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f525-119">Request headers</span></span>

| <span data-ttu-id="7f525-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7f525-120">Name</span></span>       | <span data-ttu-id="7f525-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7f525-121">Type</span></span> | <span data-ttu-id="7f525-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7f525-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7f525-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f525-123">Authorization</span></span>  | <span data-ttu-id="7f525-124">string</span><span class="sxs-lookup"><span data-stu-id="7f525-124">string</span></span>  | <span data-ttu-id="7f525-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f525-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f525-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f525-127">Request body</span></span>

<span data-ttu-id="7f525-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f525-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f525-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f525-129">Response</span></span>

<span data-ttu-id="7f525-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f525-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f525-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7f525-131">Example</span></span>

<span data-ttu-id="7f525-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7f525-132">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7f525-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f525-133">Request</span></span>

<span data-ttu-id="7f525-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f525-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
```

##### <a name="response"></a><span data-ttu-id="7f525-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f525-135">Response</span></span>

<span data-ttu-id="7f525-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7f525-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
