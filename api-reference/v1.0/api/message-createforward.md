---
title: 'message: createForward'
description: Создание черновика для пересылки указанного ресурса message. После этого можно обновить черновик, чтобы добавить содержимое в **текст** или изменить другие свойства сообщения, либо просто отправить черновик.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 484eb33c3cfe7dc9c1dc3ec896e45cff9ecce61d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565557"
---
# <a name="message-createforward"></a><span data-ttu-id="1e553-104">message: createForward</span><span class="sxs-lookup"><span data-stu-id="1e553-104">message: createForward</span></span>

<span data-ttu-id="1e553-105">Создание черновика для пересылки указанного ресурса [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="1e553-105">Create a draft to forward the specified [message](../resources/message.md).</span></span> <span data-ttu-id="1e553-106">После этого можно [обновить](../api/message-update.md) черновик, чтобы добавить содержимое в **текст** или изменить другие свойства сообщения, либо просто [отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="1e553-106">You can then [update](../api/message-update.md) the draft to add content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e553-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e553-107">Permissions</span></span>

<span data-ttu-id="1e553-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e553-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e553-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e553-110">Permission type</span></span>      | <span data-ttu-id="1e553-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e553-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e553-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e553-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e553-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e553-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1e553-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e553-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e553-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e553-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1e553-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e553-116">Application</span></span> | <span data-ttu-id="1e553-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e553-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e553-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e553-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```

## <a name="request-headers"></a><span data-ttu-id="1e553-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e553-119">Request headers</span></span>

| <span data-ttu-id="1e553-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1e553-120">Name</span></span>       | <span data-ttu-id="1e553-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1e553-121">Type</span></span> | <span data-ttu-id="1e553-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1e553-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1e553-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e553-123">Authorization</span></span>  | <span data-ttu-id="1e553-124">string</span><span class="sxs-lookup"><span data-stu-id="1e553-124">string</span></span>  | <span data-ttu-id="1e553-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e553-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e553-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e553-127">Request body</span></span>

<span data-ttu-id="1e553-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1e553-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e553-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e553-129">Response</span></span>

<span data-ttu-id="1e553-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e553-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e553-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1e553-131">Example</span></span>

<span data-ttu-id="1e553-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1e553-132">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1e553-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e553-133">Request</span></span>

<span data-ttu-id="1e553-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e553-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
```

##### <a name="response"></a><span data-ttu-id="1e553-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e553-135">Response</span></span>

<span data-ttu-id="1e553-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e553-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
