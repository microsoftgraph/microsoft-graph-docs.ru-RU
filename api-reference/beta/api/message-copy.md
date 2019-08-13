---
title: 'message: copy'
description: Копирование сообщения в папку.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d3e59c0eb8f248d98078878568414ab103529aaf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347033"
---
# <a name="message-copy"></a><span data-ttu-id="feac0-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="feac0-103">message: copy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feac0-104">Копирование сообщения в папку.</span><span class="sxs-lookup"><span data-stu-id="feac0-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="feac0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="feac0-105">Permissions</span></span>

<span data-ttu-id="feac0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="feac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="feac0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="feac0-108">Permission type</span></span> | <span data-ttu-id="feac0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="feac0-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="feac0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="feac0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="feac0-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="feac0-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="feac0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="feac0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="feac0-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="feac0-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="feac0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="feac0-114">Application</span></span> | <span data-ttu-id="feac0-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="feac0-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="feac0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="feac0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="feac0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="feac0-117">Request headers</span></span>

| <span data-ttu-id="feac0-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="feac0-118">Header</span></span> | <span data-ttu-id="feac0-119">Значение</span><span class="sxs-lookup"><span data-stu-id="feac0-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="feac0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="feac0-120">Authorization</span></span> | <span data-ttu-id="feac0-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="feac0-121"></span></span> <span data-ttu-id="feac0-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="feac0-122">Required.</span></span> |
| <span data-ttu-id="feac0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="feac0-123">Content-Type</span></span> | <span data-ttu-id="feac0-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="feac0-124"></span></span> <span data-ttu-id="feac0-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="feac0-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="feac0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="feac0-126">Request body</span></span>

<span data-ttu-id="feac0-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="feac0-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="feac0-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="feac0-128">Parameter</span></span> | <span data-ttu-id="feac0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="feac0-129">Type</span></span> | <span data-ttu-id="feac0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="feac0-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="feac0-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="feac0-131">destinationId</span></span>|<span data-ttu-id="feac0-132">String</span><span class="sxs-lookup"><span data-stu-id="feac0-132">String</span></span>|<span data-ttu-id="feac0-133">Идентификатор целевой папки либо имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="feac0-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="feac0-134">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="feac0-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="feac0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="feac0-135">Response</span></span>

<span data-ttu-id="feac0-136">В случае успеха этот метод возвращает код отклика `201 Created` и ресурс [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="feac0-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="feac0-137">Пример</span><span class="sxs-lookup"><span data-stu-id="feac0-137">Example</span></span>

<span data-ttu-id="feac0-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="feac0-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="feac0-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="feac0-139">Request</span></span>

<span data-ttu-id="feac0-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="feac0-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="feac0-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="feac0-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="feac0-142">C#</span><span class="sxs-lookup"><span data-stu-id="feac0-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="feac0-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="feac0-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="feac0-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="feac0-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="feac0-145">Java</span><span class="sxs-lookup"><span data-stu-id="feac0-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="feac0-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="feac0-146">Response</span></span>

<span data-ttu-id="feac0-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="feac0-147">Here is an example of the response.</span></span>

> <span data-ttu-id="feac0-148">**Примечание.**  Представленный здесь объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="feac0-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="feac0-149">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="feac0-149">All the properties will be returned from an actual call.</span></span>
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
