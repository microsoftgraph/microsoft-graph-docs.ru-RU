---
title: 'message: copy'
description: Копирование сообщения в папку.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 92ee0aeaa230015c0073177ab8f48e7ed5b91596
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43355211"
---
# <a name="message-copy"></a><span data-ttu-id="dacb8-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="dacb8-103">message: copy</span></span>

<span data-ttu-id="dacb8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dacb8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dacb8-105">Копирование сообщения в папку.</span><span class="sxs-lookup"><span data-stu-id="dacb8-105">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="dacb8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dacb8-106">Permissions</span></span>

<span data-ttu-id="dacb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dacb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dacb8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dacb8-109">Permission type</span></span> | <span data-ttu-id="dacb8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dacb8-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="dacb8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dacb8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dacb8-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dacb8-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dacb8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dacb8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dacb8-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dacb8-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dacb8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dacb8-115">Application</span></span> | <span data-ttu-id="dacb8-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dacb8-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dacb8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dacb8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="dacb8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dacb8-118">Request headers</span></span>

| <span data-ttu-id="dacb8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dacb8-119">Header</span></span> | <span data-ttu-id="dacb8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="dacb8-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="dacb8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dacb8-121">Authorization</span></span> | <span data-ttu-id="dacb8-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="dacb8-122">`Bearer {token}`.</span></span> <span data-ttu-id="dacb8-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dacb8-123">Required.</span></span> |
| <span data-ttu-id="dacb8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dacb8-124">Content-Type</span></span> | <span data-ttu-id="dacb8-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="dacb8-125">`application/json`.</span></span> <span data-ttu-id="dacb8-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dacb8-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dacb8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dacb8-127">Request body</span></span>

<span data-ttu-id="dacb8-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dacb8-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dacb8-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="dacb8-129">Parameter</span></span> | <span data-ttu-id="dacb8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dacb8-130">Type</span></span> | <span data-ttu-id="dacb8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dacb8-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="dacb8-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="dacb8-132">destinationId</span></span>|<span data-ttu-id="dacb8-133">String</span><span class="sxs-lookup"><span data-stu-id="dacb8-133">String</span></span>|<span data-ttu-id="dacb8-134">Идентификатор целевой папки либо имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="dacb8-134">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="dacb8-135">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="dacb8-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="dacb8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dacb8-136">Response</span></span>

<span data-ttu-id="dacb8-137">В случае успеха этот метод возвращает код отклика `201 Created` и ресурс [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dacb8-137">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dacb8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="dacb8-138">Example</span></span>

<span data-ttu-id="dacb8-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dacb8-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="dacb8-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="dacb8-140">Request</span></span>
<span data-ttu-id="dacb8-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dacb8-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dacb8-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="dacb8-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="dacb8-143">C#</span><span class="sxs-lookup"><span data-stu-id="dacb8-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dacb8-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dacb8-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dacb8-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dacb8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dacb8-146">Java</span><span class="sxs-lookup"><span data-stu-id="dacb8-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dacb8-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="dacb8-147">Response</span></span>

<span data-ttu-id="dacb8-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dacb8-148">Here is an example of the response.</span></span>

> <span data-ttu-id="dacb8-149">**Примечание.**  Представленный здесь объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dacb8-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dacb8-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dacb8-150">All the properties will be returned from an actual call.</span></span>
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
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
