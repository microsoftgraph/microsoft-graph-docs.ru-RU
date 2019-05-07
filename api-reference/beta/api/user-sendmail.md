---
title: Отправка почты
description: Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 469a47619db92bcb3b4234b7b39f390740d5a480
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637061"
---
# <a name="send-mail"></a><span data-ttu-id="932c3-104">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="932c3-104">Send mail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="932c3-p102">Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="932c3-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="932c3-107">В одном вызове метода **sendMail** можно выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="932c3-107">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="932c3-108">Включение [вложения](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="932c3-108">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="932c3-109">Используйте [упоминание](../resources/mention.md) , чтобы вызвонить другому пользователю в новом сообщении.</span><span class="sxs-lookup"><span data-stu-id="932c3-109">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="932c3-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="932c3-110">Permissions</span></span>
<span data-ttu-id="932c3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="932c3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="932c3-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="932c3-113">Permission type</span></span>      | <span data-ttu-id="932c3-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="932c3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="932c3-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="932c3-115">Delegated (work or school account)</span></span> | <span data-ttu-id="932c3-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="932c3-116">Mail.Send</span></span>    |
|<span data-ttu-id="932c3-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="932c3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="932c3-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="932c3-118">Mail.Send</span></span>    |
|<span data-ttu-id="932c3-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="932c3-119">Application</span></span> | <span data-ttu-id="932c3-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="932c3-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="932c3-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="932c3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="932c3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="932c3-122">Request headers</span></span>
| <span data-ttu-id="932c3-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="932c3-123">Header</span></span>       | <span data-ttu-id="932c3-124">Значение</span><span class="sxs-lookup"><span data-stu-id="932c3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="932c3-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="932c3-125">Authorization</span></span>  | <span data-ttu-id="932c3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="932c3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="932c3-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="932c3-128">Content-Type</span></span>  | <span data-ttu-id="932c3-129">application/json</span><span class="sxs-lookup"><span data-stu-id="932c3-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="932c3-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="932c3-130">Request body</span></span>
<span data-ttu-id="932c3-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="932c3-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="932c3-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="932c3-132">Parameter</span></span>    | <span data-ttu-id="932c3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="932c3-133">Type</span></span>   |<span data-ttu-id="932c3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="932c3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="932c3-135">Message</span><span class="sxs-lookup"><span data-stu-id="932c3-135">Message</span></span>|[<span data-ttu-id="932c3-136">Message</span><span class="sxs-lookup"><span data-stu-id="932c3-136">Message</span></span>](../resources/message.md)|<span data-ttu-id="932c3-p105">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="932c3-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="932c3-139">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="932c3-139">SaveToSentItems</span></span>|<span data-ttu-id="932c3-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="932c3-140">Boolean</span></span>|<span data-ttu-id="932c3-p106">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="932c3-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="932c3-144">Если вы хотите использовать **упоминание** , чтобы вызвонить другому пользователю в новом сообщении:</span><span class="sxs-lookup"><span data-stu-id="932c3-144">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="932c3-145">Включите в текст запроса обязательное свойство **toRecipients** , свойства **упоминаютх** и все доступные для записи свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="932c3-145">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="932c3-146">Для каждого упоминания в свойстве **упоминания** необходимо указать указанное свойство. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="932c3-146">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="932c3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="932c3-147">Response</span></span>

<span data-ttu-id="932c3-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="932c3-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="932c3-150">Пример</span><span class="sxs-lookup"><span data-stu-id="932c3-150">Example</span></span>
<span data-ttu-id="932c3-151">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="932c3-151">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="932c3-152">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="932c3-152">Request 1</span></span>
<span data-ttu-id="932c3-153">Ниже приведен пример запроса на динамическое создание и отправку сообщения.</span><span class="sxs-lookup"><span data-stu-id="932c3-153">Here is an example of the request to create and send a message on the fly.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 512

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
          "address": "samanthab@contoso.onmicrosoft.com"
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

##### <a name="response-1"></a><span data-ttu-id="932c3-154">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="932c3-154">Response 1</span></span>
<span data-ttu-id="932c3-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="932c3-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="932c3-156">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="932c3-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="932c3-157">Языках</span><span class="sxs-lookup"><span data-stu-id="932c3-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="932c3-158">Язык</span><span class="sxs-lookup"><span data-stu-id="932c3-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-2"></a><span data-ttu-id="932c3-159">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="932c3-159">Request 2</span></span>
<span data-ttu-id="932c3-160">В следующем примере показано сообщение от пользователя, выполнившего вход, в Samantha стенд.</span><span class="sxs-lookup"><span data-stu-id="932c3-160">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="932c3-161">Сообщение также содержит упоминание другого пользователя, дана свопе.</span><span class="sxs-lookup"><span data-stu-id="932c3-161">The message also includes a mention of another user, Dana Swope.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_mentions"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 344

{
  "Message": {
    "subject": "Project kickoff",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
  }
}
```

##### <a name="response-2"></a><span data-ttu-id="932c3-162">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="932c3-162">Response 2</span></span>
<span data-ttu-id="932c3-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="932c3-163">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="932c3-164">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="932c3-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="932c3-165">Языках</span><span class="sxs-lookup"><span data-stu-id="932c3-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail_with_mentions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="932c3-166">Язык</span><span class="sxs-lookup"><span data-stu-id="932c3-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail_with_mentions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-3"></a><span data-ttu-id="932c3-167">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="932c3-167">Request 3</span></span>
<span data-ttu-id="932c3-168">В следующем примере создается сообщение с использованием настраиваемых заголовков сообщений Интернета и выполняется его отправка.</span><span class="sxs-lookup"><span data-stu-id="932c3-168">The next example creates a message with custom Internet message headers and sends the message.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
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

##### <a name="response-3"></a><span data-ttu-id="932c3-169">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="932c3-169">Response 3</span></span>
<span data-ttu-id="932c3-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="932c3-170">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="932c3-171">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="932c3-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="932c3-172">Языках</span><span class="sxs-lookup"><span data-stu-id="932c3-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="932c3-173">Язык</span><span class="sxs-lookup"><span data-stu-id="932c3-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
