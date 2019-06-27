---
title: 'message: forward'
description: Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 551a7186c25ae6b0251fa6bcf077ade8358d44fb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263737"
---
# <a name="message-forward"></a><span data-ttu-id="ae613-104">message: forward</span><span class="sxs-lookup"><span data-stu-id="ae613-104">message: forward</span></span>

<span data-ttu-id="ae613-p102">Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="ae613-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae613-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae613-107">Permissions</span></span>
<span data-ttu-id="ae613-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae613-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae613-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae613-110">Permission type</span></span>      | <span data-ttu-id="ae613-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae613-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae613-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae613-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ae613-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ae613-113">Mail.Send</span></span>    |
|<span data-ttu-id="ae613-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae613-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae613-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ae613-115">Mail.Send</span></span>    |
|<span data-ttu-id="ae613-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae613-116">Application</span></span> | <span data-ttu-id="ae613-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ae613-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae613-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae613-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="ae613-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae613-119">Request headers</span></span>
| <span data-ttu-id="ae613-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ae613-120">Name</span></span>       | <span data-ttu-id="ae613-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ae613-121">Type</span></span> | <span data-ttu-id="ae613-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ae613-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ae613-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae613-123">Authorization</span></span>  | <span data-ttu-id="ae613-124">string</span><span class="sxs-lookup"><span data-stu-id="ae613-124">string</span></span>  | <span data-ttu-id="ae613-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae613-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae613-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae613-127">Content-Type</span></span> | <span data-ttu-id="ae613-128">string</span><span class="sxs-lookup"><span data-stu-id="ae613-128">string</span></span>  | <span data-ttu-id="ae613-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae613-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae613-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae613-131">Request body</span></span>
<span data-ttu-id="ae613-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ae613-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ae613-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="ae613-133">Parameter</span></span>    | <span data-ttu-id="ae613-134">Тип</span><span class="sxs-lookup"><span data-stu-id="ae613-134">Type</span></span>   |<span data-ttu-id="ae613-135">Описание</span><span class="sxs-lookup"><span data-stu-id="ae613-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae613-136">comment</span><span class="sxs-lookup"><span data-stu-id="ae613-136">comment</span></span>|<span data-ttu-id="ae613-137">String</span><span class="sxs-lookup"><span data-stu-id="ae613-137">String</span></span>|<span data-ttu-id="ae613-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="ae613-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ae613-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="ae613-140">toRecipients</span></span>|<span data-ttu-id="ae613-141">Коллекция объектов [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="ae613-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="ae613-142">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="ae613-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="ae613-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae613-143">Response</span></span>

<span data-ttu-id="ae613-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ae613-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae613-146">Пример</span><span class="sxs-lookup"><span data-stu-id="ae613-146">Example</span></span>
<span data-ttu-id="ae613-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ae613-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae613-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae613-148">Request</span></span>
<span data-ttu-id="ae613-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae613-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="ae613-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae613-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="ae613-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae613-151">Response</span></span>
<span data-ttu-id="ae613-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae613-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ae613-153">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ae613-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ae613-154">C#</span><span class="sxs-lookup"><span data-stu-id="ae613-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_forward-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae613-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="ae613-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_forward-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ae613-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ae613-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_forward-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-forward.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-forward.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-forward.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
