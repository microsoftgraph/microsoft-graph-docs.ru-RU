---
title: 'message: copy'
description: Копирование сообщения в папку.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3b02ef34b362cbe2b97623219a942b63ebd6d7eb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128794"
---
# <a name="message-copy"></a><span data-ttu-id="73dc4-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="73dc4-103">message: copy</span></span>

<span data-ttu-id="73dc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73dc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73dc4-105">Копирование сообщения в папку.</span><span class="sxs-lookup"><span data-stu-id="73dc4-105">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="73dc4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73dc4-106">Permissions</span></span>

<span data-ttu-id="73dc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73dc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73dc4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73dc4-109">Permission type</span></span> | <span data-ttu-id="73dc4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73dc4-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="73dc4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73dc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73dc4-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73dc4-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="73dc4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73dc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73dc4-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73dc4-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="73dc4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73dc4-115">Application</span></span> | <span data-ttu-id="73dc4-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73dc4-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="73dc4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73dc4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="73dc4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73dc4-118">Request headers</span></span>

| <span data-ttu-id="73dc4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73dc4-119">Header</span></span> | <span data-ttu-id="73dc4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="73dc4-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="73dc4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73dc4-121">Authorization</span></span> | <span data-ttu-id="73dc4-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="73dc4-122">`Bearer {token}`.</span></span> <span data-ttu-id="73dc4-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="73dc4-123">Required.</span></span> |
| <span data-ttu-id="73dc4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73dc4-124">Content-Type</span></span> | <span data-ttu-id="73dc4-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="73dc4-125">`application/json`.</span></span> <span data-ttu-id="73dc4-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="73dc4-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73dc4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73dc4-127">Request body</span></span>

<span data-ttu-id="73dc4-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="73dc4-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="73dc4-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="73dc4-129">Parameter</span></span> | <span data-ttu-id="73dc4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="73dc4-130">Type</span></span> | <span data-ttu-id="73dc4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="73dc4-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="73dc4-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="73dc4-132">destinationId</span></span>|<span data-ttu-id="73dc4-133">String</span><span class="sxs-lookup"><span data-stu-id="73dc4-133">String</span></span>|<span data-ttu-id="73dc4-134">Идентификатор целевой папки либо имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="73dc4-134">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="73dc4-135">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="73dc4-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="73dc4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="73dc4-136">Response</span></span>

<span data-ttu-id="73dc4-137">В случае успеха этот метод возвращает код отклика `201 Created` и ресурс [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73dc4-137">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73dc4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="73dc4-138">Example</span></span>

<span data-ttu-id="73dc4-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="73dc4-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="73dc4-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="73dc4-140">Request</span></span>

<span data-ttu-id="73dc4-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73dc4-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73dc4-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="73dc4-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="73dc4-143">C#</span><span class="sxs-lookup"><span data-stu-id="73dc4-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73dc4-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73dc4-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73dc4-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73dc4-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73dc4-146">Java</span><span class="sxs-lookup"><span data-stu-id="73dc4-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="73dc4-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="73dc4-147">Response</span></span>

<span data-ttu-id="73dc4-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="73dc4-148">Here is an example of the response.</span></span>

> <span data-ttu-id="73dc4-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73dc4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


