---
title: Отправка почты
description: Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9383da54b3cf326f27cc4b6f7c63f0bddb20a60
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893289"
---
# <a name="send-mail"></a><span data-ttu-id="8c1a5-104">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="8c1a5-104">Send mail</span></span>

<span data-ttu-id="8c1a5-p102">Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="8c1a5-107">Вы можете включить [вложенный файл](../resources/fileattachment.md) при вызове действия **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-107">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c1a5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c1a5-108">Permissions</span></span>
<span data-ttu-id="8c1a5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c1a5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8c1a5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c1a5-111">Permission type</span></span>      | <span data-ttu-id="8c1a5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c1a5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c1a5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c1a5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8c1a5-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8c1a5-114">Mail.Send</span></span>    |
|<span data-ttu-id="8c1a5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c1a5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c1a5-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8c1a5-116">Mail.Send</span></span>    |
|<span data-ttu-id="8c1a5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c1a5-117">Application</span></span> | <span data-ttu-id="8c1a5-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8c1a5-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c1a5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c1a5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="8c1a5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c1a5-120">Request headers</span></span>
| <span data-ttu-id="8c1a5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c1a5-121">Header</span></span>       | <span data-ttu-id="8c1a5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8c1a5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c1a5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c1a5-123">Authorization</span></span>  | <span data-ttu-id="8c1a5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8c1a5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c1a5-126">Content-Type</span></span>  | <span data-ttu-id="8c1a5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8c1a5-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c1a5-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c1a5-128">Request body</span></span>
<span data-ttu-id="8c1a5-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c1a5-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="8c1a5-130">Parameter</span></span>    | <span data-ttu-id="8c1a5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8c1a5-131">Type</span></span>   |<span data-ttu-id="8c1a5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c1a5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c1a5-133">message</span><span class="sxs-lookup"><span data-stu-id="8c1a5-133">message</span></span>|[<span data-ttu-id="8c1a5-134">Message</span><span class="sxs-lookup"><span data-stu-id="8c1a5-134">Message</span></span>](../resources/message.md)|<span data-ttu-id="8c1a5-p105">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="8c1a5-137">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="8c1a5-137">saveToSentItems</span></span>|<span data-ttu-id="8c1a5-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c1a5-138">Boolean</span></span>|<span data-ttu-id="8c1a5-p106">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8c1a5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c1a5-142">Response</span></span>

<span data-ttu-id="8c1a5-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c1a5-145">Пример</span><span class="sxs-lookup"><span data-stu-id="8c1a5-145">Example</span></span>
<span data-ttu-id="8c1a5-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-146">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="8c1a5-147">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="8c1a5-147">Request 1</span></span>
<span data-ttu-id="8c1a5-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8c1a5-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c1a5-149">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c1a5-150">C#</span><span class="sxs-lookup"><span data-stu-id="8c1a5-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c1a5-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c1a5-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c1a5-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c1a5-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8c1a5-153">Java</span><span class="sxs-lookup"><span data-stu-id="8c1a5-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="8c1a5-154">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="8c1a5-154">Response 1</span></span>
<span data-ttu-id="8c1a5-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="8c1a5-156">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="8c1a5-156">Request 2</span></span>
<span data-ttu-id="8c1a5-157">В следующем примере создается сообщение с использованием настраиваемых заголовков сообщений Интернета и выполняется его отправка.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-157">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8c1a5-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c1a5-158">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c1a5-159">C#</span><span class="sxs-lookup"><span data-stu-id="8c1a5-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c1a5-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c1a5-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c1a5-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c1a5-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8c1a5-162">Java</span><span class="sxs-lookup"><span data-stu-id="8c1a5-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="8c1a5-163">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="8c1a5-163">Response 2</span></span>
<span data-ttu-id="8c1a5-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c1a5-164">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
