---
title: 'message: copy'
description: Копирование сообщения в папку.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2be9d62a8c5b44736612330ebb56fd3f13149e4c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274916"
---
# <a name="message-copy"></a><span data-ttu-id="f3f8b-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="f3f8b-103">message: copy</span></span>

<span data-ttu-id="f3f8b-104">Копирование сообщения в папку.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3f8b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f8b-105">Permissions</span></span>

<span data-ttu-id="f3f8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3f8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f3f8b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f8b-108">Permission type</span></span> | <span data-ttu-id="f3f8b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3f8b-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="f3f8b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3f8b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3f8b-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3f8b-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f3f8b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3f8b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3f8b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3f8b-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f3f8b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3f8b-114">Application</span></span> | <span data-ttu-id="f3f8b-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3f8b-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3f8b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3f8b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="f3f8b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3f8b-117">Request headers</span></span>

| <span data-ttu-id="f3f8b-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3f8b-118">Header</span></span> | <span data-ttu-id="f3f8b-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f3f8b-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="f3f8b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3f8b-120">Authorization</span></span> | <span data-ttu-id="f3f8b-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-121"></span></span> <span data-ttu-id="f3f8b-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-122">Required.</span></span> |
| <span data-ttu-id="f3f8b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f3f8b-123">Content-Type</span></span> | <span data-ttu-id="f3f8b-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-124"></span></span> <span data-ttu-id="f3f8b-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3f8b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3f8b-126">Request body</span></span>

<span data-ttu-id="f3f8b-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f3f8b-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="f3f8b-128">Parameter</span></span> | <span data-ttu-id="f3f8b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f3f8b-129">Type</span></span> | <span data-ttu-id="f3f8b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f3f8b-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="f3f8b-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="f3f8b-131">destinationId</span></span>|<span data-ttu-id="f3f8b-132">String</span><span class="sxs-lookup"><span data-stu-id="f3f8b-132">String</span></span>|<span data-ttu-id="f3f8b-133">Идентификатор целевой папки либо имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="f3f8b-134">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="f3f8b-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="f3f8b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3f8b-135">Response</span></span>

<span data-ttu-id="f3f8b-136">В случае успеха этот метод возвращает код отклика `201 Created` и ресурс [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3f8b-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f3f8b-137">Example</span></span>

<span data-ttu-id="f3f8b-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f3f8b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3f8b-139">Request</span></span>
<span data-ttu-id="f3f8b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f3f8b-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3f8b-141">Response</span></span>

<span data-ttu-id="f3f8b-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-142">Here is an example of the response.</span></span>

> <span data-ttu-id="f3f8b-143">**Примечание.**  Представленный здесь объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f3f8b-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3f8b-144">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f3f8b-145">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f3f8b-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f3f8b-146">C#</span><span class="sxs-lookup"><span data-stu-id="f3f8b-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_copy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3f8b-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="f3f8b-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_copy-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f3f8b-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f3f8b-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_copy-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-copy.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-copy.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-copy.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
