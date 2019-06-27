---
title: Отправка почты
description: Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 65715f4ffe1df1f11dec93a2d9992b91eb6b29ac
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278668"
---
# <a name="send-mail"></a><span data-ttu-id="5b97e-104">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="5b97e-104">Send mail</span></span>

<span data-ttu-id="5b97e-p102">Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5b97e-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="5b97e-107">Вы можете включить [вложенный файл](../resources/fileattachment.md) при вызове действия **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="5b97e-107">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b97e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b97e-108">Permissions</span></span>
<span data-ttu-id="5b97e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b97e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5b97e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b97e-111">Permission type</span></span>      | <span data-ttu-id="5b97e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b97e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b97e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b97e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5b97e-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5b97e-114">Mail.Send</span></span>    |
|<span data-ttu-id="5b97e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b97e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b97e-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5b97e-116">Mail.Send</span></span>    |
|<span data-ttu-id="5b97e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b97e-117">Application</span></span> | <span data-ttu-id="5b97e-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5b97e-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b97e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b97e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="5b97e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b97e-120">Request headers</span></span>
| <span data-ttu-id="5b97e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b97e-121">Header</span></span>       | <span data-ttu-id="5b97e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5b97e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b97e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b97e-123">Authorization</span></span>  | <span data-ttu-id="5b97e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b97e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5b97e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b97e-126">Content-Type</span></span>  | <span data-ttu-id="5b97e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5b97e-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b97e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b97e-128">Request body</span></span>
<span data-ttu-id="5b97e-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5b97e-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5b97e-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="5b97e-130">Parameter</span></span>    | <span data-ttu-id="5b97e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5b97e-131">Type</span></span>   |<span data-ttu-id="5b97e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5b97e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b97e-133">message</span><span class="sxs-lookup"><span data-stu-id="5b97e-133">message</span></span>|[<span data-ttu-id="5b97e-134">Message</span><span class="sxs-lookup"><span data-stu-id="5b97e-134">Message</span></span>](../resources/message.md)|<span data-ttu-id="5b97e-p105">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b97e-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="5b97e-137">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="5b97e-137">saveToSentItems</span></span>|<span data-ttu-id="5b97e-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b97e-138">Boolean</span></span>|<span data-ttu-id="5b97e-p106">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="5b97e-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5b97e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b97e-142">Response</span></span>

<span data-ttu-id="5b97e-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5b97e-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b97e-145">Пример</span><span class="sxs-lookup"><span data-stu-id="5b97e-145">Example</span></span>
<span data-ttu-id="5b97e-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5b97e-146">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="5b97e-147">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="5b97e-147">Request 1</span></span>
<span data-ttu-id="5b97e-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b97e-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```

##### <a name="response-1"></a><span data-ttu-id="5b97e-149">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="5b97e-149">Response 1</span></span>
<span data-ttu-id="5b97e-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b97e-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5b97e-151">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5b97e-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5b97e-152">C#</span><span class="sxs-lookup"><span data-stu-id="5b97e-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b97e-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b97e-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5b97e-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b97e-154">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_sendmail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="5b97e-155">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="5b97e-155">Request 2</span></span>
<span data-ttu-id="5b97e-156">В следующем примере создается сообщение с использованием настраиваемых заголовков сообщений Интернета и выполняется его отправка.</span><span class="sxs-lookup"><span data-stu-id="5b97e-156">The next example creates a message with custom Internet message headers and sends the message.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "9/9/2018: concert",
    "body": {
      "contentType": "HTML",
      "content": "The group represents Nevada."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    ],
    "internetMessageHeaders":[
      {
        "name":"x-custom-header-group-name",
        "value":"Nevada"
      },
      {
        "name":"x-custom-header-group-id",
        "value":"NV001"
      }
    ]
  }
}
```

##### <a name="response-2"></a><span data-ttu-id="5b97e-157">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="5b97e-157">Response 2</span></span>
<span data-ttu-id="5b97e-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b97e-158">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5b97e-159">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5b97e-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5b97e-160">C#</span><span class="sxs-lookup"><span data-stu-id="5b97e-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b97e-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b97e-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5b97e-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b97e-162">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
